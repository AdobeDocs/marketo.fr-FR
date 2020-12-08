---
unique-page-id: 4719304
description: Actions Salesforce appliquées - Documents marketing - Documentation du produit
title: Actions Salesforce appliquées
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Actions Salesforce appliquées {#implied-salesforce-actions}

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Lorsqu&#39;une étape de flux spécifique à Salesforce s&#39;exécute, des étapes supplémentaires sont parfois exécutées automatiquement. Voici les règles, donc vous savez :

Ces règles s&#39;appliquent *lorsque la personne n&#39;est pas actuellement dans [Salesforce.com](http://Salesforce.com)* en tant que contact ou responsable.

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
   <td>Synchroniser la personne avec<br>SFDCAdd avec SFDC Campaign</td> 
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

Vous pouvez filtrer les enregistrements SFDC dans une Liste dynamique à l’aide du filtre de type **** SFDC avec l’opérateur défini sur &quot;n’est pas vide&quot;. Tous les enregistrements de la DDC ont une valeur dans ce champ.

N&#39;oubliez pas que ces actions automatiques ne se produisent que si le prospect n&#39;est pas actuellement dans [Salesforce.com.](http://Salesforce.com)

La synchronisation Salesforce est cool, non ?
