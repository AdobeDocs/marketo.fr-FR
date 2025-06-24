---
description: Configuration de l’intégration ON24 avec Marketo - Documentation de Marketo - Documentation du produit
title: Configuration de l’intégration ON24 avec Marketo
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 3%

---

# Configuration de l’intégration ON24 avec Marketo{#set-up-the-on24-integration-with-marketo}

Voici comment configurer votre intégration d’événement ON24.

## Créer un rôle API uniquement {#create-an-api-only-role}

1. Dans Mon Marketo, cliquez sur **Admin**.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. Sous Sécurité, cliquez sur **Utilisateurs et rôles**.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. Cliquez sur l’onglet **Rôles** puis sur **Nouveau rôle**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. Saisissez un nom de rôle. Ouvrez le menu **API Access** et sélectionnez « Objet personnalisé en lecture-écriture » et « Personne en lecture-écriture ». Cliquez sur **Créer**.

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## Créer un nouvel utilisateur {#create-a-new-user}

1. Toujours dans Utilisateurs et rôles, cliquez sur l’onglet **Utilisateurs** puis sur **Inviter un nouvel utilisateur**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. Saisissez les informations du nouvel utilisateur et cliquez sur **Suivant**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. Sélectionnez le rôle API ON24 uniquement que vous venez de créer. Cochez la case **API uniquement**. Cliquez sur **Suivant**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. Cliquez sur **Envoyer**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>Aucune invitation n’est requise pour les utilisateurs d’API uniquement.

## Configurer la connexion ON24 {#set-up-on24-connection}

1. Toujours dans la section Admin, cliquez sur **LaunchPoint**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. Cliquez sur **Nouveau** puis **Nouveau service**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. Choisissez un nom d’affichage. Cliquez sur la liste déroulante **Service** et sélectionnez **Personnalisé**. Saisissez une description. Cliquez sur le menu déroulant Utilisateur API uniquement et sélectionnez l’utilisateur que vous avez créé [dans les étapes ci-dessus](#create-a-new-user). Cliquez sur **Créer**.

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. Recherchez le service LaunchPoint personnalisé que vous venez de créer et cliquez sur Afficher les détails.

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. Mettez en surbrillance, cliquez avec le bouton droit de la souris, copiez et enregistrez l’ID client (vous en aurez besoin ultérieurement). Répétez l’opération pour le secret client.

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. Dans l’arborescence de gauche, cliquez sur Services Web.

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. Sous « API REST », mettez en surbrillance, cliquez avec le bouton droit de la souris, copiez et enregistrez la première partie de l’identité (jusqu’au « m » dans .com).

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. Avec votre ID client, votre secret client et votre identité enregistrés, accédez à votre compte ON24. Le reste des étapes y sont effectuées et se trouvent dans la documentation [ON24](https://support.on24.com/hc/en-us/articles/21420762650523-Data-Integration-Setup-Instructions-When-Using-Marketo-Registration-Option-1){target="_blank"}.
