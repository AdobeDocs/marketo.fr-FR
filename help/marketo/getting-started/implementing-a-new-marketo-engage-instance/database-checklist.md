---
description: Configurez la section Base de données pour votre nouvelle instance de Marketo Engage.
title: Bonnes pratiques relatives aux nouvelles instances - Liste de contrôle des bases de données
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
source-git-commit: df8087dbaf2b621d0d877eba1c16f160ee9bf460
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 9%

---

# Bonnes pratiques relatives aux nouvelles instances : liste de contrôle de la base de données {#new-instance-best-practices-database-checklist}

La section Base de données vous permet de trouver les attributs clés des personnes de votre instance. En savoir plus sur les étapes nécessaires pour parcourir différentes listes et segments dans votre base de données, ainsi que sur la gestion des enregistrements de personnes.

Pensez à [télécharger les listes de contrôle](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) et suivre votre progression.

## Listes intelligentes du système {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Toutes les personnes</td>
    <td><li>Déterminez l’implémentation d’une synchronisation 1:1 avec votre CRM ou l’application de filtres pour limiter qui passe d’un système à l’autre et quand.</li> 
    <li>Vérifiez le nombre total de personnes et de personnes pouvant faire l’objet d’un marketing dans votre <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html?lang=fr" target="_blank">base de données de Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Liste de blocage</td>
    <td><li>Définissez des critères de liste bloquée. Envisagez d’ajouter les domaines d’un concurrent à votre <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html?lang=fr" target="_blank">liste bloquée</a> afin de l’empêcher de recevoir vos emails.</li></td>
  </tr>
  <tr>
    <td>Marketing interrompu</td>
    <td><li>Définissez les critères <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">Marketing suspendu</a> .</li></td>
  </tr>
  <tr>
    <td>Adresses e-mail renvoyées </td>
    <td><li>Définissez vos critères pour les adresses électroniques rebonds.</li>
    <li>Passez en revue les personnes de la catégorie "Email non valide" et déterminez si leurs emails doivent être <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html?lang=fr" target="_blank">réinitialisés manuellement</a>.</li></td>
  </tr>
  <tr>
    <td>Doublons possibles</td>
    <td><li>Vérifiez les personnes dans la liste Doublons possibles .</li> 
    <li>Définissez votre stratégie de gestion des doublons pour déterminer si vous souhaitez <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=fr" target="_blank">fusionner les personnes manuellement</a>.</li>  
    <li>Si vous disposez d'une intégration CRM, définissez un processus et un compte pour <a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">l'effet de la fusion de pistes dans votre CRM</a>.</li></td>
  </tr>
  <tr>
    <td>Pas de programme d'acquisition</td>
    <td><li>Créez des campagnes dans vos modèles de programme qui définissent un programme d’acquisition, en particulier si vous utilisez des formulaires globaux.</li></td>
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
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Listes intelligentes du groupe</td>
    <td><li>N’oubliez pas de créer des listes dynamiques de groupe afin qu’il n’y ait pas de listes en double.</li>
    <li>Effectuez le suivi des listes maîtres dans la base de données.</li></td>
  </tr>
</tbody>
</table>

## Segmentation {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:21%">Zone</th>
    <th style="width:79%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentation</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html?lang=fr" target="_blank">Créez des segments</a> en fonction des besoins de votre entreprise. Chaque abonnement est limité à 20 segments et 100 segments pour chaque segmentation.</li></td>
  </tr>
</tbody>
</table>
