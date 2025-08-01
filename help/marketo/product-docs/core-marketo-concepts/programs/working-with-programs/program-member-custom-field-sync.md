---
description: Synchronisation des champs personnalisés des membres de programme - Documents Marketo - Documentation du produit
title: Synchronisation des champs personnalisés des membres du programme
exl-id: 7facfc79-a411-4ad9-b847-2002763af5bb
feature: Programs
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 11%

---

# Synchronisation des champs personnalisés des membres du programme {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>* Création de [champs personnalisés du membre de programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target="_blank"}
>* [Synchroniser une campagne  [!DNL Salesforce]  un programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}

>[!NOTE]
>
>L’objet Membre de programme peut avoir jusqu’à 20 champs personnalisés. Ces champs sont disponibles pour tous les programmes.

## Mapper les champs Salesforce aux champs personnalisés des membres de programme {#map-salesforce-fields-to-program-member-custom-fields}

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/program-member-custom-field-sync-1.png)

1. Cliquez sur **[!DNL Salesforce]**, puis sur **[!UICONTROL Modifier]** en regard de Synchronisation des champs personnalisés des membres de programme.

   ![](assets/program-member-custom-field-sync-2.png)

1. Utilisez la zone de recherche pour localiser les champs [!DNL Salesforce] à mapper. Dans cet exemple, nous utilisons l’option Ne pas appeler.

   ![](assets/program-member-custom-field-sync-3.png)

1. Cliquez sur la liste déroulante.

   ![](assets/program-member-custom-field-sync-4.png)

1. Sélectionnez le Marketo [!UICONTROL champ personnalisé de membre de programme] à mapper.

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >La liste déroulante affiche uniquement les [!UICONTROL champs personnalisés du membre de programme] qui correspondent au type de données du champ de [!DNL Salesforce].

1. Pour d’autres mappages de champs, désélectionnez la zone de recherche et répétez les étapes 3 à 5.

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >Les modifications apportées aux données des membres du programme sur les champs mappés seront synchronisées entre Marketo et [!DNL Salesforce] à l’avenir.

   >[!NOTE]
   >
   >Si vous renommez ou modifiez le type de données d’un champ dans [!DNL Salesforce], nous supprimerons tout mappage de ce champ avec le [!UICONTROL champ personnalisé du membre de programme]. Vous pouvez toutefois le remapper avec le nouveau champ après révision.

## Annuler le mappage des champs Salesforce des champs personnalisés des membres du programme {#unmap-salesforce-fields-from-program-member-custom-fields}

Si vous souhaitez libérer un champ pour le remplacer, ou simplement effectuer une modification générale, vous devez d’abord annuler le mappage. Voici comment procéder.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/program-member-custom-field-sync-7.png)

1. Cliquez sur **[!DNL Salesforce]**, puis sur **[!UICONTROL Modifier]** en regard de Synchronisation des champs personnalisés des membres de programme.

   ![](assets/program-member-custom-field-sync-8.png)

1. Utilisez la zone de recherche pour localiser le ou les champs que vous souhaitez annuler le mappage. Dans cet exemple, nous utilisons l’option Ne pas appeler.

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >Vous pouvez cocher la case **[!UICONTROL Mappé]** pour n’afficher que les champs mappés.

1. Annulez le mappage en cliquant sur le **X** en regard du champ.

   ![](assets/program-member-custom-field-sync-10.png)

1. Le mappage est maintenant supprimé. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/program-member-custom-field-sync-11.png)

## Mappage du type de données {#data-type-mapping}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Type de donnés SFDC</th>
      <th>Type de données de champ personnalisé du membre de programme</th>
    </tr>
    <tr>
      <td>Texte</td>
      <td>Chaîne</td>
    </tr>
    <tr>
      <td>Liste de sélection</td>
      <td>Chaîne</td>
    </tr>
    <tr>
      <td>Liste de sélection à sélection multiple</td>
      <td>Chaîne</td>
    </tr>
    <tr>
      <td>Téléphone</td>
      <td>Chaîne</td>
    </tr>
    <tr>
      <td>E-mail</td>
      <td>Chaîne</td>
    </tr>
    <tr>
      <td>Nombre(m)</td>
      <td>Nombre entier</td>
    </tr>
    <tr>
      <td>Nombre(m,n)</td>
      <td>Flottante</td>
    </tr>
    <tr>
      <td>Case à cocher</td>
      <td>Booléen</td>
    </tr>
    <tr>
      <td>URL</td>
      <td>URL</td>
    </tr>
    <tr>
      <td>Date</td>
      <td>Date</td>
    </tr>
    <tr>
      <td>Datetime</td>
      <td>Datetime</td>
    </tr>
    <tr>
      <td>Recherche (référence)</td>
      <td>Chaîne</td>
    </tr>
    <tr>
      <td>Base64</td>
      <td>Chaîne</td>
    </tr>
  </tbody>
</table>

>[!MORELIKETHIS]
>
>* [Modifier les données de membre de programme](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target="_blank"}
>* [Affichez les données sur la grille des Membres du programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target="_blank"}
>* [Synchronisation SFDC - Synchronisation de la campagne](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
