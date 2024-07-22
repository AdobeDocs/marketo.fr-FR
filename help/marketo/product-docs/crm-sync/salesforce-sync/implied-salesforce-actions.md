---
unique-page-id: 4719304
description: Actions Salesforce appliquées - Documents Marketo - Documentation du produit
title: Actions Salesforce appliquées
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 21%

---

# Actions Salesforce appliquées {#implied-salesforce-actions}

Lorsqu’une étape de flux spécifique à Salesforce s’exécute, des étapes supplémentaires sont parfois automatiquement exécutées. Voici les règles, donc vous savez :

Ces règles s’appliquent lorsque la personne n’est actuellement pas dans [Salesforce.com](https://Salesforce.com){target="_blank"} en tant que contact ou prospect.

<table> 
 <thead> 
  <tr> 
   <th>Étape Flux Marketo</th> 
   <th>Action automatique</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ajouter à la campagne SFDC</td> 
   <td>Synchroniser individu dans SFDC</td> 
  </tr> 
  <tr> 
   <td>Modifier le statut dans une campagne SFDC</td> 
   <td>Synchroniser la personne avec SFDC<br>Ajouter à SFDC Campaign</td> 
  </tr> 
  <tr> 
   <td>Modifier le détenteur</td> 
   <td><p>Synchroniser individu dans SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Convertir individu</td> 
   <td><p>Synchroniser individu dans SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Créer une tâche</td> 
   <td>Synchroniser individu dans SFDC</td> 
  </tr> 
 </tbody> 
</table>

Vous pouvez filtrer les enregistrements SFDC dans une liste dynamique à l’aide du filtre **[!UICONTROL Type SFDC]** avec l’opérateur défini sur &quot;n’est pas vide&quot;. Tous les enregistrements de la DDC ont une valeur dans ce champ.

N’oubliez pas que ces actions automatiques ne se produisent que si le prospect n’est pas actuellement dans [Salesforce.com](https://salesforce.com){target="_blank"}
