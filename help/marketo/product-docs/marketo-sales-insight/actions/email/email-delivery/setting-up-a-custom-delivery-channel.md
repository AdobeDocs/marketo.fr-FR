---
description: Configuration d’un canal de diffusion personnalisé - Documents Marketo - Documentation du produit
title: Configuration d’un canal de diffusion personnalisé
hide: true
hidefromtoc: true
source-git-commit: 55afdc537d0a5d0b6114f478c4dd2ded09c84e34
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Configuration d’un canal de diffusion personnalisé {#setting-up-a-custom-delivery-channel}

Marketo Sales Connect vous permet de vous intégrer à un serveur SMTP personnalisé pour la diffusion de vos emails. Il s’agit d’une excellente option pour ceux qui ne souhaitent pas envoyer des emails en bloc depuis leur canal de diffusion Gmail ou Exchange.

Les utilisateurs peuvent configurer un serveur SMTP personnalisé pour leur propre utilisation, ou les administrateurs peuvent configurer un serveur SMTP d’équipe à partager avec tous les utilisateurs de Sales Connect de votre instance.

>[!NOTE]
>
>* Outre la configuration de votre serveur SMTP, votre [l&#39;identité de l&#39;email doit être vérifiée](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) avant de pouvoir envoyer des emails.
>* Nous vous recommandons de travailler avec votre équipe informatique ou votre fournisseur de serveur SMTP pour obtenir les informations d’identification de serveur appropriées pour votre serveur SMTP.
>* Vous ne pouvez pas connecter votre serveur Gmail et Exchange à l’aide des informations d’identification du serveur SMTP. Utilisez notre service Email Connection pour vous intégrer à ces fournisseurs.


## SMTP personnalisé {#custom-smtp}

1. Connectez-vous au [application web](https://toutapp.com/login), cliquez sur l’icône d’engrenage en haut à droite et choisissez **Paramètres**.

PICC

1. Sous Mon compte, cliquez sur **Paramètres de messagerie électronique**.

PICC

1. Cliquez sur **Canal de diffusion personnalisé**.

PICC

1. Saisissez vos informations d’identification SMTP Server, puis cliquez sur **Connexion**.

PICC

>[!NOTE]
>
>S’il s’agit de votre seul canal de diffusion, il est automatiquement affecté à toutes vos identités d’email, et vous en avez terminé ici. Si ce n’est pas votre seul canal de diffusion, passez à l’étape 5.

1. Pendant que vous êtes toujours dans Paramètres du courrier électronique, cliquez sur **Adresse et signature**.

PICC

1. Recherchez l&#39;identité email pour laquelle vous souhaitez choisir un canal de diffusion et cliquez sur **Choisir le canal de diffusion**.

PICC

1. Dans la carte de délivrabilité, cliquez sur **Modifier**.

PICC

1. Cliquez sur la liste déroulante Canal et sélectionnez le canal de diffusion personnalisé que vous venez d’ajouter. Cliquez sur **Enregistrer**.

PICC

>[!NOTE]
>
>Si l’administrateur de votre équipe configure le serveur SMTP d’équipe, il s’appliquera automatiquement uniquement à votre identité de messagerie par défaut et sera disponible en tant qu’option pour vos autres identités de messagerie.

## Serveur SMTP de l’équipe {#team-smtp-server}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Connectez-vous au [application web](https://toutapp.com/login), cliquez sur l’icône d’engrenage en haut à droite et choisissez **Paramètres**.

PICC

1. Sous Paramètres d’administration, cliquez sur **Général**.

PICC

1. Cliquez sur **Canal de diffusion de l’équipe**.

PICC

1. Saisissez vos informations d’identification SMTP Server, puis cliquez sur **Connexion**.

PICC

>[!NOTE]
>
>Le serveur SMTP d’équipe sera le canal de diffusion par défaut de l’identité email par défaut pour tous les membres de l’équipe. En outre, il sera disponible en tant qu’option de canal de diffusion pour toutes les autres identités d’email.

>[!MORELIKETHIS]
>
>* [Connexion par e-mail pour les utilisateurs de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connexion par e-mail pour les utilisateurs Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

