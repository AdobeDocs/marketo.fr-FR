---
description: Liste de contrôle de la base de données des instances héritées - Documents Marketo - Documentation du produit
title: Liste de contrôle de la base de données des instances héritées
feature: Getting Started
exl-id: 278a6a2f-7b68-4003-8727-129e0dc96c12
source-git-commit: 2c74c71c9311312f7e0991ed5598ccb09a9b1f15
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 7%

---

# Instance héritée : liste de contrôle de base de données {#inherited-instance-database-checklist}

Comprenez le nombre total de personnes, de personnes pouvant faire l’objet d’un marketing et de sources d’acquisition par les principales personnes dans votre abonnement. N’oubliez pas de [télécharger les listes de contrôle](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) et suivez vos progrès.

## Listes intelligentes du système {#system-smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th> 
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Toutes les personnes</td> 
   <td><li>Le nombre de personnes dans la variable <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">base</a>?</li>
<li>Si votre base de données est presque pleine, la politique de votre société vous recommande-t-elle d’augmenter la taille de votre base de données ou de nettoyer les données historiques ?</li>
<li>Votre base de données globale est-elle commercialisable à au moins 85 % ? 
<br/>     Si le vôtre tombe sous ce seuil, consultez les autres listes intelligentes du système (Liste bloquée, Marketing suspendu, Doublons, Désabonner) avec une plus grande attention.</li></td>
  </tr>
  <tr> 
   <td>Personnes désinscrites</td> 
   <td><li>Quels sont vos critères pour <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">personnes désabonnées</a>? Y a-t-il trop de personnes désinscrites ?</li>
<li>Vos méthodes de désabonnement sont-elles conformes à vos exigences en matière de confidentialité des données ?</li>
<li>Votre préférence de désabonnement est-elle à jour ? Combien de temps les enregistrements sont-ils restés dans votre base de données comme non commercialisables ?</li></td>
  </tr>
  <tr> 
   <td>Marketing interrompu</td> 
   <td><li>Quels sont vos critères pour <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">Marketing suspendu</a>? Trop de personnes sont-elles suspendues dans le marketing ?</li>
<li>Combien de temps les enregistrements sont-ils restés dans l’état Marketing suspendu ?</li>
<p>Exemple de cas d’utilisation Marketing suspendu : enregistrements de personnes qui sont activement impliquées dans les ventes à des stade avancé pour lesquels vous souhaitez supprimer les communications marketing.</td>
  </tr>
   <tr> 
   <td>Liste de blocage</td> 
   <td><li>Quels sont vos critères pour <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">placer sur la liste bloquée des enregistrements</a>? Y a-t-il trop de gens qui sont placés sur la liste bloquée ?</li></td>
  </tr>
  <tr> 
   <td>Adresses e-mail renvoyées</td> 
   <td><li>As-tu beaucoup de choses ? <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">personnes ayant fait un bounce</a> dans votre base de données ?
   <br/>     Si c'est le cas, envisagez d'examiner pourquoi.</li></td></li></td>
  </tr>
  <tr> 
   <td>Doublons possibles</td> 
   <td><li>Combien <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">enregistrement potentiellement en double</a> y en a-t-il ?
   <br/>     Envisagez de les supprimer ou de les fusionner.</li></td>
  </tr>
   <tr> 
   <td>Pas de programme d'acquisition</td> 
   <td><li>Combien de personnes n’ont pas de <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">programme d'acquisition</a>?
   <br/>     S'il y a beaucoup de choses, réfléchissez à pourquoi.</li></td>
  </tr>
 </tbody> 
</table>

## Listes intelligentes {#smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th> 
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Listes intelligentes</td> 
   <td><li>Combien <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">Listes dynamiques</a> y en a-t-il ? Comment sont-ils utilisés dans cette instance ?</li>
   <p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : dans la section Base de données , les listes dynamiques de groupe sont générées par l’utilisateur et les listes dynamiques système sont des listes par défaut créées par Marketo Engage.
<li>Les listes sont-elles organisées dans une structure de dossiers cohérente ? 
<br/>     Si vous disposez de listes orphelines, envisagez d’organiser votre arborescence afin que les ressources soient faciles à trouver.</li>
<p><img src="assets/tip-icon.png" alt="icône de bulle">CONSEIL : <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">Archivage</a> Les listes intelligentes qui ne sont plus nécessaires aideront à l’organisation et aux performances.</td>
  </tr>
 </tbody> 
</table>

## Listes statiques {#static-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th> 
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Listes statiques</td> 
   <td><li>Combien <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">Listes statiques</a> y en a-t-il ? Comment sont-ils utilisés dans cette instance ?</li>
   <p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : dans la section Base de données, les listes de groupes sont des listes statiques.</td>
  </tr>
 </tbody> 
</table>

## Segmentations {#segmentations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Zone</th> 
   <th>Objectif de la révision</th>
  </tr> 
  <tr> 
   <td>Segmentations</td> 
   <td><li>Quel <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">segmentation</a> y en a-t-il ? Comment sont-ils utilisés ?</li>
<li>Trop de personnes dans <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">segments par défaut</a>?</li>
<li>Existe-t-il une segmentation pour l’audience vendable ? 
<br/>     Si ce n'est pas le cas, envisagez d'en créer un.</li></td>
  </tr>
 </tbody> 
</table>
