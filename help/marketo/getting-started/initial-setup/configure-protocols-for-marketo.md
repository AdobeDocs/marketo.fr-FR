---
unique-page-id: 4720433
description: Configurer les protocoles pour Marketo Engage - Documents Marketo Engage - Documentation du produit
title: Configurer les protocoles pour Marketo Engage
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '2129'
ht-degree: 100%

---

# Configurer les protocoles pour Marketo Engage{#configure-protocols-for-marketo-engage}

Si vous ou votre entreprise utilisez des paramètres de pare-feu ou de serveur proxy restrictifs, vous (ou votre administrateur ou administratrice réseau) devrez peut-être placer sur la liste autorisée certains domaines et plages d’adresses IP pour vous assurer que Adobe Marketo Engage fonctionne comme prévu.

Pour obtenir de l’aide sur la mise en œuvre des protocoles ci-dessous, veuillez partager cet article avec votre service informatique. Si votre service informatique restreint l’accès web à l’aide d’une liste autorisée, demandez-leur d’ajouter les domaines suivants (y compris l’astérisque) pour autoriser toutes les ressources et tous les sockets web de Marketo Engage :

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Étape 1 : créer des enregistrements DNS pour les pages de destination et les e-mails {#step-create-dns-records-for-landing-pages-and-email}

**CNAME du lien de suivi**

Votre équipe marketing a dû vous envoyer deux demandes de nouveaux enregistrements CNAME. La première concerne les URL des pages de destination. Celles-ci apparaissent donc dans des URL qui reflètent votre domaine et non Marketo Engage (l’hôte réel). La seconde concerne les liens de suivi inclus dans les e-mails qu’ils envoient à partir de Marketo Engage.

`1` **Ajouter un CNAME pour les pages de destination**

Ajoutez le CNAME de page de destination qui vous a été envoyé à votre enregistrement DNS, de sorte que `[YourLandingPageCNAME]` pointe vers la chaîne de compte unique qui est affectée à vos pages de destination Marketo Engage. Connectez-vous au site du registraire de votre domaine et saisissez le CNAME de la page de destination et la chaîne de compte. En règle générale, cela implique trois champs :

* Alias : saisissez `[YourLandingPageCNAME]` (fourni par le marketing).
* Type : CNAME
* Pointer vers : saisissez `[MunchkinID].mktoweb.com` (fourni par le marketing).

`2` **Ajouter un CNAME pour les liens de suivi des e-mails**

Ajoutez le CNAME d’e-mail que le service marketing vous a envoyé, de sorte que `[YourEmailCNAME]` pointe vers [MktoTrackingLink], le lien de suivi par défaut attribué par Marketo Engage, au format suivant :
`[YourEmailCNAME].[YourDomain].com` IN CNAME `[MktoTrackingLink]`.

Par exemple :

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>La valeur `[MktoTrackingLink]` doit être le domaine de branding par défaut.

`3` **Avertir votre équipe marketing**

Avertissez votre équipe marketing une fois ce processus terminé.

`4` **Contactez l’[assistance Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} pour commencer le processus d’approvisionnement d’un certificat SSL.**

Le traitement peut prendre jusqu’à 3 jours ouvrables.

## Étape 2 : placer sur la liste autorisée les adresses IP Marketo Engage {#step-allowlist-marketo-ips}

Lorsque votre groupe marketing utilise Marketo Engage pour envoyer des e-mails de test (bonne pratique avant d’envoyer des e-mails éclairs), les e-mails de test sont parfois bloqués par des systèmes anti-spam qui s’appuient sur les adresses IP de l’expéditeur ou de l’expéditrice pour vérifier que l’e-mail est valide. Pour vous assurer que ces e-mails de test arrivent à destination, ajoutez Marketo Engage sur la liste autorisée.

Ajoutez ces adresses IP à la liste autorisée de votre entreprise :

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Certains systèmes anti-spam utilisent le champ Chemin de retour de l’e-mail au lieu de l’adresse IP pour la mise sur liste autorisée. Dans ce cas, la meilleure approche consiste à utiliser la liste autorisée « &#42;.mktomail.com », car Marketo Engage utilise plusieurs sous-domaines de boîte aux lettres. D’autres systèmes anti-spam placent sur la liste autorisée en fonction de l’adresse d’expédition. Dans ces situations, veillez à inclure tous les domaines d’envoi (« De ») que votre groupe marketing utilise pour communiquer avec les personnes/prospects.

>[!NOTE]
>
>Postini utilise une technologie unique et nécessite de placer sur la liste autorisée des plages d’adresses IP. Consultez [Placer sur la liste autorisée avec Postini](https://nation.marketo.com/docs/DOC-1066).

## Étape 3 : configurer SPF et DKIM {#step-set-up-spf-and-dkim}

Votre équipe marketing doit également fournir les informations DKIM (Domain Keys Identified Mail) à ajouter à votre enregistrement de ressources DNS (également répertorié ci-dessous). Suivez les étapes pour configurer correctement DKIM et SPF (Sender Policy Framework), puis informez votre équipe marketing que cette mise à jour a été effectuée.

1. Pour configurer SPF, ajoutez la ligne suivante aux entrées DNS :

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`
include: mktomail.com ~all

   Si vous avez déjà un enregistrement SPF existant dans l’entrée DNS, ajoutez-y simplement ce qui suit :
include: mktomail.com

   Remplacez CompanyDomain par le domaine principal de votre site web (par exemple, « `(company.com/)` ») et CorpIP par l’adresse IP du serveur de messagerie de votre entreprise (par exemple, « 255.255.255.255 »). Si vous prévoyez d’envoyer des e-mails à partir de plusieurs domaines via Marketo Engage, demandez à votre personnel informatique d’ajouter cette ligne pour chaque domaine (sur une seule ligne).

1. Pour DKIM, créez des enregistrements de ressources DNS pour chaque domaine que vous voulez configurer. Vous trouverez ci-dessous les enregistrements d’hôtes et les valeurs TXT pour chaque domaine soumis à une connexion :

   `[DKIMDomain1]` : l’enregistrement hôte est `[HostRecord1]` et la valeur TXT est `[TXTValue1]`.

   `[DKIMDomain2]` : l’enregistrement hôte est `[HostRecord2]` et la valeur TXT est `[TXTValue2]`.

   Copiez HostRecord et TXTValue pour chaque DKIMDomain que vous avez configuré après avoir suivi les [instructions ici](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. N’oubliez pas de vérifier chaque domaine dans Admin > E-mail > DKIM une fois que votre personnel informatique a terminé cette étape.

## Étape 4 : configurer DMARC {#set-up-dmarc}

DMARC (Domain-based Message Authentication, Reporting &amp; Conformance) est un protocole d’authentification utilisé pour aider les organisations à protéger leur domaine contre une utilisation non autorisée. DMARC étend les protocoles d’authentification existants, tels que SPF et DKIM, pour informer les serveurs de destination des actions à entreprendre en cas d’échec d’authentification sur leur domaine. Bien que le protocole DMARC soit actuellement facultatif, il est vivement recommandé, car il permet de mieux protéger la marque et la réputation de votre entreprise. Les principaux fournisseurs, tels que Google et Yahoo, exigent l’utilisation de DMARC pour les expéditeurs en masse depuis février 2024.

Pour que DMARC fonctionne, vous devez disposer d’au moins l’un des enregistrements TXT DNS suivants :

* Un SPF valide
* Un enregistrement DKIM valide pour votre domaine FROM: (recommandé pour Marketo Engage)

En outre, vous devez disposer d’un enregistrement TXT de DNS spécifique à DMARC pour votre domaine FROM:. Vous pouvez éventuellement définir l’adresse e-mail de votre choix pour indiquer où les rapports DMARC doivent se trouver au sein de votre organisation, afin de pouvoir surveiller les rapports.

Il est recommandé de déployer lentement l’implémentation de DMARC en faisant passer votre politique DMARC par les étapes p=none, p=quarantine, puis p=reject lorsque vous comprenez l’impact potentiel de DMARC. Définissez votre politique DMARC sur un alignement moins strict sur SPF et DKIM.

### Exemple de workflow DMARC {#dmarc-example-workflow}

1. Si votre configuration permet de recevoir des rapports DMARC, vous devez procéder comme suit…

   I. Analysez les commentaires et les rapports que vous recevez et utilisez (p=none), ce qui indique à la personne destinataire de n’effectuer aucune action sur les messages dont l’authentification a échoué, mais d’envoyer tout de même des rapports par e-mail à l’expéditeur ou à l’expéditrice.

   II. Examinez les problèmes liés à SPF/DKIM et corrigez-les si l’authentification de messages légitimes échoue.

   III. Déterminez si SPF ou DKIM sont alignés et réussissent l’authentification pour tous les e-mails légitimes.

   IV. Examinez les rapports pour vous assurer que les résultats sont conformes aux attentes en fonction de vos politiques SPF/DKIM.

1. Ajustez la politique sur (p=quarantine), qui indique au serveur de messagerie de réception de mettre en quarantaine les e-mails dont l’authentification échoue (en plaçant généralement ces messages dans le dossier des spams).

   I. Examinez les rapports pour vous assurer que les résultats sont conformes à vos attentes.

1. Si le comportement des messages au niveau p=quarantine vous convient, vous pouvez ajuster la politique sur (p=reject). La politique p=reject indique à la personne destinataire de refuser complètement (rebond) tout e-mail pour le domaine qui ne réussit pas l’authentification. Lorsque cette politique est activée, seul un e-mail qui est vérifié comme étant authentifié à 100 % par votre domaine aura une chance d’être placé en boîte de réception.

>[!CAUTION]
>
>Utilisez cette politique avec précaution et déterminez si elle est appropriée pour votre organisation.

### Création de rapports DMARC {#dmarc-reporting}

DMARC permet de recevoir des rapports concernant les e-mails qui échouent l’authentification SPF/DKIM. Il existe deux types de rapports générés par les fournisseurs d’accès Internet dans le cadre du processus d’authentification que les expéditeurs et expéditrices peuvent recevoir via les balises RUA/RUF dans leur politique DMARC.

* Rapports agrégés (RUA) : ne contiennent aucune information d’identification personnelle (PII) susceptible d’être sensible au RGPD (Règlement général sur la protection des données).

* Rapports d’analyse (RUF) : contiennent des adresses e-mail sensibles au RGPD. Avant de les utiliser, vérifiez en interne comment traiter les informations qui doivent être conformes au RGPD.

Ces rapports sont principalement utilisés pour recevoir une vue d’ensemble des e-mails faisant l’objet de tentatives d’usurpation. Il s’agit de rapports hautement techniques qui sont mieux gérés par un outil tiers.

### Exemples d’enregistrements DMARC {#example-dmarc-records}

* Enregistrement minimum : `v=DMARC1; p=none`

* Enregistrement redirigé vers une adresse e-mail pour la réception des rapports : `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### Balises DMARC et leurs fonctions {#dmarc-tags-and-what-they-do}

Les enregistrements DMARC comportent plusieurs composants appelés balises DMARC. Chaque balise possède une valeur qui spécifie un certain aspect de DMARC.

<table>
<thead>
  <tr>
    <th>Nom de la balise </th>
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
    <td>Cette balise DMARC spécifie la version. Il n’existe qu’une seule version à ce jour. Sa valeur est donc fixe : v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>Obligatoire</td>
    <td>Montre la politique DMARC sélectionnée, qui ordonne à la personne destinataire de signaler, mettre en quarantaine ou rejeter les e-mails dont les contrôles d’authentification échouent.</td>
    <td>p=none, quarantine ou reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Facultatif</td>
    <td>Permet à la personne propriétaire du domaine de spécifier des options de création de rapports.</td>
    <td>0 : génération du rapport en cas d’échec total
    <br>1 : génération du rapport en cas d’échec d’un élément
    <br>d : génération du rapport en cas d’échec de DKIM
    <br>s : génération du rapport en cas d’échec de SPF</td>
    <td>1 (recommandé pour les rapports DMARC)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>Facultatif</td>
    <td>Indique le pourcentage de messages soumis à un filtrage.</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>Facultatif (recommandé)</td>
    <td>Indique où les rapports agrégés seront diffusés.</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>Facultatif (recommandé)</td>
    <td>Identifie l’endroit où les rapports d’analyse seront diffusés.</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>Facultatif</td>
    <td>Spécifie la politique DMARC pour les sous-domaines du domaine parent.</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>Facultatif</td>
    <td>Peut être strict (s) ou relâché (r). L’alignement relâché signifie que le domaine est utilisé dans la signature DKIM et peut être un sous-domaine de l’adresse « From ». Un alignement strict signifie que le domaine est utilisé dans la signature DKIM et doit correspondre exactement au domaine utilisé dans l’adresse From.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>Facultatif</td>
    <td>Peut être strict (s) ou relâché (r). L’alignement relâché signifie que le domaine ReturnPath peut être un sous-domaine de l’adresse From. L’alignement strict signifie que le domaine Return-Path doit correspondre exactement à l’adresse From.</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

Pour plus d’informations sur DMARC et toutes ses options, consultez le site [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC et Marketo Engage {#dmarc-and-marketo-engage}

Il existe deux types d’alignement pour DMARC : l’alignement DKIM et l’alignement SPF.

>[!NOTE]
>
>Il est recommandé d’effectuer l’alignement de DMARC sur DKIM par rapport à SPF pour Marketo Engage.

* DMARC aligné sur DKIM : pour configurer un protocole DMARC aligné sur DKIM, vous devez effectuer les opérations suivantes :

   * Configurez DKIM pour le domaine FROM: de votre message. Suivez les instructions [dans cet article](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Configurer DMARC pour le domaine FROM:/DKIM configuré précédemment

* SPF aligné sur DMARC : pour configurer un protocole SPF aligné sur DMARC via un chemin de retour de marque, vous devez effectuer les opérations suivantes :

   * Configurer le domaine Return-Path de la marque
      * Configurer l’enregistrement SPF approprié
      * Modifier l’enregistrement MX pour revenir au MX par défaut du centre de données à l’origine de l’envoie de votre courrier

   * Configurer DMARC pour le domaine Return-Path de la marque

* Si vous envoyez des e-mails depuis Marketo Engage via une adresse IP dédiée et que vous n’avez pas encore mis en place de chemin de retour personnalisé, ou si vous n’avez pas la certitude de l’avoir fait, ouvrez un ticket auprès de l’[assistance Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Si vous envoyez des e-mails depuis Marketo Engage par le biais d’un pool partagé d’adresses IP, vous pouvez déterminer si vous remplissez les critères pour les adresses IP de confiance en vous [enregistrant ici](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. Le cjemin de retour de marque est offert gratuitement aux personnes effectuant des envois à partir d’adresses IP de confiance Marketo Engage. Si votre demande est approuvée pour ce programme, contactez l’assistance Adobe pour configurer le chemin de retour de la marque.

   * Adresses IP de confiance : groupe partagé d’adresses IP qui sont réservées aux personnes dont le volume d’envoi est inférieur à 75 000 par mois et qui ne remplissent pas les critères pour une adresse IP dédiée. Ces personnes doivent également répondre aux exigences des bonnes pratiques.

* Si vous envoyez des e-mails à partir de Marketo Engage par le biais d’adresses IP partagées et que vous ne remplissez pas les critères des adresses IP de confiance, mais que vous envoyez plus de 100 000 messages par mois, vous devez contacter l’équipe Adobe en charge des comptes (votre gestionnaire de compte) pour acheter une adresse IP dédiée.

* L’alignement SPF strict n’est pas pris en charge ni recommandé pour Marketo Engage.

## Étape 5 : configurer des enregistrements MX pour votre domaine {#step-set-up-mx-records-for-your-domain}

Un enregistrement MX vous permet de recevoir des e-mails du domaine depuis lequel vous envoyez des e-mails afin de traiter les réponses et les répondeurs automatiques. Si vous effectuez un envoi à partir de votre domaine d’entreprise, il est probable que ce paramètre soit déjà configuré. Si ce n’est pas le cas, vous pouvez généralement le configurer pour qu’il soit mappé à votre enregistrement MX de domaine d’entreprise.

## Adresses IP sortantes {#outbound-ip-addresses}

Une connexion sortante est une connexion établie par Marketo Engage à un serveur sur Internet en votre nom. Certains partenaires/fournisseurs avec lesquels vous travaillez ou votre propre service informatique peuvent utiliser des listes autorisées pour restreindre l’accès aux serveurs. Si tel est le cas, vous devez leur fournir des blocs d’adresses IP sortantes Marketo Engage à ajouter à leurs listes autorisées.

**Webhooks**

Les [webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} de Marketo Engage sont un mécanisme d’intégration sortant. Lorsqu’une action de flux [Appeler le Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} est exécutée dans le cadre d’une campagne intelligente, une requête HTTP est envoyée à un service web externe. Si l’éditeur du service web utilise une liste autorisée sur le pare-feu du réseau sur lequel se trouve le service web externe, il doit ajouter les blocs d’adresses IP répertoriés ci-dessous à leur liste autorisée.

**Synchronisation CRM**

La [synchronisation CRM Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} et la [synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} de Marketo Engage sont des mécanismes d’intégration qui effectuent les requêtes HTTP sortantes vers les API publiées par votre fournisseur CRM. Vous devez vous assurer que votre service informatique ne bloque aucun des blocs d’adresses IP ci-dessous pour accéder aux API de votre fournisseur CRM.

**Blocs d’adresses IP sortantes Marketo Engage**

Les tableaux suivants couvrent tous les serveurs Marketo Engage qui effectuent des appels sortants. Utilisez les listes ci-dessous pour configurer une liste autorisée d’adresses IP, un serveur, un pare-feu, une liste de contrôle d’accès, un groupe de sécurité ou un service tiers afin de recevoir des connexions sortantes de Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Bloc d’adresses IP (notation CIDR)</th>
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
   <th>Adresse IP individuelle</th>
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
