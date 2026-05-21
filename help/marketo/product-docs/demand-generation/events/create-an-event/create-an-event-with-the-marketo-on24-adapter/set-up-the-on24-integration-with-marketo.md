---
description: Découvrez comment configurer l’intégration ON24 avec Marketo. Connectez votre compte ON24 afin de synchroniser les webinaires et les données d’enregistrement.
title: Configurer l’intégration d’ON24 à Marketo
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
TQID: https://experienceleague.adobe.com/qIKnrBwavLmy7tBqPTLvz72AJNIiVRzoEKQtH0OVgWg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 299
ht-degree: 7%

---

# Configurer l’intégration d’ON24 à Marketo{#set-up-the-on24-integration-with-marketo}

Pour configurer votre intégration d’événement ON24, procédez comme suit.

## Créer un rôle API uniquement {#create-an-api-only-role}

1. Dans Mon Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. Sous [!UICONTROL Sécurité], cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Rôles]** puis sur **[!UICONTROL Nouveau rôle]**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. Saisissez un [!UICONTROL Nom du rôle]. Ouvrez le menu **[!UICONTROL API Access]** et sélectionnez « [!UICONTROL Objet personnalisé en lecture-écriture] » et « [!UICONTROL Personne en lecture-écriture] ». Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## Créer un nouvel utilisateur {#create-a-new-user}

1. Toujours en [!UICONTROL Utilisateurs et rôles], cliquez sur l’onglet **[!UICONTROL Utilisateurs]** et cliquez sur **[!UICONTROL Inviter un nouvel utilisateur]**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. Saisissez les informations du nouvel utilisateur et cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. Sélectionnez le rôle [!UICONTROL API ON24 uniquement (tous les espaces de travail)] que vous avez créé. Cochez la case **[!UICONTROL API uniquement]**. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. Cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>Aucune invitation n’est requise pour les utilisateurs et utilisatrices de l’API uniquement.

## Configurer la connexion ON24 {#set-up-on24-connection}

1. Toujours dans la section [!UICONTROL Admin], cliquez sur **[!UICONTROL LaunchPoint]**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. Cliquez sur **[!UICONTROL Nouveau]** puis **[!UICONTROL Nouveau service]**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. Choisissez un [!UICONTROL nom d’affichage]. Cliquez sur la liste déroulante **[!UICONTROL Service]** et sélectionnez **[!UICONTROL Personnalisé]**. Saisissez une [!UICONTROL description]. Cliquez sur le menu déroulant [!UICONTROL Utilisateur API uniquement] et sélectionnez l’utilisateur que vous avez créé [dans les étapes ci-dessus](#create-a-new-user). Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. Recherchez le service [!DNL LaunchPoint] personnalisé que vous avez créé et cliquez sur [!UICONTROL Afficher les détails].

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. Mettez en surbrillance, cliquez avec le bouton droit, copiez et enregistrez l’[!UICONTROL ID client] (vous en aurez besoin ultérieurement). Répétez l’opération pour [!UICONTROL Secret client].

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. Dans l’arborescence de gauche, cliquez sur **[!UICONTROL Services web]**.

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. Sous « [!UICONTROL API REST] », mettez en surbrillance, cliquez avec le bouton droit de la souris, copiez et enregistrez la première partie de l’[!UICONTROL Identité] (jusqu’au « m » dans .com).

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. Avec votre ID client, votre secret client et votre identité enregistrés, accédez à votre compte ON24. Le reste des étapes y sont effectuées et se trouvent dans la documentation [ON24](https://support.on24.com/hc/en-us/articles/21420762650523-Data-Integration-Setup-Instructions-When-Using-Marketo-Registration-Option-1){target="_blank"}.
