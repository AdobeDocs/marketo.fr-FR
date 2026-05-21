---
description: Documentez la configuration de votre nouvelle instance Marketo Engage.
title: 'Bonnes Pratiques Relatives Aux Nouvelles Instances : Documentez Votre Configuration'
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
TQID: https://experienceleague.adobe.com/pqbf84tAUt49rWUD7rONRuZNgR8v5yMmYTqwqlXqgAs
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2: id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 536
ht-degree: 4%

---

# Bonnes pratiques relatives à une nouvelle instance : documenter votre configuration {#new-instance-best-practices-document-your-setup}

Maintenant que vous avez appris les principales zones de produit à configurer pour une nouvelle instance de Marketo Engage, l’étape suivante consiste à créer de la documentation pour la configuration de votre instance et tech stack. Que vous le créiez par le biais d’une feuille de calcul ou d’une application de gestion de projet, votre documentation sera une excellente ressource pour suivre la progression et enregistrer les détails, ainsi que pour maintenir votre instance structurée et durable pour les futurs spécialistes du marketing au sein de votre organisation.

## Données {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Importer une liste</td>
    <td><li>Collectez une liste des sources de données à partir desquelles les enregistrements seront extraits <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people" target="_blank">à importer dans Marketo Engage</a>.</li>
    <li>Si vous effectuez un import à partir de plusieurs sources de données, pensez à utiliser des listes de Principal ou à <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">créer un champ personnalisé</a> dans l’enregistrement de personne pour indiquer la source de données.</li></td>
  </tr>
  <tr>
    <td>Intégration de la base de données</td>
    <td><li>Si vous utilisez la synchronisation native entre Marketo Engage et votre CRM, réfléchissez soigneusement aux champs que vous souhaitez synchroniser entre les systèmes. Tous les champs n’ont pas besoin d’être synchronisés. Soyez donc stratégique concernant vos flux de données.</li></td>
  </tr>
</tbody>
</table>

## Documentation {#documentation}

<table>
<thead>
  <tr>
    <th style="width:20%">Zone</th>
    <th style="width:80%">Éléments action</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Utilisateurs et utilisatrices</td>
    <td><li>Documentez les <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">utilisateurs actuels</a> dans votre instance pour des raisons de sécurité. Les détails suivants doivent être inclus au minimum (et sont tous visibles en accédant à Admin &gt; Utilisateurs et rôles) :</li>
    <ul>
    <li>Nom</li>
    <li>E-mail</li>
    <li>Connexion</li>
    <li>Rôle</li>
    <li>Date d'expiration de l'accès</li>
    <li>Date de création de l’utilisateur</li>
    <li>Date de connexion la plus récente</li></ul>
    <p><img src="assets/note-icon.png" alt="icône de note"> REMARQUE : vous pouvez également développer ce point pour inclure la documentation relative aux rôles/autorisations.
    <p>
    <li>En tant qu’administrateur de produit Marketo Engage, développez un processus interne pour auditer et mettre à jour la liste des utilisateurs de Marketo Engage à une cadence régulière. Pour apporter des modifications à la liste des utilisateurs dans Adobe Admin Console, envisagez des <a href="https://helpx.adobe.com/fr/enterprise/using/users.html" target="_blank">actions en bloc</a> telles que le chargement d’un fichier .CSV, l’utilisation de l’API REST User Management, etc.</li></td>
  </tr>
  <tr>
    <td>Organisation</td>
    <td><li>Documentez la structure de dossiers convenue, les conventions de nommage standard pour les programmes, les ressources, etc., et la raison pour laquelle les décisions ont été prises. <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">Pour en savoir plus sur les bonnes pratiques, cliquez ici.</a></li></td>
  </tr>
  <tr>
    <td>Journal des modifications</td>
    <td><li>Créez un journal des modifications dans lequel vous pouvez documenter ce qui change dans votre instance et le motif des modifications. <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">Pour en savoir plus sur les bonnes pratiques, cliquez ici.</a></li></td>
  </tr>
  <tr>
    <td>Playbooks</td>
    <td><li>Créez un playbook d’utilisateur ou un playbook d’administrateur pour les utilisateurs internes qui se connectent à l’instance.</li></td>
  </tr>
  <tr>
    <td>Conversations avec les équipes internes</td>
    <td><li>Alignez les attentes de l’équipe marketing interne de Marketo Engage sur les fonctionnalités de Marketo Engage.</li>
    <li>Identifiez les équipes qui seront vos parties prenantes dans l’instance Marketo Engage et documentez leurs objectifs pour atteindre l’utilisation de Marketo Engage en tant que technologie.</li></td>
  </tr>
  <tr>
    <td>Espaces de travail et partitions (le cas échéant)</td>
    <td><li>Documentez la définition des espaces de travail et leur relation aux partitions de la base de données (par exemple, un espace de travail global qui présente tout le monde par rapport aux secteurs d’activité).</li>
    <li>Importez les nouveaux enregistrements dans la partition appropriée.</li>
    <li>Définissez la valeur dans votre CRM qui place les utilisateurs dans la partition appropriée.</li></td>
  </tr>
</tbody>
</table>
