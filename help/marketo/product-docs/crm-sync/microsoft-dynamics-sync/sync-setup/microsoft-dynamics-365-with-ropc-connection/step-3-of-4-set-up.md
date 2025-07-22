---
description: Étape 3 sur 4 - Configuration de l’application cliente sur MS [!DNL Dynamics] - Documents Marketo - Documentation du produit
title: Étape 3 sur 4 - Configurer l’application cliente sur MS [!DNL Dynamics]
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Étape 3 sur 4 : configurer l’application cliente sur MS [!DNL Dynamics] {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Étape 1 de 4 : installer la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [Étape 2 de 4 : configurer la solution Marketo avec une connexion de contrôle de mot de passe du propriétaire de la ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. Accédez à cet article [Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Suivez toutes les étapes. Pour l&#39;étape 3, entrez un nom d&#39;application approprié (p. ex. « [!DNL Marketo Integration] »). Sous Types de compte pris en charge, sélectionnez Compte dans cet annuaire organisationnel uniquement.

1. Notez l’ID d’application (ClientId). Vous devrez le saisir dans Marketo ultérieurement.

1. Accordez le consentement administrateur en suivant les étapes décrites dans [cet article](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Générez un secret client dans Admin Center en cliquant sur **[!UICONTROL Certificats et secrets]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Cliquez sur **[!UICONTROL Nouveau secret client]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Ajoutez une description du secret client et cliquez sur **[!UICONTROL Ajouter]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Veillez à prendre note de la valeur Secret client (affichée dans la capture d’écran ci-dessous), car vous en aurez besoin ultérieurement. Il n’est affiché qu’une seule fois et vous ne pourrez plus le récupérer.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## [!DNL Azure AD] Federated avec [!DNL AD FS On-prem] {#azure-ad-federated-with-ad-fs-on-prem}

Federated [!DNL Azure] AD to [!DNL ADFS Onprem] nécessite la création d’une politique de découverte de domaine d’accueil pour l’application spécifique. Avec cette politique, [!DNL Azure] Active Directory redirigera la demande d&#39;authentification vers le service de fédération. Pour cela, la synchronisation de hachage de mot de passe doit être activée dans [!DNL AD Connect]. Pour plus d’informations, consultez les sections [[!DNL OAuth] avec [!DNL ROPC]](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) et [Définir une politique Hrd pour une application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Des références supplémentaires [ici](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&text=This%20report%20includes%20includes%20federated,are%20federated%20to%20Azure%20AD.){target="_blank"} sont disponibles.

## Avant de passer à l’étape 4 {#before-proceeding-to-step-4}

* Si vous souhaitez limiter le nombre d’enregistrements synchronisés, [configurez un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) maintenant.
* Exécutez le processus [Validate [!DNL Microsoft Dynamics] Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Il vérifie que vos configurations initiales ont été correctement effectuées.
* Connectez-vous à l’utilisateur de synchronisation Marketo dans [!DNL Microsoft Dynamics] CRM.

>[!MORELIKETHIS]
>
>* [Étape 4 de 4 : connecter la solution Marketo à la connexion de contrôle de mot de passe du propriétaire de la ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md){target="_blank"}
