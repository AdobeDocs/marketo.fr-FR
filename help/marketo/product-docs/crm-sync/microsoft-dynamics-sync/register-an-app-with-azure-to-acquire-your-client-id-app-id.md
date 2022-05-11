---
unique-page-id: 12983390
description: Enregistrement d’une application avec Azure pour acquérir votre ID client/ID d’application - Documents Marketo - Documentation du produit
title: Enregistrement d’une application avec Azure pour acquérir votre ID client/ID d’application
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
source-git-commit: 6f15abf1fed69431b3bbe249c908b0f90a56d391
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Enregistrement d’une application avec Azure pour acquérir votre ID client/ID d’application {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Principale Directory étend vos répertoires sur site dans le cloud, fournissant la prise en charge de MS Dynamics 365 CRM avec authentification ADFS On-premise.

## Enregistrement d’une nouvelle application {#registering-a-new-app}

1. [Connexion](https://login.microsoftonline.com/){target=&quot;_blank&quot;} vers le portail de gestion Microsoft Azure à l’aide d’un compte avec des autorisations d’administrateur. Vous pouvez également accéder au portail Microsoft Azure à l’aide du Centre d’administration Office 365 en développant le **Administration** dans le volet de navigation de gauche et en sélectionnant **Azure AD**.

   >[!CAUTION]
   >
   >Vous devez utiliser un compte dans le même abonnement Office 365 que celui avec lequel vous envisagez d’enregistrer l’application.

   >[!NOTE]
   >
   >Si vous n’avez pas de compte Azure, vous pouvez [inscription](https://azure.microsoft.com/en-us/free/){target=&quot;_blank&quot;} pour une seule. Pour plus d’informations, reportez-vous à la documentation Microsoft ou contactez votre représentant Microsoft. Une fois que vous avez créé un compte Azure, vous pouvez enregistrer une ou plusieurs applications en suivant la procédure décrite ci-dessous.
   >
   >
   >Si vous disposez d’un compte Azure mais que votre abonnement Office 365 avec Microsoft Dynamics 365 n’est pas disponible dans votre abonnement Azure, suivez [ces instructions](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target=&quot;_blank&quot;} pour associer les deux comptes.

1. Rechercher et cliquer sur **Azure Principal Directory** dans le volet de navigation de gauche.

   ![](assets/two.png)

1. Sous Gérer, cliquez sur **Inscriptions des applications**.

   ![](assets/three.png)

1. Cliquez sur **Nouvelle inscription** en haut de la page.

   ![](assets/four.png)

1. Saisissez un nom pour votre application, sélectionnez le type de compte approprié, puis saisissez une URL de redirection. Cliquez ensuite sur **Enregistrer** au bas de la page.

   ![](assets/five.png)

1. Votre application devrait maintenant apparaître dans la **Inscriptions des applications** .

   ![](assets/six.png)

## Configuration des autorisations d’application {#configuring-app-permissions}

1. Sous , **Inscriptions des applications** dans votre Principal Directory, cliquez sur l’application pour laquelle vous souhaitez configurer des autorisations.

   ![](assets/seven.png)

1. Sous Gérer, cliquez sur **Autorisations d’API**.

   ![](assets/eight.png)

1. Cliquez sur le bouton **Ajouter une autorisation** bouton .

   ![](assets/nine.png)

1. Choisir **Dynamics CRM**.

   ![](assets/ten.png)

1. Vérifiez les **Accès à Common Data Service en tant qu’utilisateurs de l’organisation****** , puis cliquez sur **Ajoutez des autorisations.**

   ![](assets/eleven.png)

1. Une fois les autorisations ajoutées, patientez au moins 10 secondes.

   ![](assets/twelve.png)

1. Cliquez sur le bouton **Autorisation du consentement de l’administrateur** bouton .

   ![](assets/thirteen.png)

1. Cliquez sur **Oui** pour confirmer.

   ![](assets/fourteen.png)

   Et vous avez fini !

   ![](assets/fifteen.png)
