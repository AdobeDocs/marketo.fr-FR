---
description: AEM-AAAA-MM-JJ-Envoi de courrier électronique unique - Documents Marketo - Documentation du produit
title: AEM-AAAA-MM-JJ-Envoi de courrier électronique unique
feature: Programs
exl-id: 58782d4c-658b-42cd-9ca3-fa53c7476e48
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 16%

---

# AEM-AAAA-MM-JJ-Envoi de courrier électronique unique {#em-yyyy-mm-dd-single-email-send}

Cet exemple envoie un seul courrier électronique à l’aide d’un programme de courrier électronique de Marketo Engage. Le courrier électronique peut inclure ou non un test A/B.

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
   <td>E-mail</td> 
   <td>01-Member 
<br/>02-Engaged-Success</td>
   <td>Inclusif</td>
   <td>E-mail</td>
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
   <td>01-Email-Thank You</td>
  </tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Performance des e-mails</td>
  </tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Performance du lien par e-mail</td>
  </tr>
  <tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>01-Engagé (succès du programme)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Assets : héberge toutes les ressources créatives 
<br/> (sous-dossiers pour les pages d’entrée et de messagerie)  </td>
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

![](assets/em-yyyy-mm-dd-single-email-send-1.png)

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

>[!NOTE]
>
>Pensez à mettre à jour les valeurs de mon jeton dans le modèle de programme et chaque fois que vous utilisez le programme, selon les besoins.

>[!TIP]
>
>N’oubliez pas d’activer la campagne &quot;01-Engaged&quot; (engagement 01) pour suivre les performances ! Effectuez cette opération _avant_ que votre formulaire soit actif et que les courriers électroniques soient envoyés.
