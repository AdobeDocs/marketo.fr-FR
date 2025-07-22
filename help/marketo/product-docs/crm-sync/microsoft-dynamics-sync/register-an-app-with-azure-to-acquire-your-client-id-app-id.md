---
unique-page-id: 12983390
description: Enregistrer une application avec Azure pour acquérir votre ID client/ID d’application - Documents Marketo - Documentation du produit
title: Enregistrez une application avec Azure pour acquérir votre ID client/ID d’application
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Enregistrez une application avec Azure pour acquérir votre ID client/ID d’application {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory étend vos annuaires locaux dans le cloud, fournissant la prise en charge de [!DNL MS Dynamics 365] CRM avec l&#39;authentification ADFS sur site.

## Enregistrement d’une nouvelle application {#registering-a-new-app}

1. [Connectez-vous](https://login.microsoftonline.com/){target="_blank"} au portail de gestion Microsoft Azure à l’aide d’un compte disposant d’autorisations d’administrateur. Vous pouvez également accéder au portail Microsoft Azure par le biais du Centre d’administration Office 365 en développant l’élément **[!UICONTROL Admin]** dans le volet de navigation de gauche et en sélectionnant **[!UICONTROL Azure AD]**.

   >[!CAUTION]
   >
   >Vous devez utiliser un compte dans le même abonnement [!DNL Office 365] que celui avec lequel vous avez l’intention d’enregistrer l’application.

   >[!NOTE]
   >
   >Si vous ne disposez pas d’un compte Azure, vous pouvez vous [inscrire](https://azure.microsoft.com/en-us/free/){target="_blank"} pour l’un d’eux. Reportez-vous à la documentation de Microsoft ou contactez votre représentant Microsoft pour plus d’informations. Une fois que vous avez créé un compte Azure, vous pouvez enregistrer une ou plusieurs applications en suivant la procédure décrite ci-dessous.
   >
   >
   >Si vous disposez d’un compte Azure, mais que votre abonnement [!DNL Office 365] avec [!DNL Microsoft Dynamics 365] n’est pas disponible dans votre abonnement Azure, suivez [ces instructions](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"} pour associer les deux comptes.

1. Recherchez et cliquez sur **[!UICONTROL Azure Active Directory]** dans le volet de navigation de gauche.

   ![](assets/two.png)

1. Sous [!UICONTROL Gérer], cliquez sur **[!UICONTROL Enregistrement des applications]**.

   ![](assets/three.png)

1. Cliquez sur **[!UICONTROL Nouvel enregistrement]** en haut de la page.

   ![](assets/four.png)

1. Saisissez un nom pour votre application, choisissez votre type de compte applicable et saisissez une URL de redirection. Cliquez ensuite sur **[!UICONTROL Enregistrer]** au bas de la page.

   ![](assets/five.png)

1. Votre application doit maintenant apparaître dans l’onglet **[!UICONTROL Enregistrements des applications]**.

   ![](assets/six.png)

## Configuration des autorisations d’application {#configuring-app-permissions}

1. Sous l’onglet **[!UICONTROL Enregistrements des applications]** dans votre Active Directory, cliquez sur l’application pour laquelle vous souhaitez configurer des autorisations.

   ![](assets/seven.png)

1. Sous [!UICONTROL Gérer], cliquez sur **[!UICONTROL Autorisations d’API]**.

   ![](assets/eight.png)

1. Cliquez sur le bouton **[!UICONTROL Ajouter une autorisation]**.

   ![](assets/nine.png)

1. Choisissez **[!UICONTROL Dynamics CRM]**.

   ![](assets/ten.png)

1. Cochez la case **[!UICONTROL Accéder au service commun de données en tant qu’utilisateurs de l’organisation]** puis cliquez sur **[!UICONTROL Ajouter des autorisations].**

   ![](assets/eleven.png)

1. Une fois les autorisations ajoutées, patientez au moins 10 secondes.

   ![](assets/twelve.png)

1. Cliquez sur le bouton **[!UICONTROL Accorder le consentement administrateur]**.

   ![](assets/thirteen.png)

1. Cliquez sur **[!UICONTROL Oui]** pour confirmer.

   ![](assets/fourteen.png)

   Et c&#39;est fini !

   ![](assets/fifteen.png)
