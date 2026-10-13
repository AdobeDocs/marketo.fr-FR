---
unique-page-id: 7504051
description: Découvrez comment gérer les données de personne dans Marketo Engage, notamment comment gérer les données de personne manage-person-data. Utilisez ce guide pour passer à l’étape suivante.
title: Gérer les données de personne
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/rIiC-JXLkaMByk7GizVOcCEcUHN8AL-8Hy66-U2GZhs'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
    internal-label: Segmentation
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 24%
---
# Gérer les données de personne {#manage-person-data}

Tirez parti des données de personne pour les [!DNL Web Personalization] en sélectionnant les champs de personne à utiliser dans votre segmentation.

1. Accédez à **[!UICONTROL Paramètres du compte]**.

   ![](assets/image2015-5-7-15-3a17-3a23.png)

1. Accédez à **[!UICONTROL Base de données]**.

   ![](assets/account-settings-dropdown-database.jpg)

## Ajout d’un champ Personne {#adding-a-new-person-field}

1. Sélectionnez **Champ à ajouter** dans la liste déroulante pour ajouter un champ de données personne à la liste.

   ![](assets/add-a-person-field-hand.jpg)

   >[!NOTE]
   >
   >Un nouveau champ est ajouté avec un statut En attente et son activation peut prendre jusqu’à 24 heures.

## Supprimer un champ de personne {#deleting-a-person-field}

1. Cliquez sur l’icône de suppression ( ![—](assets/image2015-3-24-13-3a45-3a56.png)) pour supprimer un champ de la liste. Cliquez sur **[!UICONTROL Oui]** pour confirmer la suppression du champ.

   ![](assets/web-engagement-settings-delete.jpg)

   >[!NOTE]
   >
   >**Gestion des champs de données de personne**
   >
   >* Seuls les champs de données Personne peuvent être inclus.
   >* Vous pouvez ajouter jusqu’à 30 champs de données Personne
   >* L’activation des nouveaux champs ajoutés peut prendre jusqu’à 24 heures.
   >* La longueur maximale de chaînes de caractères est de 255 caractères.
   >* Les champs masqués seront automatiquement supprimés

<table>
 <tbody>
  <tr>
   <th><p>REST API Nom</p></th>
   <th><p>SOAP API Nom</p></th>
   <th><p>Nom convivial</p></th>
  </tr>
  <tr>
   <td><p>service</p></td>
   <td><p>Service</p></td>
   <td><p>Service</p></td>
  </tr>
  <tr>
   <td><p>titre</p></td>
   <td><p>Titre</p></td>
   <td><p>Intitulé du poste</p></td>
  </tr>
  <tr>
   <td><p>évaluation</p></td>
   <td><p>Évaluation</p></td>
   <td><p>Évaluation</p></td>
  </tr>
  <tr>
   <td><p>leadScore</p></td>
   <td><p>LeadScore</p></td>
   <td><p>Score</p></td>
  </tr>
  <tr>
   <td><p>leadStatus</p></td>
   <td><p>LeadStatus</p></td>
   <td><p>Statut</p></td>
  </tr>
  <tr>
   <td><p>priorité</p></td>
   <td><p>Priorité</p></td>
   <td><p>Priorité</p></td>
  </tr>
  <tr>
   <td><p>leadRole</p></td>
   <td><p>LeadRole</p></td>
   <td><p>Rôle</p></td>
  </tr>
  <tr>
   <td><p>désabonné</p></td>
   <td><p>Désabonné ou désabonnée</p></td>
   <td><p>Désabonné ou désabonnée</p></td>
  </tr>
 </tbody>
</table>

Les champs de prospect suivants sont fournis prêts à l’emploi pour les nouveaux comptes [!DNL Web Personalization] :

>[!MORELIKETHIS]
>
>[Créer un segment à l’aide de données de personne connues](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
