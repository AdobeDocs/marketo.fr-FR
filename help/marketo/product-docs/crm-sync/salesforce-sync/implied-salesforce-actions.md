---
unique-page-id: 4719304
description: Actions Salesforce implicites - Documentation de Marketo - Documentation du produit
title: Actions Salesforce implicites
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 21%

---

# Actions Salesforce implicites {#implied-salesforce-actions}

Lorsqu’une étape de flux spécifique à [!DNL Salesforce] s’exécute, des étapes supplémentaires sont parfois exécutées automatiquement. Voici les règles, donc vous savez :

Ces règles s&#39;appliquent lorsque la personne n&#39;est pas actuellement dans [Salesforce.com](https://Salesforce.com){target="_blank"} en tant que contact ou prospect.

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
   <td>Synchroniser la personne avec SFDC<br>Add à SFDC Campaign</td> 
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

Vous pouvez filtrer les enregistrements SFDC dans une liste dynamique à l’aide du filtre **[!UICONTROL Type de SFDC]** avec l’opérateur défini sur « [!UICONTROL &#x200B; n’est pas vide »]. Tous les enregistrements SFDC ont une valeur dans ce champ.

N&#39;oubliez pas que ces actions automatiques ne se produisent que si le prospect n&#39;est pas actuellement dans [Salesforce.com](https://salesforce.com){target="_blank"}
