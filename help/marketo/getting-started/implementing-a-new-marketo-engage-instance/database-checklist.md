---
description: Configurez la section Base de données pour votre nouvelle instance Marketo Engage.
title: Bonnes pratiques relatives aux nouvelles instances - Liste de contrôle de la base de données
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 9%

---

# Bonnes Pratiques Relatives Aux Nouvelles Instances : Liste De Contrôle De Base De Données {#new-instance-best-practices-database-checklist}

Dans la section Base de données, vous trouverez les attributs clés des personnes de votre instance. Découvrez les étapes nécessaires pour parcourir les différentes listes et segmentations de votre base de données, ainsi que pour gérer les enregistrements de personnes.

N’oubliez pas de [télécharger les listes de contrôle](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) et de suivre vos progrès.

## Listes intelligentes du système {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Toutes les personnes</td>
    <td><li>Déterminez la mise en œuvre d’une synchronisation 1:1 avec votre CRM ou l’application de filtres pour limiter les personnes qui passent d’un système à un autre et quand.</li>
    <li>Vérifiez le nombre total de personnes et de personnes commercialisables dans votre base de données <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html?lang=fr" target="_blank">Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Liste de blocage</td>
    <td><li>Définissez des critères de place sur la liste bloquée. Envisagez d'ajouter les domaines de vos concurrents à votre <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html?lang=fr" target="_blank">liste bloquée </a> pour les empêcher de recevoir l'un de vos e-mails.</li></td>
  </tr>
  <tr>
    <td>Marketing interrompu</td>
    <td><li>Définissez les critères <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">Marketing suspendu</a>.</li></td>
  </tr>
  <tr>
    <td>Adresses e-mail renvoyées </td>
    <td><li>Définissez vos critères pour les adresses e-mail de rebond.</li>
    <li>Vérifiez les personnes de la catégorie « E-mail non valide » et déterminez si leurs e-mails doivent être <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html?lang=fr" target="_blank">réinitialisés manuellement</a>.</li></td>
  </tr>
  <tr>
    <td>Doublons possibles</td>
    <td><li>Vérifier les personnes dans la liste des doublons possibles.</li>
    <li>Définissez votre stratégie de gestion des doublons afin de déterminer si vous souhaitez <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=fr" target="_blank">fusionner les personnes manuellement</a>.</li>
    <li>Si vous disposez d’une intégration CRM, définissez un processus et un compte pour <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">l’effet de la fusion des prospects dans votre CRM</a>.</li></td>
  </tr>
  <tr>
    <td>Pas de programme d'acquisition</td>
    <td><li>Établissez des campagnes dans vos modèles de programme qui définissent un programme d’acquisition, en particulier si vous utilisez des formulaires globaux.</li></td>
  </tr>
  <tr>
    <td>Personnes désinscrites</td>
    <td><li>Vérifiez vos critères pour <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=fr" target="_blank">Personnes désabonnées</a>.</li></td>
  </tr>
</tbody>
</table>

## Listes intelligentes du groupe {#group-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Listes intelligentes du groupe</td>
    <td><li>Veillez à créer des listes dynamiques de groupe afin d’éviter les doublons.</li>
    <li>Suivre les listes principales dans la base de données.</li></td>
  </tr>
</tbody>
</table>

## Segmentation {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:21%">Zone</th>
    <th style="width:79%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentation</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html?lang=fr" target="_blank">Créez des segmentations</a> en fonction des besoins de votre entreprise. Chaque abonnement est limité à 20 segmentations et 100 segments dans chaque segmentation.</li></td>
  </tr>
</tbody>
</table>
