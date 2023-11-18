---
description: Étape 3 sur 4 - Configuration de l’application cliente sur MS Dynamics - Documents Marketo - Documentation du produit
title: Étape 3 sur 4 - Configuration de l’application cliente sur MS Dynamics
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Étape 3 sur 4 : configuration de l’application cliente sur MS Dynamics {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Étape 1 sur 4 : installation de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [Étape 2 sur 4 : configuration de la solution Marketo avec la connexion de contrôle de mot de passe du propriétaire de la ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. Accédez à [Article de Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Suivez toutes les étapes. Pour l’étape 3, saisissez un nom d’application approprié (par exemple, &quot;Intégration Marketo&quot;). Sous Types de compte pris en charge, sélectionnez Compte dans cet annuaire organisationnel uniquement.

1. Notez l’ID de l’application (ClientId). Vous devrez le saisir ultérieurement dans Marketo.

1. Octroyez le consentement de l’administrateur en suivant les étapes de la section [cet article](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Générez un secret client dans le Centre d’administration en cliquant sur **[!UICONTROL Certificats et secrets]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Cliquez sur **[!UICONTROL Nouveau secret client]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Ajoutez une description du secret client et cliquez sur **[!UICONTROL Ajouter]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Veillez à prendre note de la valeur Secret client (vue dans la capture d’écran ci-dessous), car vous en aurez besoin ultérieurement. Elle n’est affichée qu’une seule fois et vous ne pourrez plus la récupérer.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated avec AD FS On-premise {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD à ADFS Onprem nécessite la création d’une stratégie de détection des domaines domestiques pour l’application spécifique. Avec cette stratégie, Azure AD redirigera la demande d’authentification vers le service de fédération. Pour ce faire, la synchronisation du hachage de mot de passe doit être activée dans AD Connect. Pour plus d’informations, voir [OAuth avec ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} and [Set an hrd policy for an application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

Références supplémentaires [peut être consulté ici](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20else%20include%20federated,are%20federated%20to%20Azure%20AD.){target="_blank"}.

## Avant de passer à l’étape 4 {#before-proceeding-to-step-4}

* Si vous souhaitez limiter le nombre d&#39;enregistrements synchronisés, [configurer un filtre de synchronisation personnalisé](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} maintenant.
* Exécutez la variable [Validation de la synchronisation Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} processus. Il vérifie que vos premières configurations ont été effectuées correctement.
* Connectez-vous à l’utilisateur de synchronisation Marketo dans Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>* [Étape 4 sur 4 : Connexion de la solution Marketo à la connexion du contrôle de mot de passe du propriétaire de la ressource](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md){target="_blank"}
