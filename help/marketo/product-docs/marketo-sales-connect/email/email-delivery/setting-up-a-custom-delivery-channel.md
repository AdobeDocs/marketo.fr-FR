---
unique-page-id: 14746470
description: Configuration d’un Canal de Diffusion personnalisé - Documents marketing - Documentation du produit
title: Configuration d’un Canal de Diffusion personnalisé
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# Configuration d’un Canal de Diffusion personnalisé {#setting-up-a-custom-delivery-channel}

Marketo Sales Connect vous permet de vous intégrer à un serveur SMTP personnalisé pour la diffusion de vos e-mails. C&#39;est une option idéale pour ceux qui ne veulent pas envoyer des e-mails en vrac à partir de leur canal Gmail ou Exchange diffusion.

Les utilisateurs peuvent configurer un serveur SMTP personnalisé pour leur propre utilisation, ou les administrateurs peuvent configurer un serveur SMTP d&#39;équipe à partager entre tous les utilisateurs de Sales Connect de votre instance.

>[!NOTE]
>
>* Outre la configuration de votre serveur SMTP, votre [identité de courriel doit être vérifiée](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) avant de pouvoir envoyer des courriers électroniques.
>* Nous vous recommandons de travailler avec votre équipe informatique ou votre fournisseur de serveur SMTP pour obtenir les informations d’identification de serveur appropriées pour votre serveur SMTP.
>* Vous ne pouvez pas connecter votre serveur Gmail et Exchange à l’aide des informations d’identification du serveur SMTP. Utilisez notre service Email Connection pour vous intégrer à ces fournisseurs.


## SMTP personnalisé {#custom-smtp}

1. Connectez-vous à l’[application Web](https://toutapp.com/login), cliquez sur l’icône en forme d’engrenage en haut à droite et choisissez **Paramètres**.

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. Sous Mon compte, cliquez sur **Paramètres de courriel**.

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. Cliquez sur **Canal de Diffusion personnalisé**.

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. Saisissez vos informations d’identification de serveur SMTP et cliquez sur **Se connecter**.

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >S&#39;il s&#39;agit de votre seul canal de diffusion, il est automatiquement affecté à toutes vos identités de messagerie, et vous avez terminé ici. Si ce n&#39;est pas votre seul canal de diffusion, veuillez continuer à l&#39;étape 5.

1. Toujours dans Paramètres de courrier électronique, cliquez sur **Adresse et signature**.

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. Recherchez l’identité électronique pour laquelle vous souhaitez choisir un canal de diffusion et cliquez sur **Choisir le Canal de Diffusion**.

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. Dans la carte de délivrabilité, cliquez sur **Modifier**.

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. Cliquez sur la liste déroulante Canal et choisissez le canal de diffusion personnalisé que vous venez d’ajouter. Cliquez sur **Enregistrer**.

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >Si l&#39;administrateur de votre équipe configure le serveur SMTP d&#39;équipe, il s&#39;appliquera automatiquement uniquement à votre identité de messagerie par défaut et sera disponible en tant qu&#39;option pour vos autres identités de messagerie.

## Team SMTP Server {#team-smtp-server}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Connectez-vous à l’[application Web](https://toutapp.com/login), cliquez sur l’icône en forme d’engrenage en haut à droite et choisissez **Paramètres**.

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. Sous Paramètres d’administration, cliquez sur **Général**.

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. Cliquez sur **Canal de Diffusion d&#39;équipe**.

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. Saisissez vos informations d’identification de serveur SMTP et cliquez sur **Se connecter**.

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >Le serveur SMTP d&#39;équipe sera le canal de diffusion par défaut de l&#39;identité de courriel par défaut pour tous les membres de l&#39;équipe. De plus, il sera disponible en tant qu’option de canal de diffusion pour toutes les autres identités de courriel.

   >[!MORELIKETHIS]
   >
   >* [Connexion par courriel pour les utilisateurs de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
      >
      >
   * [Connexion par courriel pour les utilisateurs d&#39;Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

