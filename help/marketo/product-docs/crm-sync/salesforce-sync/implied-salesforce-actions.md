---
unique-page-id: 4719304
description: Actions Salesforce appliquées - Documents marketing - Documentation du produit
title: Actions Salesforce appliquées
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---


# Actions Salesforce appliquées {#implied-salesforce-actions}

Lorsqu&#39;une étape de flux spécifique à Salesforce s&#39;exécute, des étapes supplémentaires sont parfois exécutées automatiquement. Voici les règles, donc vous savez :

Ces règles s&#39;appliquent _lorsque la personne n&#39;est pas actuellement dans [Salesforce.com](http://Salesforce.com)_ en tant que contact ou responsable.

<table> 
 <thead> 
  <tr> 
   <th>Etape du flux marketing</th> 
   <th>Action automatique</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ajoute à la norme SFDC Campaign</td> 
   <td>Synchroniser la personne avec SFDC</td> 
  </tr> 
  <tr> 
   <td>Modifier le statut dans SFDC Campaign</td> 
   <td>Synchroniser la personne avec la DDC<br>Ajouter avec la DDC Campaign</td> 
  </tr> 
  <tr> 
   <td>Changer de propriétaire</td> 
   <td><p>Synchroniser la personne avec SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Convertir une personne</td> 
   <td><p>Synchroniser la personne avec SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Créer une Tâche</td> 
   <td>Synchroniser la personne avec SFDC</td> 
  </tr> 
 </tbody> 
</table>

Vous pouvez filtrer les enregistrements SFDC dans une Liste dynamique à l’aide du filtre **Type SFDC** avec l’opérateur défini sur &quot;n’est pas vide&quot;. Tous les enregistrements de la DDC ont une valeur dans ce champ.

N&#39;oubliez pas que ces actions automatiques ne se produisent que si la piste n&#39;est pas actuellement dans [Salesforce.com](https://salesforce.com)
