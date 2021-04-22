---
unique-page-id: 4720433
description: Configuration de protocoles pour Marketo - Marketo Docs - Documentation du produit
title: Configuration de protocoles pour Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---

# Configurer des protocoles pour Marketo {#configure-protocols-for-marketo}

Votre groupe marketing utilise Marketo pour créer des landings page de campagne et des courriers électroniques de marque. Pour s&#39;assurer que ces landings page et ces courriels fonctionnent, ils ont besoin d&#39;un peu d&#39;aide de la part de l&#39;informatique. Configurez les protocoles suivants avec les informations que votre groupe marketing aurait dû vous envoyer par courrier électronique.

Cet article doit être partagé avec le service informatique de la société qui souhaite mettre en oeuvre ces protocoles.

>[!NOTE]
>
>Si votre équipe informatique restreint l’accès au Web à l’aide d’une liste autorisée, demandez-lui d’ajouter les domaines suivants (y compris l’astérisque) pour autoriser toutes les ressources et les websockets Marketo :

* `*.marketo.com`

* `*.marketodesigner.com`

* `*.mktoweb.com`

## Étape 1 : Créer des enregistrements DNS pour les Landings page et les courriels {#step-create-dns-records-for-landing-pages-and-email}

**Suivi des CNAME de lien**

Votre équipe marketing aurait dû vous envoyer deux demandes d’enregistrement CNAME. La première concerne les URL de landing page, de sorte que les landings page apparaissent dans les URL qui reflètent votre domaine et non Marketo (l’hôte réel). La seconde concerne les liens de suivi inclus dans les courriers électroniques qu’ils envoient depuis Marketo.

`1` **Ajouter CNAME pour les Landings page**

Ajoutez le CNAME de landing page qu’ils vous ont envoyé à votre enregistrement DNS, de sorte que `[YourLandingPageCNAME]` pointe vers la chaîne de compte unique qui est attribuée à vos landings page Marketo. Connectez-vous au site du serveur d’inscriptions de votre domaine et saisissez le CNAME de landing page et la chaîne de compte. En règle générale, il s’agit de trois champs :

* Alias : Saisissez `[YourLandingPageCNAME]` (fourni par marketing)
* Type : CNAME
* Pointez sur : Saisissez `[MarketoAccountString].mktoweb.com` (fourni par marketing)

`2` **Ajouter CNAME pour les liens de Tracking email**

Ajoutez l’e-mail CNAME marketing qui vous a été envoyé de sorte que `[YourEmailCNAME]` pointe vers [MktoTrackingLink], le lien de suivi par défaut attribué par Marketo, au format suivant :\
`[YourEmailCNAME].[YourDomain].com` DANS CNAME  `[MktoTrackingLink]`

Par exemple :

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **Notifier votre équipe marketing**

Avertissez votre équipe marketing lorsque vous avez terminé ce processus.

## Étape 2 : Placer sur la liste autorisée les adresses IP Marketo {#step-allowlist-marketo-ips}

Lorsque votre groupe Marketing utilise Marketo pour envoyer des messages électroniques de test (une bonne pratique avant d’envoyer des messages instantanés), les messages électroniques de test sont parfois bloqués par des systèmes antispam qui reposent sur les adresses IP de l’expéditeur pour vérifier que le message est valide. Pour vous assurer que ces courriers électroniques de test arrivent, ajoutez Marketo à votre liste autorisée.

Ajoutez ces adresses IP à votre liste autorisée d’entreprise :

199.15.212.0/22\
192.28.144.0/20
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

Certains systèmes antispam utilisent le champ Chemin de retour du courrier électronique au lieu de l&#39;adresse IP pour autoriser l&#39;envoi. Dans ces cas, la meilleure approche consiste à placer sur la liste autorisée &quot;*.mktomail.com&quot;, car Marketo utilise plusieurs sous-domaines de boîtes aux lettres. D&#39;autres systèmes antispam placent sur la liste autorisée en fonction de l&#39;adresse De. Dans ces situations, veillez à inclure tous les domaines d’envoi (&quot;De&quot;) que votre groupe Marketing utilise pour communiquer avec les personnes/pistes.

>[!NOTE]
>
>Postini utilise une technologie unique et nécessite de placer sur la liste autorisée les plages d&#39;adresses IP. Voir [Liste autorisée avec Postini](https://nation.marketo.com/docs/DOC-1066).

## Étape 3 : Configurer SPF et DKIM {#step-set-up-spf-and-dkim}

Votre équipe marketing aurait également dû vous envoyer des informations DKIM à ajouter à votre enregistrement de ressource DNS (également répertorié ci-dessous). Suivez les étapes pour configurer avec succès DKIM et SPF, puis informez votre équipe marketing que ceci a été mis à jour.

1. Pour configurer SPF, ajoutez la ligne suivante à nos entrées DNS :

   `[CompanyDomain]` IN TXT v=spf1 mx ip4 :`[CorpIP]`\
   inclure : mktomail.com ~all

   Si notre entrée DNS contient déjà un enregistrement SPF existant, il suffit d&#39;y ajouter les éléments suivants :\
   inclure : mktomail.com

   Remplacez CompanyDomain par le domaine principal de votre site Web (ex : &quot;`(company.com/)`&quot;) et CorpIP avec l&#39;adresse IP de votre serveur de messagerie d&#39;entreprise (ex. &quot;255.255.255.255&quot;). Si vous envoyez des courriers électroniques de plusieurs domaines via Marketo, votre personnel informatique doit ajouter cette ligne pour chaque domaine (sur une seule ligne).

1. Pour DKIM, créez des enregistrements de ressources DNS pour chaque domaine à configurer. Vous trouverez ci-dessous les enregistrements d’hôtes et les valeurs TXT pour chaque domaine pour lequel nous allons signer :

   `[DKIMDomain1]`: L’enregistrement d’hôte est défini  `[HostRecord1]` et la valeur TXT est  `[TXTValue1]`définie.

   `[DKIMDomain2]`: L’enregistrement d’hôte est défini  `[HostRecord2]` et la valeur TXT est  `[TXTValue2]`définie.

   Copiez l&#39;enregistrement hôte et la valeur TXTValue pour chaque domaine DKIMDomain que vous avez configuré après avoir suivi les [instructions ici](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). N’oubliez pas de vérifier chaque domaine dans Admin > Email > DKIM une fois que votre personnel informatique a terminé cette étape.

## Étape 4 : Configurer des enregistrements MX pour votre domaine {#step-set-up-mx-records-for-your-domain}

Un enregistrement MX vous permet de recevoir du courrier dans le domaine à partir duquel vous envoyez du courrier électronique pour traiter les réponses et les répondeurs automatiques. Si vous envoyez des données à partir de votre domaine d’entreprise, il est probable que vous ayez déjà configuré cette option. Si ce n’est pas le cas, vous pouvez généralement le configurer pour le mapper à l’enregistrement MX de votre domaine d’entreprise.
