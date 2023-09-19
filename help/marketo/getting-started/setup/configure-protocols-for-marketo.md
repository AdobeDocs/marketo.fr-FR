---
unique-page-id: 4720433
description: Configuration de protocoles pour Marketo - Documents Marketo - Documentation du produit
title: Configuration de protocoles pour Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 0d6507c251e2b7567483af8d75158f6bc6a1ca49
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 4%

---

# Configuration de protocoles pour Marketo {#configure-protocols-for-marketo}

Si vous ou votre entreprise utilisez des paramètres de pare-feu ou de serveur proxy restrictifs, vous ou votre administrateur réseau devrez peut-être placer sur la liste autorisée certains domaines et plages d’adresses IP pour vous assurer que Adobe Marketo Engage fonctionne comme prévu.

## Pages d’entrée et emails de campagne de marque {#branded-campaign-landing-pages-and-emails}

Votre groupe marketing utilise Marketo pour créer des landing pages et des emails de campagne de marque. Pour s’assurer que ces landing pages et ces emails fonctionnent, le service informatique doit les aider un peu. Configurez les protocoles suivants, avec les informations que votre groupe marketing aurait dû vous envoyer par e-mail.

Cet article doit être partagé avec le service informatique de la société souhaitant mettre en oeuvre ces protocoles.

