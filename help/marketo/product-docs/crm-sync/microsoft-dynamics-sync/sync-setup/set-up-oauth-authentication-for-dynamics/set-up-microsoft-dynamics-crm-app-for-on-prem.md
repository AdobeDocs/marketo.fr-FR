---
description: Configuration de l'application Microsoft Dynamics CRM pour On-prem - Marketo Docs - Documentation du produit
title: Configuration de l'application Microsoft Dynamics CRM pour On-Prem
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---


# Configuration de l&#39;application Microsoft Dynamics CRM pour On-prem {#set-up-microsoft-dynamics-crm-app-for-on-prem}

La configuration basée sur l&#39;ID client/la clé secrète client dans Marketo peut être effectuée pour On-prem avec AD FS (ver. 2016 ou version ultérieure). Pour les versions plus anciennes d&#39;On-prem, contactez l&#39;[Assistance marketing](https://nation.marketo.com/t5/Support/ct-p/Support) pour obtenir que la méthode d&#39;authentification soit modifiée afin de ne reposer que sur l&#39;ID utilisateur et le mot de passe.

## Configuration de l&#39;application Microsoft Dynamics CRM {#set-up-microsoft-dynamics-crm-app}

Suivez les étapes décrites dans [cet article Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later).

Lorsque vous avez terminé, l&#39;étape suivante consiste à **Entrer l&#39;ID client et le secret générés par Dynamics CRM dans Marketo**.

## Saisissez l&#39;ID client et le secret générés par Dynamics CRM dans Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

Les étapes suivantes s’appliquent aux versions en ligne et aux versions instantanées.

1. Dans Marketo, cliquez sur **Admin**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-1.png)

1. Cliquez sur **Microsoft Dynamics**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-2.png)

1. Cliquez sur **Désactiver la synchronisation**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-3.png)

1. En regard des informations d’identification, cliquez sur **Modifier**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-4.png)

1. Saisissez les **ID client** et **Secret client** que vous avez récupéré précédemment et appuyez sur **Enregistrer**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-5.png)

1. Cliquez sur **Valider la configuration de synchronisation**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-6.png)

1. Cliquez sur **Suivant**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-7.png)

1. Vous devriez voir toutes les coches vertes. Cliquez sur **Fermer**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-8.png)

   >[!NOTE]
   >
   >Si un X rouge apparaît parmi vos coches vertes, consultez [cet article](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) pour connaître les options de correction.

1. Cliquez sur **Activer la synchronisation**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-9.png)

Et c&#39;est tout !
