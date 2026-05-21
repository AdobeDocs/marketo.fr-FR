---
unique-page-id: 4719304
description: Identifiez les étapes de flux Salesforce qui déclenchent une synchronisation automatique de la personne vers SFDC ou d’autres actions. Découvrez les règles relatives à Ajouter à Campaign, Modifier le propriétaire, Créer une tâche et Convertir une personne.
title: Actions Salesforce implicites
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/lI3sRqk1if-UZ7DARSrGXXM485ZjZnlqDGb4si2wvi0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 163
ht-degree: 22%

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
   <td>Synchroniser une personne dans SFDC</td>
  </tr>
  <tr>
   <td>Modifier le statut dans une campagne SFDC</td>
   <td>Synchroniser la personne avec <br>Add à SFDC Campaign</td>
  </tr>
  <tr>
   <td>Modifier l’entité propriétaire</td>
   <td><p>Synchroniser une personne dans SFDC</p></td>
  </tr>
  <tr>
   <td>Convertir une personne</td>
   <td><p>Synchroniser une personne dans SFDC</p></td>
  </tr>
  <tr>
   <td>Créer une tâche</td>
   <td>Synchroniser une personne dans SFDC</td>
  </tr>
 </tbody>
</table>

Vous pouvez filtrer les enregistrements SFDC dans une liste dynamique à l’aide du filtre **[!UICONTROL Type de SFDC]** avec l’opérateur défini sur « [!UICONTROL  n’est pas vide »]. Tous les enregistrements SFDC ont une valeur dans ce champ.

N&#39;oubliez pas que ces actions automatiques ne se produisent que si le prospect n&#39;est pas actuellement dans [Salesforce.com](https://salesforce.com){target="_blank"}
