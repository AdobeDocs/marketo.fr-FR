---
description: Reconfigurez la méthode d’authentification Dynamics - Documents Marketo - Documentation du produit
title: Reconfiguration de la méthode d’authentification Dynamics
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
source-git-commit: ab20d9683aa5987778970fd32793dc0f3056c84b
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Reconfiguration de la méthode d’authentification Dynamics {#reconfigure-dynamics-authentication-method}

Suivez les étapes ci-dessous pour mettre à jour votre méthode d’authentification Dynamics.

>[!PREREQUISITES]
>
>Configurez l’application dans Microsoft Dynamics et dans le répertoire principal (Azure AD/ADFS) à l’aide de la méthode d’authentification souhaitée dans l’un des articles suivants :
>
>* [Étape 2 sur 3 : Configuration de la solution Marketo avec connexion serveur à serveur](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)
>* [Étape 2 sur 4 : Configuration de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire des ressources](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)


1. Dans Marketo click **Administration**.

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. Cliquez sur **Microsoft Dynamics**, puis **Désactiver la synchronisation**.

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >Vous devez désactiver temporairement la synchronisation globale pour mettre à jour la méthode d’authentification.

1. Cliquez sur le bouton **Reconfigurez la nouvelle méthode d’authentification** .

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. Sélectionnez la nouvelle méthode d’authentification souhaitée (dans cet exemple, nous choisissons l’API Web).

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. Saisissez les informations d’identification requises pour la nouvelle méthode d’authentification, puis cliquez sur **Valider**.

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* Les champs spécifiques varient selon la méthode d&#39;authentification choisie et le formulaire est automatiquement mis à jour en fonction de la méthode d&#39;authentification précédente.
   >* Si vous avez déjà synchronisé , les données du formulaire ci-dessus peuvent être préremplies. Saisissez à nouveau toutes les informations d’identification pour vous assurer que les valeurs sont correctes.


1. Si tout va bien, la synchronisation des validations génère toutes les coches vertes. ![](assets/green-check.png). Vérifiez le message, puis cliquez sur **Basculer** pour mettre à jour la méthode d’authentification.

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >Si une ![](assets/red-x.png), cette étape présente un problème. Voir [Correction des problèmes de synchronisation de validation de Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) pour identifier et résoudre le ou les problèmes. Exécutez à nouveau les étapes de validation de la synchronisation jusqu’à ce que le résultat ressemble à l’image ci-dessus.

1. Cliquez sur **Confirmer** pour continuer.

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. Cliquez sur **Confirmer** encore une fois.

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. Cliquez sur **OK**.

   >[!IMPORTANT]
   >
   >Le système prend 15 minutes pour accepter le nouveau mode d’authentification. Veuillez patienter 15 minutes à compter de l’heure du commutateur avant de réactiver la synchronisation.