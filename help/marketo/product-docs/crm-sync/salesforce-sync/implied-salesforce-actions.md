---
unique-page-id: 4719304
description: Actions Salesforce appliquées - Documents Marketo - Documentation du produit
title: Actions Salesforce appliquées
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 21%

---

# Actions Salesforce appliquées {#implied-salesforce-actions}

Lorsqu&#39;une étape de flux spécifique à Salesforce s&#39;exécute, des étapes supplémentaires sont parfois exécutées automatiquement. Voici les règles, donc vous savez :

Ces règles s&#39;appliquent _lorsque la personne n&#39;est pas actuellement dans [Salesforce.com](https://Salesforce.com)_ en tant que contact ou responsable.

<table> 
 <thead> 
  <tr> 
   <th>Étape de flux Marketo</th> 
   <th>Action automatique</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ajouter à la campagne SFDC</td> 
   <td>Synchroniser individu dans SFDC</td> 
  </tr> 
  <tr> 
   <td>Modifier statut dans une campagne SFDC</td> 
   <td>Synchroniser la personne avec la DDC<br>Ajouter avec la DDC Campaign</td> 
  </tr> 
  <tr> 
   <td>Modifier détenteur</td> 
   <td><p>Synchroniser individu dans SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Convertir l’individu</td> 
   <td><p>Synchroniser individu dans SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Créer tâche</td> 
   <td>Synchroniser individu dans SFDC</td> 
  </tr> 
 </tbody> 
</table>

Vous pouvez filtrer les enregistrements SFDC dans une Liste dynamique à l’aide du filtre **Type SFDC** avec l’opérateur défini sur &quot;n’est pas vide&quot;. Tous les enregistrements de la DDC ont une valeur dans ce champ.

N&#39;oubliez pas que ces actions automatiques ne se produisent que si la piste n&#39;est pas actuellement dans [Salesforce.com](https://salesforce.com)
