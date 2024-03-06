---
description: Configuration de la section Base de données pour une nouvelle instance de Marketo Engage.
title: NOUVELLE BASE DE DONNÉES DE ZONES
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 3cb7e5ddef8ec05a7cf8d65dd9f3bafa5dcb7da1
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 13%

---

# NOUVELLE ZONE : Liste de contrôle de la base de données {#new-area-database-checklist}

Découvrez comment mettre en oeuvre les étapes nécessaires pour la section Base de données dans votre nouvelle instance de Marketo Engage. Suivez les guides &quot;Mise en oeuvre d’une nouvelle instance&quot; et effectuez le suivi des tâches en cours afin de vous aider à configurer votre instance pour une efficacité à long terme.

## Listes intelligentes du système {#system-smart-lists}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Toutes les personnes</td>
    <td><li>Déterminez l’implémentation d’une synchronisation 1:1 avec la gestion de la relation client ou l’application de filtres pour limiter qui passe d’un système à l’autre et quand.</li> 
    <li>Vérifiez le nombre total de personnes et de personnes pouvant faire l’objet d’un marketing dans votre <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html" target="_blank" rel="noopener noreferrer">base</a>.</li></td>
    <td>Texte</td>
  </tr>
  <tr>
    <td>Liste de blocage</td>
    <td><li>Définissez des critères de liste bloquée. Envisagez d’ajouter les domaines d’un concurrent à <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank" rel="noopener noreferrer">liste bloquée</a> pour les empêcher de recevoir des emails marketing et opérationnels.</li></td>
    <td>Texte</td>
  </tr>
  <tr>
    <td>Suspension du marketing</td>
    <td><li>Définir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html#marketing-suspended" target="_blank" rel="noopener noreferrer">Marketing suspendu</a> critères.</li></td>
    <td>Texte</td>
  </tr>
  <tr>
    <td>Adresses e-mail renvoyées </td>
    <td><li>Définissez vos critères pour les adresses électroniques rejetées.</li>
    <li>Vérifiez les personnes dans la catégorie Email non valide et si leurs emails doivent être <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank" rel="noopener noreferrer">réinitialiser manuellement</a>.</li></td>
    <td>Texte</td>
  </tr>
  <tr>
    <td>Doublons possibles</td>
    <td><li>Vérifiez les personnes dans la liste Doublons possibles .</li> 
    <li>Définissez votre stratégie de gestion des doublons pour déterminer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank" rel="noopener noreferrer">fusion manuelle des personnes</a> ou pas.</li>  
    <li>Si vous disposez d’une intégration CRM, vous devez définir un processus et un compte pour <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html#effect-in-salesforce" target="_blank" rel="noopener noreferrer">effet de la fusion des pistes dans le CRM</a>.</li></td>
    <td>Texte</td>
  </tr>
  <tr>
    <td>Hormis programme d’acquisition</td>
    <td><li>Créez des campagnes dans vos modèles de programme qui définissent le programme d’acquisition, en particulier si vous utilisez des formulaires globaux.</li></td>
    <td>Texte</td>
  </tr>
  <tr>
    <td>Personnes désabonnées</td>
    <td><li>Vérifiez vos critères pour <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html" target="_blank" rel="noopener noreferrer">Désabonnement des personnes</a>.</li></td>
    <td>Texte</td>
  </tr>
</tbody>
</table>

## Listes de groupes intelligentes {#group-smart-lists}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Listes de groupes intelligentes</td>
    <td><li>N’oubliez pas de créer des listes dynamiques de groupe afin qu’il n’y ait pas de listes en double.</li>
    <li>Effectuez le suivi des listes maîtres ici dans la base de données.</li></td>
    <td>Texte</td>
  </tr>
</tbody>
</table>

## Segmentation {#segmentation}

<table>
<thead>
  <tr>
    <th>Zone</th>
    <th>Éléments d’action</th>
    <th>Priorité</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentation</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html" target="_blank" rel="noopener noreferrer">Création de segments</a> en fonction des besoins de votre entreprise. Chaque abonnement est limité à 20 segments et 100 segments pour chaque segmentation.</li></td>
    <td>Texte</td>
  </tr>
</tbody>
</table>
