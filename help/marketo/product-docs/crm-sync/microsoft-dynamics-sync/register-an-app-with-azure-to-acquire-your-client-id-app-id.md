---
unique-page-id: 12983390
description: Enregistrement d'une application avec Azure pour acquérir votre ID client/ID d'application - Marketo Docs - Documentation du produit
title: Enregistrer une application avec Azure pour acquérir votre ID client/ID d'application
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Enregistrer une application avec Azure pour acquérir votre ID client/ID d&#39;application {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Principale Directory étend vos répertoires locaux dans le cloud, fournissant la prise en charge de MS Dynamics 365 CRM avec authentification ADFS sur site.

## Enregistrement d’une nouvelle application {#registering-a-new-app}

1. [Connectez-vous ](https://manage.windowsazure.com/) au portail de gestion Microsoft Azure à l&#39;aide d&#39;un compte doté d&#39;autorisations d&#39;administrateur. Vous pouvez également accéder au portail Microsoft Azure via le Centre d&#39;administration Office 365 en développant l&#39;élément **Admin** dans le volet de navigation de gauche et en sélectionnant **Azure AD**.

   >[!CAUTION]
   >
   >Vous devez utiliser un compte dans le même abonnement Office 365 que celui avec lequel vous souhaitez enregistrer l’application.

   >[!NOTE]
   >
   >Si vous n&#39;avez pas de compte Azure, vous pouvez [vous inscrire](https://azure.microsoft.com/en-us/free/) pour un compte. Consultez la documentation de Microsoft ou contactez votre représentant Microsoft pour plus d&#39;informations. Une fois que vous avez créé un compte Azure, vous pouvez enregistrer une ou plusieurs applications en suivant la procédure décrite ci-dessous.
   >
   >
   >Si vous avez un compte Azure mais que votre abonnement Office 365 avec Microsoft Dynamics 365 n&#39;est pas disponible dans votre abonnement Azure, suivez [ces instructions](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) pour associer les deux comptes.

1. Recherchez **Azure Principale Directory** et cliquez dessus dans le volet de navigation de gauche.

   ![](assets/two.png)

1. Sous Gérer, cliquez sur **Inscriptions de l’application**.

   ![](assets/three.png)

1. Cliquez sur **Nouvelle inscription** en haut de la page.

   ![](assets/four.png)

1. Saisissez un nom pour votre application, choisissez le type de compte approprié, puis saisissez une URL de redirection. Cliquez ensuite sur **S’inscrire** en bas de la page.

   ![](assets/five.png)

1. Vous devriez maintenant voir votre application dans l&#39;onglet **Inscriptions de l&#39;application**.

   ![](assets/six.png)

## Configuration des autorisations d’application {#configuring-app-permissions}

1. Sous l&#39;onglet **Inscriptions de l&#39;application** de votre Principal Directory, cliquez sur l&#39;application pour laquelle vous souhaitez configurer les autorisations.

   ![](assets/seven.png)

1. Sous Gérer, cliquez sur **Autorisations d’API**.

   ![](assets/eight.png)

1. Cliquez sur le bouton **Ajouter une autorisation**.

   ![](assets/nine.png)

1. Sélectionnez **Dynamics CRM**.

   ![](assets/ten.png)

1. Cochez la case **Accéder au service de données commun en tant qu&#39;utilisateur de l&#39;organisation****s**, puis cliquez sur **Ajouter les autorisations.**

   ![](assets/eleven.png)

1. Une fois les autorisations ajoutées, patientez au moins 10 secondes.

   ![](assets/twelve.png)

1. Cliquez sur le bouton **Octroyer le consentement de l’administrateur**.

   ![](assets/thirteen.png)

1. Cliquez sur **Oui** pour confirmer.

   ![](assets/fourteen.png)

   Et vous avez fini !

   ![](assets/fifteen.png)
