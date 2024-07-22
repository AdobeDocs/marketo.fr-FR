---
unique-page-id: 14746470
description: Configuration d’un canal de diffusion personnalisé - Documents Marketo - Documentation du produit
title: Configuration d’un canal de diffusion personnalisé
exl-id: a31f7bfd-a4ee-4948-9bdc-b49d47054d40
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 1%

---

# Configuration d’un canal de diffusion personnalisé {#setting-up-a-custom-delivery-channel}

Marketo Sales Connect vous permet de vous intégrer à un serveur SMTP personnalisé pour la diffusion de vos emails. Il s’agit d’une excellente option pour ceux qui ne souhaitent pas envoyer des emails en bloc depuis leur canal de diffusion Gmail ou Exchange.

Les utilisateurs peuvent configurer un serveur SMTP personnalisé pour leur propre utilisation, ou les administrateurs peuvent configurer un serveur SMTP d’équipe à partager avec tous les utilisateurs de Sales Connect de votre instance.

>[!NOTE]
>
>* Outre la configuration de votre serveur SMTP, votre [ identité email doit être vérifiée ](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) avant de pouvoir envoyer des emails.
>* Nous vous recommandons de travailler avec votre équipe informatique ou votre fournisseur de serveur SMTP pour obtenir les informations d’identification de serveur appropriées pour votre serveur SMTP.
>* Vous ne pouvez pas connecter votre serveur Gmail et Exchange à l’aide des informations d’identification du serveur SMTP. Utilisez notre service Email Connection pour vous intégrer à ces fournisseurs.

## SMTP personnalisé {#custom-smtp}

1. Connectez-vous à l’ [application web](https://toutapp.com/login), cliquez sur l’icône en forme d’engrenage en haut à droite et sélectionnez **Paramètres**.

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. Sous Mon compte, cliquez sur **Paramètres de courrier électronique**.

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. Cliquez sur **Canal de diffusion personnalisé**.

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. Saisissez vos informations d’identification SMTP Server et cliquez sur **Connect**.

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >S’il s’agit de votre seul canal de diffusion, il est automatiquement affecté à toutes vos identités d’email, et vous en avez terminé ici. Si ce n’est pas votre seul canal de diffusion, passez à l’étape 5.

1. Pendant que vous êtes toujours dans Paramètres du courrier électronique, cliquez sur **Adresse et signature**.

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. Recherchez l&#39;identité email pour laquelle vous souhaitez choisir un canal de diffusion et cliquez sur **Choisir le canal de diffusion**.

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. Dans la carte de délivrabilité, cliquez sur **Modifier**.

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. Cliquez sur la liste déroulante Canal et sélectionnez le canal de diffusion personnalisé que vous venez d’ajouter. Cliquez sur **Enregistrer**.

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >Si l’administrateur de votre équipe configure le serveur SMTP d’équipe, il s’appliquera automatiquement uniquement à votre identité de messagerie par défaut et sera disponible en tant qu’option pour vos autres identités de messagerie.

## Serveur SMTP de l’équipe {#team-smtp-server}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Connectez-vous à l’ [application web](https://toutapp.com/login), cliquez sur l’icône en forme d’engrenage en haut à droite et sélectionnez **Paramètres**.

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. Sous Paramètres d’administration, cliquez sur **Général**.

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. Cliquez sur **Canal de diffusion de l’équipe**.

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. Saisissez vos informations d’identification SMTP Server et cliquez sur **Connect**.

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >Le serveur SMTP d’équipe sera le canal de diffusion par défaut de l’identité email par défaut pour tous les membres de l’équipe. En outre, il sera disponible en tant qu’option de canal de diffusion pour toutes les autres identités d’email.

   >[!MORELIKETHIS]
   >
   >* [Connexion par e-mail pour les utilisateurs de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >
   >* [Connexion par e-mail pour les utilisateurs d’Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
