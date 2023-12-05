---
unique-page-id: 9437903
description: Créer un filtre de synchronisation Dynamics personnalisé - Documents Marketo - Documentation du produit
title: Création d’un filtre de synchronisation Dynamics personnalisé
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 1%

---

# Création d’un filtre de synchronisation Dynamics personnalisé {#create-a-custom-dynamics-sync-filter}

Ne souhaitez-vous pas tout synchroniser dans Marketo Engage dans votre CRM Dynamics ? Ne vous inquiétez pas ! Marketo vous permet de configurer un filtre de synchronisation et de synchronisation uniquement une partie de vos enregistrements.

## Vue d’ensemble {#overview}

Pour configurer un filtre de synchronisation Dynamics :

1. Créez un champ personnalisé Deux options (booléen) nommé new_synctomkto dans votre CRM Dynamics pour tout objet (prospect, contact, compte, opportunité et autres entités personnalisées).
1. Attribuez à ce champ une valeur Oui/Non.

Vous devez effectuer ces modifications dans Dynamics CRM, et non dans votre base de données ou votre Marketo.

>[!CAUTION]
>
>Si vous n’affectez pas le champ et laissez-le vide/NULL, il se synchronise mais ne se met pas à jour. Les enregistrements avec une valeur de champ vide/NULL dans Dynamics CRM afficheront cette valeur de champ dans Marketo comme &quot;false&quot;.

Marketo recherche ce champ lors de la synchronisation automatique en arrière-plan et détermine les enregistrements à synchroniser en fonction de cette logique :

| Valeur du champ | Synchroniser avec Marketo ? |
|---|---|
| Le champ n’existe pas | Oui |
| Le champ est vide | Oui |
| Le champ a la valeur Oui | Oui |
| Le champ a la valeur Non | Non |

>[!CAUTION]
>
>La seule façon de demander à Marketo d’ignorer un enregistrement consiste à définir explicitement la valeur du champ sur **Non**. Marketo synchronise toujours les enregistrements même si les valeurs de champ sont vides.

>[!PREREQUISITES]
>
>Installez la dernière version du module externe Marketo (3.0.0.1 ou version ultérieure). Accédez à Marketo > Admin > Microsoft Dynamics > Télécharger la solution Marketo.

## Créer un champ SyncToMkto {#create-synctomkto-field}

1. Connectez-vous à Dynamics CRM. Cliquez sur **Paramètres**, puis cliquez sur **Personnalisations**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Cliquez sur **Personnalisation du système**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Cliquez sur ![](assets/image2015-8-10-21-3a44-3a23.png) en regard de **Entités**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Cliquez sur ![](assets/image2015-8-10-21-3a44-3a23.png) en regard de **prospect** et sélectionnez **Champs**. Cliquez ensuite sur **Nouveau**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Entrée **SyncToMkto** dans le **Nom d’affichage** champ et sélectionnez **Deux options** comme la propriété **Type de données**. Cliquez ensuite sur **Enregistrer et fermer**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Choisissez n’importe quel nom d’affichage pour ce champ, mais le champ Nom doit être exactement **new_synctomkto**. Vous devez utiliser **new** comme préfixe par défaut. Si vous avez modifié la valeur par défaut, accédez à [réinitialisation du préfixe par défaut pour les noms de champ personnalisés](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}. Vous pouvez la modifier à nouveau une fois les nouveaux champs créés.

   >[!NOTE]
   >
   >Si un workflow asynchrone est configuré, l’enregistrement récupère la valeur SyncToMkto par défaut que vous avez configurée dans le champ et obtient la valeur correcte quelques secondes plus tard lorsque le workflow se termine. Si la valeur par défaut est Oui, ces enregistrements seront créés dans Marketo, puis deviennent obsolètes. Utilisation **Non** comme valeur par défaut pour éviter cela.

1. Répétez cette opération et créez le **SyncToMkto** pour toutes les autres entités sur lesquelles vous souhaitez limiter la synchronisation, telles que les entités de contact, de compte, d’opportunité et personnalisées.

## Sélection du filtre dans Marketo {#select-the-filter-in-marketo}

Même si vous avez déjà effectué votre synchronisation initiale, accédez à et sélectionnez les champs à synchroniser avec Marketo.

1. Accédez à Admin et sélectionnez **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **[!UICONTROL Modifier]** sur Détails de synchronisation du champ.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Faites défiler l’écran jusqu’au champ et cochez-le. Le nom réel doit être new_synctomkto, mais le nom d’affichage peut être de n’importe quel type. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Parfait, vous avez maintenant activé le filtre de synchronisation pour Marketo.

## Créer un workflow Dynamics pour attribuer automatiquement des valeurs de filtre de synchronisation {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Vous pouvez toujours attribuer manuellement une valeur aux champs SyncToMkto pour vos enregistrements. Mais pourquoi ne pas tirer parti de la puissance d’un workflow Dynamics et attribuer automatiquement une valeur au champ SyncToMkto lorsqu’un enregistrement est créé ou mis à jour ?

>[!NOTE]
>
>Vous ne pouvez pas le faire au niveau de la base de données. Cela doit être effectué dans le CRM manuellement ou à l&#39;aide d&#39;un workflow.
>
>Un workflow Dynamics fonctionne uniquement sur les nouveaux enregistrements créés à l’avenir, et non sur les données historiques. Utilisez une mise à jour par lots pour vous déplacer sur les enregistrements existants.

1. Accédez à votre Dynamics CRM. Cliquez sur **Paramètres**, puis **Processus**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Cliquez sur **Nouveau**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Saisissez le nom du workflow, puis sélectionnez **Workflow** comme catégorie et **prospect** comme entité. Cliquez ensuite sur **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Créez des règles pour affecter une valeur true ou false à la variable **SyncToMkto** champ en fonction des préférences de votre organisation. Cliquez sur **Enregistrer et fermer**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Définissez une action par défaut après avoir cliqué sur **Ajouter une étape** pour ajouter une condition de vérification. Cette opération définit les enregistrements auxquels vous ne souhaitez pas effectuer de synchronisation. **Non**. Sinon, ils se synchroniseront.

1. Sélectionnez le workflow, puis cliquez sur **Activer**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Voir [Règles de filtre de synchronisation personnalisées pour une adresse électronique](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"} pour configurer des règles afin de synchroniser uniquement les enregistrements pour les personnes ayant des adresses électroniques.

## Détails du filtre de synchronisation {#sync-filter-details}

Voici quelques détails de mise en oeuvre que nous pensions savoir :

* Démarrer une opération de synchronisation

  Lorsque la variable **SyncToMkto** change de valeur à partir de **Non** to **Oui**, Dynamics avertit immédiatement Marketo de commencer la synchronisation de cet enregistrement. Si l’enregistrement existe déjà, Marketo le met à jour. Sinon, Marketo crée l’enregistrement.

  >[!TIP]
  >
  >A `Create [StartSync]` est ajoutée au journal Marketo lorsque cela se produit.

* Arrêt d’une opération de synchronisation

  Lorsqu’un enregistrement change sa valeur SyncToMkto de Oui à Non, Marketo est averti de l’arrêt de la synchronisation de cet enregistrement. Cependant, l’enregistrement n’est pas supprimé, mais il cesse d’être mis à jour et devient obsolète.

>[!MORELIKETHIS]
>
>* [Filtre de synchronisation Microsoft Dynamics : admissible](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Filtre de synchronisation Microsoft Dynamics : Fusion](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [Règles de filtre de synchronisation personnalisées pour une adresse électronique](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}
