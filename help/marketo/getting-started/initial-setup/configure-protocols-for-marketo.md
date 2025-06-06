---
unique-page-id: 4720433
description: Configuration de protocoles pour Marketo Engage - Documentation du Marketo Engage - Documentation du produit
title: Configuration de protocoles pour Marketo Engage
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: ed42e3662dc1f9c3b3b27d86d1df816ce26e1076
workflow-type: tm+mt
source-wordcount: '2148'
ht-degree: 0%

---

# Configuration de protocoles pour Marketo Engage{#configure-protocols-for-marketo-engage}

Si vous ou votre entreprise utilisez des paramètres de pare-feu ou de serveur proxy restrictifs, vous ou votre administrateur réseau devrez peut-être placer sur la liste autorisée certains domaines et plages d’adresses IP pour vous assurer que Adobe Marketo Engage fonctionne comme prévu.

Pour obtenir de l’aide sur la mise en oeuvre des protocoles ci-dessous, veuillez partager cet article avec votre service informatique. S’ils limitent l’accès web à l’aide d’une liste autorisée, veillez à ajouter les domaines suivants (y compris l’astérisque) pour autoriser toutes les ressources et tous les websockets du Marketo Engage :

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Étape 1 : création d’enregistrements DNS pour les pages d’entrée et les courriers électroniques {#step-create-dns-records-for-landing-pages-and-email}

**CNAME de lien de suivi**

Votre équipe marketing aurait dû vous envoyer deux demandes de nouveaux enregistrements CNAME. La première concerne les URL de page d’entrée, de sorte que les landing pages apparaissent dans les URL qui représentent votre domaine et non le Marketo Engage (l’hôte réel). La seconde concerne les liens de tracking inclus dans les emails qu’ils envoient depuis Marketo Engage.

`1` **Ajouter un CNAME pour les pages d’entrée**

Ajoutez le CNAME de page d’entrée qu’ils vous ont envoyé à votre enregistrement DNS, de sorte que `[YourLandingPageCNAME]` pointe vers la chaîne de compte unique attribuée à vos pages d’entrée de Marketo Engage. Connectez-vous au site du serveur d’inscriptions de votre domaine et saisissez la landing page CNAME et la chaîne de compte. En règle générale, cela implique trois champs :

* Alias : Entrée `[YourLandingPageCNAME]` (fourni par le marketing)
* Type : CNAME
* Point à : Entrée `[MunchkinID].mktoweb.com` (fourni par le marketing)

`2` **Ajouter un CNAME pour les liens de suivi des emails**

Ajoutez l’e-mail CNAME marketing qui vous a été envoyé, de sorte que `[YourEmailCNAME]` pointe vers [MktoTrackingLink], le lien de suivi par défaut attribué par le Marketo Engage, au format suivant :\
`[YourEmailCNAME].[YourDomain].com` DANS CNAME `[MktoTrackingLink]`

Par exemple :

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` doit être le domaine de marque par défaut.

`3` **Avertir votre équipe marketing**

Avertissez votre équipe marketing lorsque vous avez terminé ce processus.

`4` **Contactez le [support d&#39;Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} pour lancer le processus de mise en service d&#39;un certificat SSL.**

Ce processus peut prendre jusqu’à 3 jours ouvrables.

## Étape 2 : Placer sur la liste autorisée les adresses IP des Marketo Engage {#step-allowlist-marketo-ips}

Lorsque votre groupe marketing utilise Marketo Engage pour envoyer des emails de test (une bonne pratique avant d’envoyer des messages indésirables), les emails de test sont parfois bloqués par des systèmes anti-spam qui reposent sur des adresses IP d’expéditeur pour vérifier que l’email est valide. Pour vous assurer que ces emails de test arrivent, ajoutez Marketo Engage à votre liste autorisée.

Ajoutez les adresses IP suivantes à la liste autorisée de votre entreprise :

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Certains systèmes anti-spam utilisent le champ Chemin d’accès au retour de l’email au lieu de l’adresse IP pour la mise en liste autorisée. Dans ces cas, la meilleure approche consiste à placer sur la liste autorisée &#39;&#42;.mktomail.com&#39;, car Marketo Engage utilise plusieurs sous-domaines de boîte aux lettres. D’autres systèmes anti-spam placent sur la liste autorisée en fonction de l’adresse de l’expéditeur. Dans ce cas, veillez à inclure tous les domaines d’envoi (&quot;De&quot;) que votre groupe marketing utilise pour communiquer avec les personnes/prospects.

>[!NOTE]
>
>Postini utilise une technologie unique et nécessite de placer sur la liste autorisée des plages d’adresses IP. Voir [Placer sur la liste autorisée avec Postini](https://nation.marketo.com/docs/DOC-1066).

## Étape 3 : configuration SPF et DKIM {#step-set-up-spf-and-dkim}

Votre équipe marketing doit également vous avoir envoyé des informations DKIM (Domain Keys Identified Mail) à ajouter à votre enregistrement de ressource DNS (également répertorié ci-dessous). Suivez les étapes pour configurer correctement DKIM et SPF (Sender Policy Framework), puis informez votre équipe marketing que cette configuration a été mise à jour.

1. Pour configurer SPF, ajoutez la ligne suivante à nos entrées DNS :

   `[CompanyDomain]` DANS TXT v=spf1 mx ip4:`[CorpIP]`\
   include : mktomail.com ~all

   Si nous avons déjà un enregistrement SPF existant dans notre entrée DNS, ajoutez-y simplement les éléments suivants :\
   include : mktomail.com

   Remplacez CompanyDomain par le domaine principal de votre site web (ex : &quot;`(company.com/)`&quot;) et CorpIP par l’adresse IP de votre serveur de messagerie d’entreprise (ex. : &quot;255.255.255.255&quot;). Si vous allez envoyer des emails à partir de plusieurs domaines par le biais de Marketo Engage, votre personnel informatique doit ajouter cette ligne pour chaque domaine (sur une seule ligne).

1. Pour DKIM, créez des enregistrements de ressources DNS pour chaque domaine que nous voulons configurer. Vous trouverez ci-dessous les enregistrements d’hôte et les valeurs TXT pour chaque domaine pour lequel nous allons signer :

   `[DKIMDomain1]` : l’enregistrement hôte est `[HostRecord1]` et la valeur TXT est `[TXTValue1]`.

   `[DKIMDomain2]` : l’enregistrement hôte est `[HostRecord2]` et la valeur TXT est `[TXTValue2]`.

   Copiez HostRecord et TXTValue pour chaque domaine DKIMDomain que vous avez configuré après avoir suivi les [instructions ici](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. N’oubliez pas de vérifier chaque domaine dans Admin > Email > DKIM une fois que votre personnel informatique a terminé cette étape.

## Étape 4 : configuration de DMARC {#set-up-dmarc}

DMARC (Domain-based Message Authentication, Reporting &amp; Conformance) est un protocole d’authentification utilisé pour aider les organisations à protéger leur domaine contre toute utilisation non autorisée. DMARC étend les protocoles d’authentification existants, tels que SPF et DKIM, pour informer les serveurs de destinataires des actions qu’ils doivent entreprendre en cas d’échec de l’authentification sur leur domaine. Bien que DMARC soit actuellement facultatif, il est vivement recommandé, car il protège mieux la marque et la réputation de votre entreprise. À compter de février 2024, les principaux fournisseurs tels que Google et Yahoo auront besoin de DMARC pour les expéditeurs en masse.

Pour que DMARC fonctionne, vous devez disposer d’au moins un des enregistrements TXT DNS suivants :

* Un SPF valide
* Un enregistrement DKIM valide pour votre formulaire FROM : domaine (recommandé pour Marketo Engage)

En outre, vous devez disposer d’un enregistrement TXT DNS spécifique à DMARC pour votre domaine FROM : Domain. Vous pouvez éventuellement définir une adresse électronique de votre choix pour indiquer où les rapports DMARC doivent se rendre au sein de votre organisation, afin de pouvoir surveiller les rapports.

Il est recommandé de déployer lentement la mise en oeuvre de DMARC en réaffectant la stratégie DMARC de p=none, à p=quarantine, puis à p=reject lorsque vous comprenez l’impact potentiel de DMARC et en définissant votre stratégie DMARC pour assouplir l’alignement sur SPF et DKIM.

### Exemple de processus DMARC {#dmarc-example-workflow}

1. Si vous êtes configuré pour recevoir des rapports DMARC, procédez comme suit...

   I. Analysez les commentaires et les rapports que vous recevez et utilisez (p=none), qui indique au destinataire d’effectuer aucune action contre les messages qui ne parviennent pas à s’authentifier, tout en envoyant des rapports par courrier électronique à l’expéditeur.

   II. Vérifiez et corrigez les problèmes liés à SPF/DKIM si les messages légitimes échouent à l’authentification.

   III. Déterminez si SPF ou DKIM sont alignés et transmettent l’authentification pour tous les emails légitimes.

   IV. Consultez les rapports pour vous assurer que les résultats correspondent à vos attentes en fonction de vos stratégies SPF/DKIM.

1. Passez à la stratégie (p=quarantine), qui indique au serveur de messagerie de réception de mettre en quarantaine les emails qui ne parviennent pas à s’authentifier (cela signifie généralement placer ces messages dans le dossier spam).

   I. Consultez les rapports pour vous assurer que les résultats correspondent à vos attentes.

1. Si vous êtes satisfait du comportement des messages au niveau p=quarantaine, vous pouvez ajuster la stratégie à (p=rejets). La stratégie p=reject indique au destinataire de refuser complètement (rebond) tout courrier électronique pour le domaine qui échoue à l’authentification. Lorsque cette stratégie est activée, seul le courrier électronique vérifié comme authentifié à 100 % par votre domaine aura une chance d’être placé dans une boîte de réception.

>[!CAUTION]
>
>Utilisez cette stratégie avec précaution et déterminez si elle convient à votre entreprise.

### Rapports DMARC {#dmarc-reporting}

DMARC permet de recevoir des rapports sur les emails qui échouent SPF/DKIM. Il existe deux rapports différents générés par les services de FAI dans le cadre du processus d’authentification que les expéditeurs peuvent recevoir par le biais des balises RUA/RUF de leur stratégie DMARC.

* Rapports d’agrégation (RUA) : ne contient aucune information d’identification personnelle qui serait sensible au RGPD (Règlement général sur la protection des données).

* Rapports médico-légaux (RUF) : contient des adresses électroniques sensibles au RGPD. Avant d’utiliser , il est préférable de vérifier en interne comment traiter les informations qui doivent être conformes au RGPD.

L’utilisation principale de ces rapports consiste à recevoir un aperçu des emails qui ont fait l’objet d’une tentative d’usurpation. Il s’agit de rapports hautement techniques qui sont le mieux digérés au moyen d’un outil tiers.

### Exemples d’enregistrements DMARC {#example-dmarc-records}

* Bare Minimum Record : `v=DMARC1; p=none`

* Enregistrement de la direction vers une adresse électronique pour recevoir des rapports : `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### Balises DMARC et leurs actions {#dmarc-tags-and-what-they-do}

Les enregistrements DMARC comportent plusieurs composants appelés balises DMARC. Chaque balise a une valeur qui spécifie un certain aspect de DMARC.

<table>
<thead>
  <tr>
    <th>Nom de balise </th>
    <th>Obligatoire / Facultatif </th>
    <th>Fonction </th>
    <th>Exemple </th>
    <th>Valeur par défaut </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>Obligatoire</td>
    <td>Cette balise DMARC spécifie la version. Il n’existe qu’une seule version pour l’instant. Par conséquent, cette version aura une valeur fixe v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>Obligatoire</td>
    <td>Affiche la stratégie DMARC sélectionnée et demande au destinataire de signaler, mettre en quarantaine ou rejeter les messages qui ne parviennent pas aux vérifications d’authentification.</td>
    <td>p=aucun, mise en quarantaine ou rejet</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Facultatif</td>
    <td>Permet au propriétaire du domaine de spécifier des options de création de rapports.</td>
    <td>0 : générer un rapport si tout échoue 
    <br>1 : générer un rapport en cas d’échec 
    <br>d : générer un rapport en cas d’échec de DKIM 
    <br>s : générer un rapport en cas d’échec du SPF</td>
    <td>1 (recommandé pour les rapports DMARC)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>Facultatif</td>
    <td>Indique le pourcentage de messages soumis au filtrage.</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>Facultatif (recommandé)</td>
    <td>Identifie l’emplacement où les rapports agrégés seront distribués.</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>Facultatif (recommandé)</td>
    <td>Identifie l’endroit où les rapports médico-légaux seront remis.</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>Facultatif</td>
    <td>Spécifie la stratégie DMARC pour les sous-domaines du domaine parent.</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>Facultatif</td>
    <td>Peut être Strict (s) ou Relaxé ®. Un alignement décontracté signifie que le domaine utilisé dans la signature DKIM peut être un sous-domaine de l’adresse "De". Un alignement strict signifie que le domaine utilisé dans la signature DKIM doit correspondre exactement à celui utilisé dans l’adresse De.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>Facultatif</td>
    <td>Peut être Strict (s) ou Relaxé ®. Un alignement relâché signifie que le domaine ReturnPath peut être un sous-domaine de l’adresse de l’expéditeur. Un alignement strict signifie que le domaine Return-Path doit correspondre exactement à l’adresse From.</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

Pour plus d’informations sur DMARC et toutes ses options, consultez le site [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC et Marketo Engage {#dmarc-and-marketo-engage}

Il existe deux types d’alignement pour DMARC : l’alignement DKIM et l’alignement SPF.

>[!NOTE]
>
>Il est recommandé d’aligner DMARC sur DKIM par rapport à SPF pour Marketo Engage.

* DMARC aligné sur DKIM : pour configurer le DMARC aligné sur DKIM, vous devez :

   * Configurez DKIM pour le formulaire DE : domaine de votre message. Suivez les instructions [ de cet article ](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Configuration de DMARC pour le domaine From:/DKIM configuré précédemment

* SPF aligné sur DMARC : pour configurer SPF aligné sur DMARC via un chemin de retour de marque, vous devez :

   * Configuration d’un domaine de chemin d’accès retour de marque
      * Configuration de l’enregistrement SPF approprié
      * Modifiez l’enregistrement MX pour qu’il revienne au MX par défaut du centre de données dans lequel votre courrier sera envoyé.

   * Configuration de DMARC pour le domaine de chemin d’accès retour de marque

* Si vous envoyez des courriers électroniques à partir d’un Marketo Engage via une adresse IP dédiée et que vous n’avez pas encore mis en oeuvre de chemin de retour de marque, ou que vous n’êtes pas sûr de l’avoir fait, veuillez ouvrir un ticket avec l’[assistance Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Si vous envoyez du courrier du Marketo Engage par le biais d’un pool partagé d’adresses IP, vous pouvez voir si vous remplissez les critères pour les adresses IP de confiance en [appliquant ici](http://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. Le chemin de retour de marque est proposé gratuitement aux envois à partir des adresses IP approuvées du Marketo Engage. Si ce programme est approuvé, contactez le support Adobe pour configurer le chemin de retour de marque.

   * Adresses IP approuvées : groupe d’adresses IP partagées réservé aux utilisateurs à volume inférieur qui envoient &lt;75 K/mois et qui ne remplissent pas les critères pour une adresse IP dédiée. Ces utilisateurs doivent également respecter les exigences relatives aux bonnes pratiques.

* Si vous envoyez des courriers électroniques de Marketo Engage par le biais d’adresses IP partagées et que vous ne remplissez pas les critères pour les adresses IP de confiance et que vous envoyez plus de 100 000 messages par mois, vous devrez contacter l’équipe du compte Adobe (votre gestionnaire de compte) pour acheter une adresse IP dédiée.

* L’alignement Strict SPF n’est ni pris en charge ni recommandé dans Marketo Engage.

## Étape 5 : configuration des enregistrements MX pour votre domaine {#step-set-up-mx-records-for-your-domain}

Un enregistrement MX vous permet de recevoir du courrier électronique vers le domaine à partir duquel vous envoyez le courrier électronique pour traiter les réponses et les réponses automatiques. Si vous envoyez depuis votre domaine d’entreprise, il est probable que celui-ci soit déjà configuré. Si ce n’est pas le cas, vous pouvez généralement le configurer pour qu’il corresponde à l’enregistrement MX de votre domaine d’entreprise.

## Adresse IP sortante {#outbound-ip-addresses}

Une connexion sortante est une connexion établie par un Marketo Engage à un serveur sur Internet en votre nom. Certains partenaires/fournisseurs avec lesquels vous travaillez, ou votre propre organisation informatique, peuvent utiliser des listes autorisées pour restreindre l’accès aux serveurs. Si tel est le cas, vous devez leur fournir des blocs d’adresses IP sortantes Marketo Engage à ajouter à leurs listes autorisées.

**Webhooks**

Le Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} est un mécanisme d’intégration sortante. Lorsqu’une action de flux [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} est exécutée dans le cadre d’une campagne dynamique, une requête HTTP est envoyée à un service Web externe. Si l’éditeur du service Web utilise une liste autorisée sur le pare-feu du réseau sur lequel se trouve le service Web externe, l’éditeur doit ajouter les blocs d’adresse IP répertoriés ci-dessous à sa liste autorisée.

**Synchronisation CRM**

Le Marketo Engage [Salesforce CRM Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} et [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} sont des mécanismes d’intégration qui effectuent des requêtes HTTP sortantes vers des API publiées par votre fournisseur de gestion de la relation client. Vous devez vous assurer que votre service informatique ne bloque aucun des blocs d’adresses IP ci-dessous pour accéder aux API de votre fournisseur de gestion de la relation client.

**Blocs d’adresses IP sortantes Marketo Engage**

Les tableaux suivants couvrent tous les serveurs Marketo Engage qui effectuent des appels sortants. Utilisez les listes ci-dessous si vous configurez une liste autorisée IP, un serveur, un pare-feu, une liste de contrôle d’accès, un groupe de sécurité ou un service tiers pour recevoir les connexions sortantes de Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Bloc d’adresse IP (notation CIDR)</th>
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
  <tr>
   <td>124.47.174.193</td>
  </tr>
  <tr>
   <td>130.248.168.16</td>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
  <tr>
   <td>199.15.213.245</td>
  </tr>
  <tr>
   <td>199.15.215.245</td>
  </tr>
 </tbody>
</table>