Si votre équipe informatique restreint l’accès web à l’aide d’une liste autorisée, demandez-lui d’ajouter les domaines suivants (y compris l’astérisque) pour autoriser toutes les ressources et tous les websockets Marketo :

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Étape 1 : création d’enregistrements DNS pour les pages d’entrée et les courriers électroniques {#step-create-dns-records-for-landing-pages-and-email}

**Suivi des CNAME de lien**

Votre équipe marketing aurait dû vous envoyer deux demandes de nouveaux enregistrements CNAME. La première concerne les URL de page d’entrée, de sorte que les pages d’entrée apparaissent dans les URL qui reflètent votre domaine et non dans Marketo (l’hôte réel). La seconde concerne les liens de tracking inclus dans les emails qu’ils envoient à partir de Marketo.

`1` **Ajout d’un CNAME pour les pages d’entrée**

Ajoutez le CNAME de page d’entrée qu’il vous a envoyé à votre enregistrement DNS, de sorte que `[YourLandingPageCNAME]` pointe vers la chaîne de compte unique attribuée à vos pages d’entrée Marketo. Connectez-vous au site du serveur d’inscriptions de votre domaine et saisissez la landing page CNAME et la chaîne de compte. En règle générale, cela implique trois champs :

* Alias : Entrée `[YourLandingPageCNAME]` (fourni par le marketing)
* Type : CNAME
* Point vers : Entrée `[MunchkinID].mktoweb.com` (fourni par le marketing)

`2` **Ajout d’un CNAME pour les liens de suivi des emails**

Ajoutez l’e-mail marketing CNAME qui vous a été envoyé, de sorte que `[YourEmailCNAME]` pointe vers [MktoTrackingLink], le lien de suivi par défaut attribué par Marketo, au format :\
`[YourEmailCNAME].[YourDomain].com` DANS CNAME `[MktoTrackingLink]`

Par exemple :

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` doit être le domaine de marque par défaut.

`3` **Notifier votre équipe marketing**

Avertissez votre équipe marketing lorsque vous avez terminé ce processus.

`4` **Contact [Prise en charge de Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} pour lancer le processus de configuration d’un certificat SSL.**

Ce processus peut prendre jusqu’à 3 jours ouvrables.

## Étape 2 : Placer sur la liste autorisée les adresses IP Marketo {#step-allowlist-marketo-ips}

Lorsque votre groupe marketing utilise Marketo pour envoyer des emails de test (une bonne pratique avant d’envoyer des messages indésirables), les emails de test sont parfois bloqués par des systèmes anti-spam qui reposent sur des adresses IP d’expéditeur pour vérifier que l’email est valide. Pour vous assurer que ces courriers électroniques de test arrivent, ajoutez Marketo à votre liste autorisée.

Ajoutez les adresses IP suivantes à la liste autorisée de votre entreprise :

94.236.119.0/26

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Certains systèmes anti-spam utilisent le champ Chemin d’accès au retour de l’email au lieu de l’adresse IP pour la mise en liste autorisée. Dans ce cas, la meilleure approche consiste à placer sur la liste autorisée &quot;&quot;&#42;.mktomail.com&#39;, car Marketo utilise plusieurs sous-domaines de boîte aux lettres. D’autres systèmes anti-spam placent sur la liste autorisée en fonction de l’adresse de l’expéditeur. Dans ce cas, veillez à inclure tous les domaines d’envoi (&quot;De&quot;) que votre groupe marketing utilise pour communiquer avec les personnes/prospects.

>[!NOTE]
>
>Postini utilise une technologie unique et nécessite de placer sur la liste autorisée des plages d’adresses IP. Voir [Placer sur la liste autorisée avec Postini](https://nation.marketo.com/docs/DOC-1066).

## Étape 3 : configuration de SPF et DKIM {#step-set-up-spf-and-dkim}

Votre équipe marketing aurait également dû vous envoyer des informations DKIM à ajouter à votre enregistrement de ressource DNS (également répertorié ci-dessous). Suivez les étapes pour configurer correctement DKIM et SPF, puis informez votre équipe marketing que cette configuration a été mise à jour.

1. Pour configurer SPF, ajoutez la ligne suivante à nos entrées DNS :

   `[CompanyDomain]` DANS TXT v=spf1 mx ip4 :`[CorpIP]`\
   include : mktomail.com ~all

   Si nous avons déjà un enregistrement SPF existant dans notre entrée DNS, ajoutez-y simplement les éléments suivants :\
   include : mktomail.com

   Remplacez CompanyDomain par le domaine principal de votre site web (par exemple : &quot;`(company.com/)`&quot;) et CorpIP avec l’adresse IP de votre serveur de messagerie d’entreprise (ex. &quot;255.255.255.255&quot;). Si vous allez envoyer des emails à partir de plusieurs domaines via Marketo, votre personnel informatique doit ajouter cette ligne pour chaque domaine (sur une seule ligne).

1. Pour DKIM, créez des enregistrements de ressources DNS pour chaque domaine que nous souhaitons configurer. Vous trouverez ci-dessous les enregistrements d’hôte et les valeurs TXT pour chaque domaine pour lequel nous allons signer :

   `[DKIMDomain1]`: l’enregistrement de l’hôte `[HostRecord1]` et la valeur TXT est `[TXTValue1]`.

   `[DKIMDomain2]`: l’enregistrement de l’hôte `[HostRecord2]` et la valeur TXT est `[TXTValue2]`.

   Copiez HostRecord et TXTValue pour chaque domaine DKIMD que vous avez configuré après avoir suivi les [instructions ici](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. N’oubliez pas de vérifier chaque domaine dans Admin > Email > DKIM une fois que votre équipe informatique a terminé cette étape.

## Étape 4 : configuration des enregistrements MX pour votre domaine {#step-set-up-mx-records-for-your-domain}

Un enregistrement MX vous permet de recevoir du courrier électronique vers le domaine à partir duquel vous envoyez le courrier électronique pour traiter les réponses et les réponses automatiques. Si vous envoyez depuis votre domaine d’entreprise, il est probable que celui-ci soit déjà configuré. Si ce n’est pas le cas, vous pouvez généralement le configurer pour qu’il corresponde à l’enregistrement MX de votre domaine d’entreprise.

## Adresse IP sortante {#outbound-ip-addresses}

Une connexion sortante est une connexion établie par un Marketo Engage à un serveur sur Internet en votre nom. Certains partenaires/fournisseurs avec lesquels vous travaillez, ou votre propre organisation informatique, peuvent utiliser des listes autorisées pour restreindre l’accès aux serveurs. Si tel est le cas, vous devez leur fournir des blocs d’adresses IP sortantes Marketo Engage à ajouter à leurs listes autorisées.

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} l’action de flux est exécutée dans le cadre d’une campagne dynamique, une requête HTTP est envoyée à un service Web externe. Si l’éditeur du service Web utilise une liste autorisée sur le pare-feu du réseau sur lequel se trouve le service Web externe, l’éditeur doit ajouter les blocs d’adresse IP répertoriés ci-dessous à sa liste autorisée.

**Synchronisation CRM**

Marketo Engage [Synchronisation CRM Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} sont des mécanismes d’intégration qui renvoient des requêtes HTTP sortantes aux API publiées par votre fournisseur de gestion de la relation client. Vous devez vous assurer que votre service informatique ne bloque aucun des blocs d’adresses IP ci-dessous pour accéder aux API de votre fournisseur de gestion de la relation client.

**Blocs d’adresses IP sortantes du Marketo Engage**

Les tableaux suivants couvrent tous les serveurs Marketo Engage qui effectuent des appels sortants. Utilisez les listes ci-dessous si vous configurez une liste autorisée IP, un serveur, un pare-feu, une liste de contrôle d’accès, un groupe de sécurité ou un service tiers pour recevoir les connexions sortantes de Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Bloc d’adresse IP (notation CIDR)</th>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>130.248.244.88/29</td>
  </tr>
  <tr>
   <td>185.28.196.0/22</td>
  </tr>
  <tr>
   <td>192.28.144.0/20</td>
  </tr>
  <tr>
   <td>192.28.160.0/19</td>
  </tr>
  <tr>
   <td>199.15.212.0/22</td>
  </tr>
 </tbody>
</table>

<table>
 <tbody>
  <tr>
   <th>Adresse IP individuelle</th>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
  <tr>
   <td>35.165.244.220</td>
  </tr>
  <tr>
   <td>44.235.171.179</td>
  </tr>
  <tr>
   <td>52.20.211.99</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
  <tr>
   <td>54.220.138.65</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.16</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>

</tbody>
</table>

