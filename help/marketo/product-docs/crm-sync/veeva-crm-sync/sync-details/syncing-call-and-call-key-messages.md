---
description: Synchronisation des messages clés d’appel et d’appel - Documents Marketo - Documentation du produit
title: Synchronisation des messages clés d’appel et d’appel
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 9%

---

# Synchronisation des messages clés d’appel et d’appel {#syncing-call-and-call-key-messages}

Les objets de message clé d’appel et d’appel dans le CRM Veeva sont synchronisés par défaut dans Marketo Engage. Marketo synchronise les données qui ont jusqu’à 6 mois, en fonction de la date de création de l’appel.

>[!NOTE]
>
>Marketo conserve les données d’appel jusqu’à six mois à compter de la date de l’appel.

**Quels sont les déclencheurs/filtres liés aux messages de clé d’appel et d’appel ?**

Déclencheurs :

* Ajout à l’appel
* Supprimé de l’appel
* Ajout à l’appel du message clé
* Supprimé du message de clé d’appel
* Appel mis à jour
* Message de la clé d’appel mise à jour

Filtres:

* Comporte un appel
* Comporte un message de clé d’appel

Les champs suivants des messages Appel et Clé d’appel sont synchronisés et peuvent être utilisés comme contraintes et déclencheurs.

<table>
  <colgroup>
    <col>
    <col>
    <col>
    <col>
    <col>
  </colgroup>
  <thead>
    <tr>
      <th>
        Objet
      </th>
      <th>
        Intitulé de champ
      </th>
      <th>
        Description
      </th>
      <th>
        Nom de champ
      </th>
      <th>
        Type de données
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Appel</td>
      <td>Comptable</td>
      <td>Recherchez le compte auquel l’appel est associé.</td>
      <td>Account_vod__c</td>
      <td>Recherche (compte)</td>
    </tr>
    <tr>
      <td>Appel</td>
      <td>Type d’appel</td>
      <td>Type d’appel conservé par le système en fonction du type et du contenu de l’appel. Ce champ est utilisé à des fins de création de rapports. Les valeurs valides sont : Détail uniquement, Détail avec exemple, Détails du groupe, Détails du groupe avec exemple, Exemple uniquement. Ces valeurs ne doivent pas être modifiées, mais les traductions de ces listes de sélection peuvent être modifiées. Les participants ont le même type d’appel que l’appel d’en-tête. Pour un appel de groupe avec 3 professionnels, les 4 enregistrements ont tous le type d’appel "Détails du groupe".</td>
      <td>Call_Type_vod__c</td>
      <td>Liste de sélection</td>
    </tr>
    <tr>
     <td>Appel</td>
      <td>Contact</td>
      <td>Recherchez le contact auquel l’appel est associé (le cas échéant).</td>
      <td>Contact_vod__c</td>
      <td>Lookup(Contact)</td>
    </tr>
    <tr>
      <td>Appel</td>
      <td>Date</td>
      <td>Date de l’appel au moment où il a été enregistré ou envoyé pour la première fois. Ce champ est défini à la date courante via un déclencheur si le champ date ou datetime n’est pas renseigné.</td>
      <td>Call_Date_vod__c</td>
      <td>Date</td>
    </tr>
    <tr>
      <td>Appel</td>
      <td>Est-ce que Parent Call ?</td>
      <td>Champ de formule pour déterminer si l’enregistrement d’appel est l’enregistrement d’appel parent ou d’appel de participant. 1 indique que l’enregistrement est l’appel parent. 0 indique qu’il s’agit d’un appel de participant.</td>
      <td>Is_Parent_Call_vod__c</td>
      <td>Formule (nombre)</td>
    </tr>
    <tr>
      <td>Appel</td>
      <td>Statut</td>
      <td>État de l’appel — Planifié, Enregistré ou Envoyé. Utilisez les outils de traduction pour modifier les valeurs d’affichage. Les déclencheurs à l’appel examinent ce champ pour voir si l’appel est verrouillé (envoyé). Cette valeur est définie pour l’utilisateur lorsque vous appuyez sur le bouton Enregistrer ou Envoyer.</td>
      <td>Status_vod__c</td>
      <td>Liste de sélection</td>
    </tr>
    <tr>
      <td>Appel</td>
      <td>Type d’enregistrement</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>Type d’enregistrement</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Appel</td>
      <td>Recherche de l’appel. Chaque message clé est associé à un appel .</td>
      <td>Call2_vod__c</td>
      <td>Principal-Detail(Call)</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Catégorie</td>
      <td>Enregistre la catégorie de messages du message. Utilisé principalement à des fins de création de rapports.</td>
      <td>Category_vod__c</td>
      <td>Liste de sélection</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Nom de présentation du CLM</td>
      <td>Nom de présentation de la ligne de commande bloquée</td>
      <td>Clm_Presentation_Name_vod__c</td>
      <td>Texte (80)</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Nom du message clé</td>
      <td>Nom du message de clé empilée</td>
      <td>Key_Message_Name_vod__c</td>
      <td>Texte (80)</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Nom du produit</td>
      <td> </td>
      <td>Product_Name__c</td>
      <td>Formule (Texte)</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Réaction</a>
      </td>
      <td>Liste des réactions au message. Modifiez la liste de sélection pour modifier les valeurs de réaction.</td>
      <td>Reaction_vod__c</td>
      <td>Liste de sélection</td>
    </tr>
  </tbody>
</table>
