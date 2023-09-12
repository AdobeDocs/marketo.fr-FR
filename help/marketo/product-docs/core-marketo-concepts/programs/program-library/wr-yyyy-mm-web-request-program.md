---
description: WR-YYYY-MM-Web Request Program - Marketo Docs - Documentation du produit
title: WR-YYYY-MM-Web Request Program
feature: Programs
source-git-commit: 720215ea958206931413f2d273a4a058bc051579
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 16%

---

# WR-YYYY-MM-Web Request Program {#wr-yyyy-mm-web-request-program}

Il s’agit d’un exemple de programme idéal pour les formulaires de demande de contact, de demande de devis, de demande de démonstration ou de demande d’évaluation utilisant un programme par défaut de Marketo Engage. Peut être utilisé avec les landing pages Marketo ou comme formulaire incorporé sur des landing pages non Marketo. Un message d’alerte est envoyé à une personne spécifique lors de l’envoi du formulaire.

Pour obtenir de l’aide sur la stratégie ou personnaliser un programme, contactez l’équipe Compte d’Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} page.

## Résumé du canal {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Canal</th> 
   <th>État d’appartenance</th>
   <th>Comportement d’analyse</th>
   <th>Type de programme</th>
  </tr> 
  <tr> 
   <td>Demande sur le Web</td> 
   <td>01 - Engagé - Succès</td>
   <td>Inclusif</td>
   <td>Par défaut</td>
  </tr>
 </tbody> 
</table>

## Le programme contient les ressources suivantes {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Type</th> 
   <th>Nom du modèle</th>
   <th>Nom de la ressource</th>
  </tr>
  <tr> 
   <td>Formulaire</td> 
   <td> </td>
   <td>FM-WebRequestForm</td>
  </tr>
  <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle de courrier électronique de démarrage rapide</a></td>
   <td>Alert-WebRequest</td>
  </tr>
  <tr> 
   <td>Page de destination</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Modèle LP de démarrage rapide</a></td>
   <td>01 - LP - Request</td>
  </tr>
  <tr> 
   <td>Page de destination</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Modèle LP de démarrage rapide</a></td>
   <td>02 - LP - ThankYou</td>
  </tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Performance page de destination </td>
  </tr>
   <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>Nouvelle personne à partir d’une requête web</td>
  </tr>
   <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>Nouvelle personne du webinaire</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Ressources : héberge toutes les ressources créatives 
<br/>(sous-dossiers pour les alertes et les pages d’entrée)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Campagnes : héberge toutes les campagnes dynamiques.</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Rapports  </td>
  </tr>
 </tbody> 
</table>

![](assets/wr-yyyy-mm-web-request-program-1.png)

## Mes jetons inclus {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Type de jeton</th> 
   <th>Nom du jeton</th>
   <th>Valeur</th>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Request-Type}}</code></td>
   <td>Nous contacter</td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.ALERT-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.ALERT-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.ALERT-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL?sans le http://</td>
  </tr>
 </tbody> 
</table>

## Règles de conflit {#conflict-rules}

* **Étiquettes du programme**
   * Créer des balises dans cet abonnement - _Recommandé_
   * Ignorer

* **Modèle de page d’entrée du même nom**
   * Copier le modèle d’origine
   * Utiliser le modèle de destination - _Recommandé_

* **Images du même nom**
   * Conserver les deux fichiers
   * Remplacer l’élément de cet abonnement - _Recommandé_

* **Modèles d&#39;email portant le même nom**
   * Conserver les deux modèles
   * Remplacer le modèle existant - _Recommandé_

## Meilleures pratiques {#best-practices}

* Après l’importation du programme de webinaire, déplacez le formulaire d’une ressource locale vers une ressource globale située dans Design Studio.
   * La réduction du nombre de formulaires et l’utilisation de ressources plus globales à partir de Design Studio vous permettent d’accroître l’évolutivité de la conception de votre programme et de la gouvernance administrative. Il offre également une certaine flexibilité pour des mises à jour régulières de conformité pour les champs, la langue d’opt-in, etc.

* Envisagez de mettre à jour les modèles de votre programme importé afin d’utiliser les modèles de marque actuels ou de mettre à jour le modèle nouvellement importé pour refléter votre marque en ajoutant un fragment de code ou vos informations de logo/pied de page appropriées.

* Envisagez de mettre à jour la convention d’affectation des noms de cet exemple de programme pour vous aligner sur votre convention d’affectation des noms.

>[!NOTE]
>
>Pensez à mettre à jour les valeurs de mon jeton dans le modèle de programme et chaque fois que vous utilisez le programme, selon les besoins.

>[!IMPORTANT]
>
>Les jetons qui font référence à une URL ne peuvent pas contenir les caractères http:// ou https:// ; dans le cas contraire, le lien ne fonctionnera pas correctement dans la ressource.
