---
unique-page-id: 12983390
description: Enregistrement d’une application avec Azure pour acquérir votre ID client/ID d’application - Documents Marketo - Documentation du produit
title: Enregistrer une application avec Azure pour acquérir votre ID client/ID d’application
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Enregistrer une application avec Azure pour acquérir votre ID client/ID d’application {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory étend vos répertoires sur site dans le cloud, fournissant ainsi une prise en charge du CRM MS Dynamics 365 avec authentification ADFS on-premise.

## Enregistrement d’une nouvelle application {#registering-a-new-app}

1. [Connectez-vous](https://login.microsoftonline.com/){target="_blank"} au portail de gestion Microsoft Azure à l’aide d’un compte avec des autorisations d’administrateur. Vous pouvez également accéder au portail Microsoft Azure via le Centre d’administration Office 365 en développant l’élément **[!UICONTROL Admin]** dans le volet de navigation de gauche et en sélectionnant **[!UICONTROL Azure AD]**.

   >[!CAUTION]
   >
   >Vous devez utiliser un compte dans le même abonnement Office 365 que celui avec lequel vous envisagez d’enregistrer l’application.

   >[!NOTE]
   >
   >Si vous n&#39;avez pas de compte Azure, vous pouvez [vous inscrire](https://azure.microsoft.com/en-us/free/){target="_blank"} pour un compte Azure. Pour plus d’informations, reportez-vous à la documentation Microsoft ou contactez votre représentant Microsoft. Une fois que vous avez créé un compte Azure, vous pouvez enregistrer une ou plusieurs applications en suivant la procédure décrite ci-dessous.
   >
   >
   >Si vous disposez d’un compte Azure mais que votre abonnement Office 365 avec Microsoft Dynamics 365 n’est pas disponible dans votre abonnement Azure, suivez [ces instructions](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"} pour associer les deux comptes.

1. Recherchez et cliquez sur **[!UICONTROL Azure Active Directory]** dans le volet de navigation de gauche.

   ![](assets/two.png)

1. Sous Gérer, cliquez sur **[!UICONTROL Inscriptions des applications]**.

   ![](assets/three.png)

1. Cliquez sur **[!UICONTROL New registration]** en haut de la page.

   ![](assets/four.png)

1. Saisissez un nom pour votre application, sélectionnez le type de compte approprié, puis saisissez une URL de redirection. Cliquez ensuite sur **[!UICONTROL Enregistrer]** en bas de la page.

   ![](assets/five.png)

1. Votre application devrait maintenant s’afficher dans l’onglet **[!UICONTROL Inscriptions de l’application]** .

   ![](assets/six.png)

## Configuration des autorisations d’application {#configuring-app-permissions}

1. Sous l’onglet **[!UICONTROL Inscriptions des applications]** de votre Active Directory, cliquez sur l’application pour laquelle vous souhaitez configurer des autorisations.

   ![](assets/seven.png)

1. Sous Gérer, cliquez sur **[!UICONTROL Autorisations d’API]**.

   ![](assets/eight.png)

1. Cliquez sur le bouton **[!UICONTROL Ajouter une autorisation]** .

   ![](assets/nine.png)

1. Sélectionnez **[!UICONTROL Dynamics CRM]**.

   ![](assets/ten.png)

1. Cochez la case **[!UICONTROL Accéder au service de données commun en tant qu&#39;utilisateurs de l&#39;organisation]**, puis cliquez sur **[!UICONTROL Ajouter des autorisations]**.

   ![](assets/eleven.png)

1. Une fois les autorisations ajoutées, patientez au moins 10 secondes.

   ![](assets/twelve.png)

1. Cliquez sur le bouton **[!UICONTROL Accorder le consentement des administrateurs]** .

   ![](assets/thirteen.png)

1. Cliquez sur **[!UICONTROL Oui]** pour confirmer.

   ![](assets/fourteen.png)

   Et vous avez fini !

   ![](assets/fifteen.png)
