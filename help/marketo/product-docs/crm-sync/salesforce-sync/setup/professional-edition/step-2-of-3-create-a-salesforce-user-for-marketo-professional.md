---
unique-page-id: 3571797
description: Étape 2 sur 3 - Création d’un utilisateur Salesforce pour Marketo (professionnel) - Documentation de Marketo - Documentation du produit
title: 'Étape 2 sur 3 : création d’un utilisateur Salesforce pour Marketo (professionnel)'
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Étape 2 sur 3 : création d’un utilisateur [!DNL Salesforce] pour Marketo (professionnel) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Ces étapes doivent être effectuées par un administrateur Salesforce.

>[!PREREQUISITES]
>
>[Étape 1 de 3 : ajouter des champs Marketo à Salesforce (professionnel)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}

Dans cet article, vous allez personnaliser les autorisations de champ avec une mise en page [!DNL Salesforce] et créer un utilisateur de synchronisation [!DNL Salesforce] à Marketo.

## Définir les mises en page {#set-page-layouts}

[!DNL Salesforce] Professional définit l’accessibilité au niveau du champ avec des mises en page, par opposition aux profils d’[!DNL Salesforce] Enterprise/Unlimited. La procédure suivante permet à l’utilisateur de la synchronisation Marketo de mettre à jour les champs personnalisés.

1. Saisissez « [!UICONTROL mises en page] » dans la barre de recherche de navigation sans appuyer sur **[!UICONTROL Entrée]**, puis cliquez sur **[!UICONTROL Mise en page]** sous **[!UICONTROL Prospects]**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Cliquez sur **[!UICONTROL Modifier]** en regard de la disposition des leads.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Cliquez sur une nouvelle **[!UICONTROL Section]** et faites-la glisser dans la mise en page.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Saisissez « Marketo » pour **[!UICONTROL Nom de la section]** et cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Cliquez sur le champ **[!UICONTROL Date d’acquisition]** et faites-le glisser dans la section **Marketo**.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Répétez l&#39;étape ci-dessus pour les champs suivants :

   * [!UICONTROL Programme d’acquisition]
   * [!UICONTROL ID du programme d’acquisition]
   * [!UICONTROL Désinscription Aux E-Mails]
   * [!UICONTROL  Ville déduite ]
   * [!UICONTROL Société déduite]
   * [!UICONTROL Pays déduit]
   * [!UICONTROL Région métropolitaine déduite]
   * [!UICONTROL Indicatif téléphonique déduit]
   * [!UICONTROL Code postal déduit]
   * [!UICONTROL Région d’État déduite]
   * [!UICONTROL  Score du lead ]
   * [!UICONTROL Référent original]
   * [!UICONTROL Moteur de recherche original]
   * [!UICONTROL Expression de recherche originale]
   * [!UICONTROL Informations Source d’origine]
   * [!UICONTROL Type Source d’origine]

   >[!NOTE]
   >
   >Ces champs doivent être dans la mise en page pour que Marketo puisse les lire/écrire.

   >[!TIP]
   >
   >Créez deux colonnes pour les champs en faisant glisser vers le bas à droite de la page. Vous pouvez déplacer des champs d’un côté à l’autre pour équilibrer la longueur des colonnes.

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé d’ajouter des champs.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Répétez toutes les étapes ci-dessus pour le Salesforce **[!UICONTROL mise en page du contact]**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. N’oubliez pas de cliquer sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé avec la **[!UICONTROL Mise en page du contact]**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >Assurez-vous que le champ **[!UICONTROL Événement d’une journée entière]** a été ajouté à la **[!UICONTROL Mise en page de l’événement]**.

## Créer un utilisateur de synchronisation {#create-sync-user}

Marketo requiert des informations d’identification pour accéder à [!DNL Salesforce]. Il est préférable de le faire avec un utilisateur dédié créé avec les étapes ci-dessous.

>[!NOTE]
>
>Si votre entreprise ne dispose pas de licences Salesforce supplémentaires, vous pouvez utiliser un utilisateur ou une utilisatrice marketing disposant du profil d’administration système.

1. Saisissez « users » (utilisateurs) dans la barre de recherche de navigation, puis cliquez sur **[!UICONTROL Utilisateurs]** sous **[!UICONTROL Gérer les utilisateurs]**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Cliquez sur **[!UICONTROL Nouvel utilisateur]**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Renseignez les champs obligatoires, sélectionnez l’**[!UICONTROL Licence utilisateur : Salesforce]**, définissez le **[!UICONTROL Profil : administrateur système]**, cochez la case **[!UICONTROL Utilisateur marketing]** et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Vérifiez que l’adresse e-mail saisie est valide. Vous devrez vous connecter en tant qu’utilisateur de synchronisation pour réinitialiser le mot de passe.

Excellent ! Vous disposez désormais d’un compte que Marketo peut utiliser pour se connecter à [!DNL Salesforce]. Faisons-le.

>[!MORELIKETHIS]
>
>[Étape 3 sur 3 : connecter Marketo et Salesforce (professionnel)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md){target="_blank"}
