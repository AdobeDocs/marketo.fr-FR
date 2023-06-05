---
description: Connexion à Outlook - Documents Marketo - Documentation du produit
title: Se connecter à Outlook
source-git-commit: 2538bd5973eb3372352c3ddbada6521911f9fc33
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 1%

---

# Se connecter à Outlook {#connect-to-outlook}

Découvrez comment connecter votre compte d’actions d’aperçu des ventes à Outlook.

>[!NOTE]
>
>Chaque utilisateur doit se connecter à Outlook à partir de son compte de vente Marketo.

## Connexion à Outlook Online {#connecting-to-outlook-online}

La connexion à Outlook signifie que vous recevrez le suivi des réponses, l’accès au canal de diffusion Outlook, la possibilité de planifier des emails dans Outlook et d’envoyer la conformité.

1. Dans Marketo Sales, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/connect-to-outlook-1.png)

1. Sous Mon compte, sélectionnez **Paramètres de messagerie électronique**.

   ![](assets/connect-to-outlook-2.png)

1. Cliquez sur le bouton **Connexion par e-mail** .

   ![](assets/connect-to-outlook-3.png)

1. Cliquez sur **Prise en main**.

   ![](assets/connect-to-outlook-4.png)

1. Sélectionner **J’utilise Outlook pour envoyer des emails** et cliquez sur **Suivant**.

   ![](assets/connect-to-outlook-5.png)

1. Sélectionnez la version d’Outlook que vous utilisez, puis cliquez sur **Suivant**. Dans cet exemple, nous choisissons Outlook Online.

   ![](assets/connect-to-outlook-6.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td> 
      <td>Également appelé Exchange Online</td> 
     </tr>
     <tr>
      <td><strong>Exchange On-premise</strong></td> 
      <td>Inclut Exchange 2013 et 2016</td> 
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Marketo ne prend actuellement pas en charge les comptes hybrides Exchange.

1. Cliquez sur **OK**.

   ![](assets/connect-to-outlook-7.png)

1. Si vous n’êtes pas connecté à Outlook, saisissez les informations de connexion, puis cliquez sur **Suivant**. Si tel est le cas, sélectionnez le compte auquel vous souhaitez vous connecter, puis cliquez sur **Suivant**. Dans cet exemple, nous sommes déjà connectés.

   ![](assets/connect-to-outlook-8.png)

1. Cliquez sur **Accepter**.

   ![](assets/connect-to-outlook-9.png)

   Vous pouvez utiliser cette connexion pour effectuer le suivi des emails, mais aussi comme canal de diffusion.

   >[!NOTE]
   >
   >Outlook Online (Office365) applique ses propres limites d’envoi. [En savoir plus ici](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md#email-provider-limits).

## Connexion à Exchange On-Premise {#connecting-to-exchange-on-premise}

La connexion à Exchange On-Premise signifie que vous recevrez le suivi des réponses, l’accès au canal de diffusion Outlook, la possibilité de planifier des emails dans Outlook et d’envoyer la conformité.

1. Dans Marketo Sales, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/connect-to-outlook-10.png)

1. Sous Mon compte, sélectionnez **Paramètres de messagerie électronique**.

   ![](assets/connect-to-outlook-11.png)

1. Cliquez sur le bouton **Connexion par e-mail** .

   ![](assets/connect-to-outlook-12.png)

1. Cliquez sur **Prise en main**.

   ![](assets/connect-to-outlook-13.png)

1. Sélectionner **J’utilise Outlook pour envoyer des emails** et cliquez sur **Suivant**.

   ![](assets/connect-to-outlook-14.png)

1. Sélectionnez la version d’Outlook que vous utilisez, puis cliquez sur **Suivant**. Dans cet exemple, nous choisissons Exchange On-premise.

   ![](assets/connect-to-outlook-15.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td> 
      <td>Également appelé Exchange Online</td> 
     </tr>
     <tr>
      <td><strong>Exchange On-premise</strong></td> 
      <td>Inclut Exchange 2013 et 2016</td> 
     </tr>
    </tbody>
   </table>

1. Saisissez vos informations d’identification, puis cliquez sur **Connexion**.

   ![](assets/connect-to-outlook-16.png)

   >[!NOTE]
   >
   >Si vous désactivez la détection automatique dans la liste déroulante Version d’Exchange, vous devrez demander à votre service informatique l’URL d’Exchange.

   Vous pouvez utiliser cette connexion pour effectuer le suivi des emails, mais aussi comme canal de diffusion.

   >[!NOTE]
   >
   >Lors de l’utilisation d’Exchange On-premise, votre équipe informatique établira votre limite d’envoi des emails.

## Obtention de l’autorisation de connexion à Outlook Online {#getting-permission-to-connect-to-outlook-online}

Vous devrez peut-être collaborer avec votre équipe informatique pour obtenir l’autorisation de Marketo Sales de vous connecter à votre compte Outlook Online (Microsoft 365).

>[!NOTE]
>
>Informez l’équipe informatique qui gère votre compte Microsoft 365 que l’application à laquelle vous devez accéder est &quot;Marketo Sales Connect&quot;.

Selon les préférences de votre équipe informatique et la configuration actuelle, il est préférable de les consulter pour savoir comment accorder l’accès. Vous trouverez ci-dessous quelques articles qui peuvent guider la conversation.

* Consentement global : [Applications intégrées et Azure AD pour les administrateurs Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365/enterprise/integrated-apps-and-azure-ads?view=o365-worldwide){target="_blank"}
* Consentement de l’utilisateur : [Configuration du consentement des utilisateurs pour les applications](https://learn.microsoft.com/en-us/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal&amp;pivots=portal){target="_blank"}
* Consentement de l’administrateur : [Configuration du processus de consentement de l’administrateur](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* Activation ou désactivation du consentement de l’utilisateur : [Gestion du consentement des utilisateurs pour les applications dans Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* Gestion avec Microsoft Defender : [Gestion des applications OAuth](https://learn.microsoft.com/en-us/defender-cloud-apps/manage-app-permissions){target="_blank"}
