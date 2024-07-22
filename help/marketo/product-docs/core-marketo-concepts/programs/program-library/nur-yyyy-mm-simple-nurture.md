---
description: NUR-AAAA-MM-Simple Nurture - Documents Marketo - Documentation du produit
title: NUR-AAAA-MM-Simple Nurture
feature: Programs
exl-id: aed11d75-3190-46ea-8b0b-c1494645901d
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 15%

---

# NUR-AAAA-MM-Simple Nurture {#nur-yyyy-mm-simple-nurture}

Il s’agit d’un exemple de programme d’aide à la retraite simple, qui utilise le programme d’engagement des Marketo Engage, avec du contenu cadencé pour passer au fil du temps dans votre base de données, tout en utilisant des flux pour guider les enregistrements à travers les parcours en fonction du comportement.

Pour obtenir de l’aide sur la stratégie ou personnaliser un programme, contactez l’équipe chargée du compte Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} .

## Résumé du canal {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Canal</th> 
   <th>État d’appartenance</th>
   <th>Comportement d'analyse</th>
   <th>Type de programme</th>
  </tr> 
  <tr> 
   <td>Nurture</td> 
   <td>01 - Membre 
<br/>02 - Engagé - Succès</td>
   <td>Inclusif</td>
   <td>Engagement</td>
  </tr>
 </tbody> 
</table>

## Le programme contient l’Assets suivante {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Type</th> 
   <th>Nom du modèle</th>
   <th>Nom de la ressource</th>
  </tr> 
  <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle de courrier électronique de démarrage rapide</a></td>
   <td>01 - Email</td>
  </tr>
   <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle de courrier électronique de démarrage rapide</a></td>
   <td>02 - Email</td>
  </tr>
   <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle de courrier électronique de démarrage rapide</a></td>
   <td>03 - Email</td>
  </tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Performance des e-mails</td>
  </tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Performance du stream d'engagement</td>
  </tr>
  <tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>01 - Ajouter à l’éducation</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>02 - Infirmière en pause</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>03 - Reprise de la formation</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>04 - Engagé (succès du programme)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Assets : héberge toutes les ressources créatives
   <br/>(sous-dossiers pour les emails)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Campagnes : héberge toutes les campagnes dynamiques.</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Rapports</td>
  </tr>
 </tbody> 
</table>

![](assets/nur-yyyy-mm-simple-nurture-1.png)

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
   <td><code>{{my.Email-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Email-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
 </tbody> 
</table>

## Règles de conflit {#conflict-rules}

* **Balises de programme**
   * Créer des balises dans cet abonnement - _Recommandé_
   * Ignorer

* **Modèle de page d’entrée avec le même nom**
   * Copier le modèle d&#39;origine
   * Utiliser le modèle de destination - _Recommandé_

* **Images du même nom**
   * Conserver les deux fichiers
   * Remplacer un élément de cet abonnement - _Recommandé_

* **Modèles d&#39;email portant le même nom**
   * Conserver les deux modèles
   * Remplacer le modèle existant - _Recommandé_

## Meilleures pratiques {#best-practices}

* Envisagez de mettre à jour les modèles de votre programme importé afin d’utiliser les modèles de marque actuels ou de mettre à jour le modèle nouvellement importé pour refléter votre marque en ajoutant un fragment de code ou vos informations de logo/pied de page appropriées.

* Envisagez de mettre à jour la convention d’affectation des noms de cet exemple de programme pour vous aligner sur votre convention d’affectation des noms.

* Assurez-vous que des règles sont en place pour mettre en pause et reprendre votre cadence de formation. Ces campagnes dynamiques doivent être activées ou planifiées avant l’activation du programme d’engagement.

>[!NOTE]
>
>Pensez à mettre à jour les valeurs de mon jeton dans le modèle de programme et chaque fois que vous utilisez le programme, selon les besoins.

>[!TIP]
>
>N’oubliez pas d’activer la campagne &quot;04 - Engaged (Program Success)&quot; pour le suivi du succès. Effectuez cette _avant_ l&#39;envoi de vos emails.
