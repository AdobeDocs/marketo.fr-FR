---
description: Reconfiguration [!DNL Dynamics] Méthode d’authentification - Documents Marketo - Documentation du produit
title: Reconfigure [!DNL Dynamics] Authentication Method
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 2%

---

# Reconfigurer la méthode d’authentification Dynamics {#reconfigure-dynamics-authentication-method}

Suivez les étapes ci-dessous pour mettre à jour votre méthode d’authentification [!DNL Dynamics].

>[!PREREQUISITES]
>
>Configurez l’application dans [!DNL Microsoft Dynamics] et Active Directory (Azure AD/ADFS) à l’aide de la méthode d’authentification souhaitée à partir de l’un des articles suivants :
>
>* [Étape 2 de 3 : configurer la solution Marketo avec une connexion serveur à serveur](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}
>* [Étape 2 de 4 : configurer la solution Marketo avec une connexion de contrôle de mot de passe du propriétaire de la ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. Cliquez sur **Microsoft Dynamics** puis **[!UICONTROL Désactiver la synchronisation]**.

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >Vous devez désactiver temporairement la synchronisation globale pour mettre à jour la méthode d’authentification.

1. Cliquez sur l’onglet **[!UICONTROL Reconfigurer la nouvelle méthode d’authentification]**.

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. Sélectionnez la nouvelle méthode d’authentification souhaitée (dans cet exemple, nous choisissons API Web).

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. Saisissez les informations d’identification requises pour la nouvelle méthode d’authentification et cliquez sur **[!UICONTROL Valider]**.

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* Les champs spécifiques varient selon la méthode d’authentification choisie et le formulaire est automatiquement mis à jour en fonction de la méthode d’authentification précédente.
   >* Si vous avez déjà effectué une synchronisation, les données du formulaire ci-dessus peuvent être pré-renseignées. Saisissez à nouveau toutes les informations d’identification pour vous assurer que les valeurs sont correctes.

1. Si tout est correct, la synchronisation de validation génère toutes les coches vertes ![](assets/green-check.png). Vérifiez le message et cliquez sur **[!UICONTROL Basculer]** pour mettre à jour la méthode d’authentification.

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >Si vous voyez une ![](assets/red-x.png), cette étape présente un problème. Voir [Correction [!DNL Dynamics] des problèmes de synchronisation de validation](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) pour identifier et résoudre le ou les problèmes. Réexécutez ensuite les étapes de validation de la synchronisation jusqu’à ce que le résultat ressemble à l’image ci-dessus.

1. Cliquez sur **[!UICONTROL Confirmer]** pour continuer.

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. Cliquez de nouveau sur **[!UICONTROL Confirmer]**.

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. Cliquez sur **[!UICONTROL OK]**.

   >[!IMPORTANT]
   >
   >Le système prend 15 minutes pour accepter le nouveau mode d’authentification. Patientez 15 minutes à partir de l’heure du changement avant de réactiver la synchronisation.
