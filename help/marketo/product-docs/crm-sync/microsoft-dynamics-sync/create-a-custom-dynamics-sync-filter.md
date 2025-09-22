---
unique-page-id: 9437903
description: Création d’un filtre  [!DNL Dynamics]  synchronisation personnalisé - Documents Marketo - Documentation du produit
title: Création d’un filtre  [!DNL Dynamics]  synchronisation personnalisé
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 1%

---

# Créer un filtre de synchronisation de [!DNL Dynamics] personnalisé {#create-a-custom-dynamics-sync-filter}

Marketo vous permet de configurer un filtre de synchronisation et de synchroniser uniquement une partie de vos enregistrements.

## Vue d’ensemble {#overview}

Pour configurer un filtre de synchronisation [!DNL Dynamics] :

1. Créez un champ personnalisé à deux options (booléen) nommé `new_synctomkto` dans votre CRM Dynamics pour tout objet (prospect, contact, compte, opportunité et autres entités personnalisées).
1. Affectez une valeur Oui/Non à ce champ.

Vous devez effectuer ces modifications dans Dynamics CRM, et non dans votre base de données ou Marketo.

>[!CAUTION]
>
>Si vous n’affectez pas le champ et le laissez vide/nul, il se synchronise mais ne se met pas à jour. Les enregistrements dont la valeur de champ est vide/NULL dans Dynamics CRM afficheront cette valeur de champ dans Marketo avec la mention « false ».

Marketo recherche ce champ lors de la synchronisation automatique en arrière-plan et détermine les enregistrements à synchroniser en fonction de cette logique :

| Valeur du champ | Synchroniser avec Marketo ? |
|---|---|
| Le champ n’existe pas | Oui |
| Le champ est vide | Oui |
| Le champ a la valeur Oui | Oui |
| Le champ a la valeur Non | Non |

>[!CAUTION]
>
>La seule façon de dire à Marketo d’ignorer un enregistrement est de définir explicitement la valeur du champ sur **Non**. Marketo synchronise toujours les enregistrements même si les valeurs des champs sont vides.

>[!PREREQUISITES]
>
>Installez la dernière version du plug-in Marketo (3.0.0.1 ou ultérieure). Accédez à Marketo > [!UICONTROL Admin] > [!DNL Microsoft Dynamics] > [!UICONTROL Télécharger la solution Marketo].

## Créer un champ SyncToMoto {#create-synctomkto-field}

1. Connectez-vous à votre Dynamics CRM. Cliquez sur **Paramètres**, puis sur **Personnalisations**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Cliquez sur **[!UICONTROL Personnaliser le système]**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Cliquez sur ![](assets/image2015-8-10-21-3a44-3a23.png) en regard de **[!UICONTROL Entités]**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Cliquez sur ![](assets/image2015-8-10-21-3a44-3a23.png) en regard de **[!UICONTROL Lead]** et sélectionnez **[!UICONTROL Champs]**. Cliquez ensuite sur **[!UICONTROL Nouveau]**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Saisissez **SyncToMkto** dans le champ **[!UICONTROL Nom d’affichage]** et sélectionnez **[!UICONTROL Deux options]** comme **[!UICONTROL Type de données]**. Cliquez ensuite sur **[!UICONTROL Enregistrer et fermer]**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Choisissez un nom d&#39;affichage pour ce champ, mais le champ Nom doit être exactement **new_synctomkto**. Vous devez utiliser **new** comme préfixe par défaut. Si vous avez modifié la valeur par défaut, rendez-vous ici pour [réinitialiser le préfixe par défaut pour les noms de champ personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}. Vous pouvez la modifier une fois les nouveaux champs créés.

   >[!NOTE]
   >
   >Si vous avez configuré un workflow asynchrone, l’enregistrement obtient la valeur SyncToMoto par défaut que vous avez configurée dans le champ et obtient la valeur correcte quelques secondes plus tard, lorsque le workflow se termine. Si la valeur par défaut est définie sur Oui, ces enregistrements seront créés dans Marketo, puis deviendront obsolètes. Utilisez **Non** comme valeur par défaut pour éviter cette situation.

