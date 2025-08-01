---
description: Liste de contrôle de la base de données d’instance héritée - Documents Marketo - Documentation du produit
title: Liste de contrôle de la base de données de l'instance héritée
feature: Getting Started
exl-id: 278a6a2f-7b68-4003-8727-129e0dc96c12
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 7%

---

# Instance héritée : liste de contrôle de la base de données {#inherited-instance-database-checklist}

Comprenez le nombre total de personnes, de personnes commercialisables et de sources qui achètent le plus dans votre abonnement. N’oubliez pas de [télécharger les listes de contrôle](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) et de suivre vos progrès.

## Listes intelligentes du système {#system-smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Toutes les personnes</td>
   <td><li>Combien de personnes existent dans la <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">base de données</a> ?</li>
<li>Si votre base de données est presque pleine, votre politique d’entreprise recommande-t-elle d’étendre la taille de votre base de données ou de nettoyer les données historiques ?</li>
<li>Votre base de données globale est-elle commercialisable à au moins 85 % ?
<br/>     Placer sur la liste bloquée Si la vôtre est inférieure à ce seuil, examinez les autres listes intelligentes système (, Marketing Suspendu, Dupliqués, Désabonnement) avec une plus grande attention.</li></td>
  </tr>
  <tr>
   <td>Personnes désinscrites</td>
   <td><li>Quels sont vos critères pour les <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">personnes désabonnées</a> ? Y a-t-il trop de personnes désabonnées ?</li>
<li>Vos méthodes de désabonnement sont-elles conformes à vos exigences en matière de confidentialité des données ?</li>
<li>Votre préférence de désabonnement est-elle à jour ? Depuis combien de temps les enregistrements sont-ils restés dans votre base de données comme non commercialisables ?</li></td>
  </tr>
  <tr>
   <td>Marketing interrompu</td>
   <td><li>Quels sont vos critères pour <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">Marketing suspendu</a> ? Y a-t-il trop de personnes dont le marketing est suspendu ?</li>
<li>Depuis combien de temps les enregistrements ont-ils le statut Marketing suspendu ?</li>
<p>Exemple de cas d’utilisation de marketing suspendu : des personnes qui sont impliquées activement dans des ventes à un stade avancé des opportunités pour lesquelles vous souhaitez supprimer les communications marketing.</td>
  </tr>
   <tr>
   <td>Liste de blocage</td>
   <td><li>Placer sur la liste bloquée Quels sont vos critères pour les enregistrements <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank"></a> ? Placer sur la liste bloquée Y a-t-il trop de gens qui sont traités?</li></td>
  </tr>
  <tr>
   <td>Adresses e-mail renvoyées</td>
   <td><li>Y a-t-il beaucoup de <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">personnes ayant rebondi</a> dans votre base de données ?
   <br/>     Si oui, envisagez d’en rechercher la raison.</li></td></li></td>
  </tr>
  <tr>
   <td>Doublons possibles</td>
   <td><li>Combien y a-t-il d’enregistrements <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">potentiellement en double</a> ?
   <br/>     Envisagez de les supprimer ou de les fusionner.</li></td>
  </tr>
   <tr>
   <td>Pas de programme d'acquisition</td>
   <td><li>Combien de personnes n'ont pas de <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">programme d'acquisition</a>?
   <br/>     S’il y en a beaucoup, envisagez d’en examiner la raison.</li></td>
  </tr>
 </tbody>
</table>

## Listes intelligentes {#smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Listes intelligentes</td>
   <td><li>Combien y a-t-il de <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">listes intelligentes</a> ? Comment sont-ils utilisés dans ce cas ?</li>
   <p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : dans la section Base de données, les listes dynamiques de groupe sont générées par l'utilisateur et les listes dynamiques système sont des listes créées par défaut par Marketo Engage.
<li>Les listes sont-elles organisées dans une structure de dossiers cohérente ?
<br/>     Si vous disposez de listes orphelines, pensez à organiser votre arborescence afin que les ressources soient faciles à trouver.</li>
<p><img src="assets/tip-icon.png" alt="icône d’astuce">CONSEIL : l’<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">archivage</a> les listes dynamiques devenues inutiles facilitent l’organisation et améliorent les performances.</td>
  </tr>
 </tbody>
</table>

## Listes statiques {#static-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Listes statiques</td>
   <td><li>Combien y a-t-il de <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">listes statiques</a> ? Comment sont-ils utilisés dans ce cas ?</li>
   <p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : dans la section Base de données, les listes de groupes sont des listes statiques.</td>
  </tr>
 </tbody>
</table>

## Segmentations {#segmentations}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Zone</th>
   <th>Vérifier le focus</th>
  </tr>
  <tr>
   <td>Segmentations</td>
   <td><li>Quelles <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">segmentations</a> y a-t-il ? Comment sont-ils utilisés ?</li>
<li>Y a-t-il trop de personnes dans les <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">segments par défaut</a> ?</li>
<li>Existe-t-il une segmentation pour l’audience commercialisable ?
<br/>     Sinon, envisagez d’en créer un.</li></td>
  </tr>
 </tbody>
</table>
