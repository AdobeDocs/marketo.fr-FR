---
description: Documentez la configuration de votre nouvelle instance de Marketo Engage.
title: Bonnes pratiques relatives aux nouvelles instances - Document de votre configuration
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
source-git-commit: 3004885d1b6b986eb30072d2f67c5bd29ad251c7
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 2%

---

# Bonnes pratiques relatives à la nouvelle instance : documenter votre configuration {#new-instance-best-practices-document-your-setup}

Maintenant que vous avez appris les principales zones de produit à configurer pour une nouvelle instance de Marketo Engage, l’étape suivante consiste à créer la documentation pour la configuration de votre instance et la pile technique. Que vous le créiez au moyen d’une feuille de calcul ou d’une application de gestion de projet, votre documentation sera une excellente ressource pour suivre l’avancement et enregistrer les détails, ainsi que pour préserver la structure et la durabilité de votre instance pour les futurs marketeurs de votre entreprise.

## Données {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Importer une liste</td>
    <td><li>Collecte d’une liste de sources de données dont les enregistrements seront extraits de vers <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started-with-marketo/quick-wins/import-a-list-of-people" target="_blank">import dans Marketo Engage</a>.</li>
    <li>Si vous importez depuis plusieurs sources de données, pensez à utiliser des listes de Principal ou <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">création d’un champ personnalisé</a> sur l’enregistrement de la personne pour indiquer la source de données.</li></td>
  </tr>
  <tr>
    <td>Intégration de base de données</td>
    <td><li>Si vous utilisez la synchronisation native entre Marketo Engage et votre CRM, réfléchissez attentivement aux champs que vous souhaitez synchroniser entre les systèmes. Tous les champs n’ont pas besoin d’être synchronisés. Soyez donc stratégique quant à vos flux de données.</li></td>
  </tr>
</tbody>
</table>

## Documentation {#documentation}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments d’action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Utilisateurs et utilisatrices</td>
    <td><li>Document <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">utilisateurs actuels</a> dans votre instance pour des raisons de sécurité. Les détails suivants doivent être inclus au minimum (et sont tous visibles en accédant à Adobe Admin Console &gt; Utilisateurs) :</li>
    <br>Nom
    <br>Email
    <br>Type d’ID
    <br>Profil(s) de produit
    <p>
    <li>En tant qu’administrateur de produit Marketo Engage, développez un processus interne pour contrôler et mettre à jour la liste des utilisateurs Marketo Engage à une cadence normale. Pour apporter des modifications à la liste des utilisateurs dans Adobe Admin Console, envisagez <a href="https://helpx.adobe.com/fr/enterprise/using/users.html" target="_blank">actions en bloc</a>, comme charger un fichier .CSV, à l’aide de l’API REST User Management, etc.</li></td>
  </tr>
  <tr>
    <td>Entreprise</td>
    <td><li>Documentez la structure de dossiers convenue, les conventions d’attribution de noms standard pour les programmes, les ressources, etc., et les raisons pour lesquelles les décisions ont été prises. <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">Découvrez les bonnes pratiques ici.</a></li></td>
  </tr>
  <tr>
    <td>Changelog</td>
    <td><li>Créez un fichier de modification dans lequel vous pouvez documenter les modifications apportées à votre instance et les raisons de ces modifications. <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">Découvrez les bonnes pratiques ici.</a></li></td>
  </tr>
  <tr>
    <td>Livres</td>
    <td><li>Créez un manuel d’utilisateur ou un manuel d’administration pour les utilisateurs internes intégrés à l’instance.</li></td>
  </tr>
  <tr>
    <td>Conversations avec les équipes internes</td>
    <td><li>Commencez à aligner les attentes de l’équipe marketing interne à l’égard des Marketo Engage avec les capacités du Marketo Engage.</li>
    <li>Identifiez les équipes qui seront vos parties prenantes dans l’instance de Marketo Engage et documentez leurs objectifs afin d’utiliser Marketo Engage en tant que technologie.</li></td>
  </tr>
</tbody>
</table>
