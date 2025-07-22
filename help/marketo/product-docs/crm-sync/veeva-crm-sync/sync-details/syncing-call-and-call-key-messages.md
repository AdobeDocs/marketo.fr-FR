---
description: Synchronisation des messages clés d’appel et d’appel - Documents Marketo - Documentation du produit
title: Synchronisation des messages d’appel et de clé d’appel
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 10%

---

# Synchronisation des messages d’appel et de clé d’appel {#syncing-call-and-call-key-messages}

Les objets Appel et Message Clé d’appel dans [!DNL Veeva] CRM sont synchronisés par défaut dans Marketo Engage. Marketo synchronise les données qui ont jusqu’à 6 mois, en fonction de la date de création de l’appel.

>[!NOTE]
>
>Marketo conserve les données d’appel jusqu’à six mois à compter de la date de l’appel.

**Quels sont les déclencheurs/filtres liés à l’appel et au message de clé d’appel ?**

Déclencheurs :

* Ajouté à l’appel
* Supprimé de l’appel
* Ajouté au message de clé d&#39;appel
* Supprimé du message de clé d&#39;appel
* Appel mis à jour
* Message Clé D’Appel Mis À Jour

Filtres:

* A un appel
* Contient un message de clé d’appel

Les champs suivants des messages Appel et Clé d&#39;appel sont synchronisés et peuvent être utilisés comme contraintes et déclencheurs.

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
        Nom du champ
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
      <td>Recherche du compte auquel l’appel est associé.</td>
      <td>Account_vod__c</td>
      <td>Recherche (compte)</td>
    </tr>
    <tr>
      <td>Appel</td>
      <td>Type d’appel</td>
      <td>Type d’appel qui est géré par le système en fonction du type et du contenu de l’appel. Ce champ est utilisé à des fins de création de rapports. Les valeurs valides sont les suivantes : Détail uniquement, Détail avec échantillon, Détail du groupe, Détail du groupe avec échantillon, Échantillon uniquement. Ces valeurs ne doivent pas être modifiées, mais les traductions de ces listes de sélection peuvent être modifiées. Les participants ont le même type d’appel que l’appel d’en-tête. Pour un appel de groupe avec 3 professionnels, les 4 enregistrements ont le type d’appel « Détails du groupe »</td>
      <td>Call_Type_vod__c</td>
      <td>Liste de sélection</td>
    </tr>
    <tr>
     <td>Appel</td>
      <td>Contact</td>
      <td>Recherchez le contact (le cas échéant) auquel l’appel est associé.</td>
      <td>Contact_vod__c</td>
      <td>Recherche (contact)</td>
    </tr>
    <tr>
      <td>Appel</td>
      <td>Date</td>
      <td>Date de l’appel à laquelle il a été enregistré ou envoyé pour la première fois. Ce champ est défini via un déclencheur sur la date actuelle si aucun champ date ou datetime n’est fourni.</td>
      <td>Call_Date_vod__c</td>
      <td>Date</td>
    </tr>
    <tr>
      <td>Appel</td>
      <td>Est l'appel parent ?</td>
      <td>Champ de formule permettant de déterminer si l’enregistrement d’appel correspond à l’appel parent ou à un enregistrement d’appel de participant. 1 indique que l’enregistrement est l’appel parent. 0 indique qu’il s’agit d’un appel de participant.</td>
      <td>Is_Parent_Call_vod__c</td>
      <td>Formule (Nombre)</td>
    </tr>
    <tr>
      <td>Appel</td>
      <td>Statut</td>
      <td>Statut de l’appel : Planifié, Enregistré ou Envoyé. Utilisez le pupitre de traduction pour modifier les valeurs d’affichage. Les déclencheurs lors de l’appel examinent ce champ pour voir si l’appel est verrouillé (envoyé). Cette valeur est définie pour l’utilisateur ou l’utilisatrice lorsqu’il appuie sur le bouton Enregistrer ou Envoyer.</td>
      <td>Status_vod__c</td>
      <td>Liste de sélection</td>
    </tr>
    <tr>
      <td>Appel</td>
      <td>Type d'enregistrement</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>Type d'enregistrement</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Appel</td>
      <td>Recherche de l’appel. Chaque message clé est associé à un appel.</td>
      <td>Call2_vod__c</td>
      <td>Principal-Detail(Appel)</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Catégorie</td>
      <td>Enregistre la catégorie du message. Utilisé principalement pour la création de rapports.</td>
      <td>Category_vod__c</td>
      <td>Liste de sélection</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Nom de présentation CLM</td>
      <td>Nom de présentation de CLM estampillé</td>
      <td>Clm_Presentation_Name_vod__c</td>
      <td>Texte (80)</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Nom du message clé</td>
      <td>Nom du message de clé horodaté</td>
      <td>Key_Message_Name_vod__c</td>
      <td>Texte (80)</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Nom du produit</td>
      <td> </td>
      <td>Product_Name__c</td>
      <td>Formule (texte)</td>
    </tr>
    <tr>
      <td>Message clé d'appel</td>
      <td>Réaction </a>
      </td>
      <td>Liste de sélection des réactions au message. Modifiez la liste de sélection pour modifier les valeurs de réaction.</td>
      <td>Reaction_vod__c</td>
      <td>Liste de sélection</td>
    </tr>
  </tbody>
</table>