1. Répétez ce processus et créez le champ **SyncToMkto** pour toutes les autres entités sur lesquelles vous souhaitez limiter la synchronisation, telles que les entités de contact, de compte, d’opportunité et personnalisées.

## Sélection du filtre dans Marketo {#select-the-filter-in-marketo}

Même si vous avez déjà effectué votre synchronisation initiale, accédez à et sélectionnez les champs à synchroniser avec Marketo.

1. Accédez à Admin et sélectionnez **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **[!UICONTROL Modifier]** dans Détails de synchronisation des champs.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto mais le Nom d&#39;affichage peut être n&#39;importe quoi. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Très bien. Vous avez maintenant activé le filtre de synchronisation pour Marketo.

## Créer un workflow [!DNL Dynamics] pour affecter automatiquement des valeurs de filtre de synchronisation {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Vous pouvez toujours attribuer manuellement une valeur aux champs SyncToMoto pour vos enregistrements. Mais pourquoi ne pas tirer parti de la puissance d’un workflow [!DNL Dynamics] et attribuer automatiquement une valeur au champ SyncToMkto lorsqu’un enregistrement est créé ou mis à jour ?

>[!NOTE]
>
>Vous ne pouvez pas effectuer cette opération au niveau de la base de données. Elle doit être effectuée manuellement dans le CRM ou à l’aide d’un workflow.
>
>Un workflow [!DNL Dynamics] fonctionne uniquement sur les nouveaux enregistrements créés à l’avenir, et non sur les données historiques. Utiliser une mise à jour par lots pour déplacer les enregistrements existants.

1. Accédez à votre Dynamics CRM. Cliquez sur **Paramètres**, puis **Processus**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Cliquez sur **[!UICONTROL Nouveau]**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Saisissez un nom pour le workflow et sélectionnez **[!UICONTROL Workflow]** comme [!UICONTROL Catégorie] et **[!UICONTROL Lead]** comme [!UICONTROL Entité]. Cliquez ensuite sur **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Créez des règles pour attribuer une valeur true ou false au champ **SyncToMkto** en fonction des préférences de votre organisation. Cliquez sur **[!UICONTROL Enregistrer et fermer]**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Définissez une action par défaut après avoir cliqué sur **[!UICONTROL Ajouter une étape]** pour ajouter une condition de vérification. Cela définit les enregistrements que vous ne souhaitez pas synchroniser sur **Non**. Sinon, ils se synchroniseront.

1. Sélectionnez le workflow et cliquez sur **[!UICONTROL Activer]**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Consultez la section [Règles de filtre de synchronisation personnalisées pour une adresse e-mail](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"} pour configurer des règles afin de synchroniser uniquement les enregistrements pour les personnes disposant d’adresses e-mail.

## Détails du filtre de synchronisation {#sync-filter-details}

Voici quelques détails d’implémentation que vous devriez connaître :

* Démarrer une opération de synchronisation

  Lorsque la valeur **SyncToMkto** passe de **Non** à **Oui**, [!DNL Dynamics] avertit immédiatement Marketo pour commencer à synchroniser cet enregistrement. Si l’enregistrement existe déjà, Marketo le met à jour. Sinon, Marketo crée l’enregistrement.

* Arrêt d’une opération de synchronisation

  Lorsqu&#39;un enregistrement change sa valeur SyncToMkto de Yes en No, Marketo est averti pour arrêter la synchronisation de cet enregistrement. Cependant, l’enregistrement n’est pas supprimé, mais il cesse d’être mis à jour et devient obsolète.

>[!MORELIKETHIS]
>
>* [Filtre de synchronisation Microsoft Dynamics : qualifier](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Filtre de synchronisation Microsoft Dynamics : fusion](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [Règles de filtre de synchronisation personnalisé pour une adresse e-mail](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}
