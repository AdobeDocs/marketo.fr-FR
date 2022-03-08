---
description: Configuration des actions Sales Insight dans Salesforce - Documents Marketo - Documentation du produit
title: Configuration des actions d’aperçu des ventes dans Salesforce
hide: true
hidefromtoc: true
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: ba1357e6970ba4e3dc496d27272d067ac87c5e6d
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Configuration des actions d’aperçu des ventes dans Salesforce {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Installer](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) ou [Mettre à niveau](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Package Sales Insight dans votre instance Salesforce
>* [Configuration de Marketo Sales Insight dans Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)


## Ajouter un nouveau site distant dans Salesforce {#add-new-remote-site-in-salesforce}

1. Dans Salesforce, cliquez sur **Configuration**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Recherchez &quot;site distant&quot; et sélectionnez **Paramètres du site distant**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Cliquez sur **Nouveau site distant**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Saisissez le Nom du site distant (il peut s’agir de &quot;MarketoSalesInsight&quot;). Saisissez l’URL du site distant (https://ims-na1-stg1.adobelogin.com) et cliquez sur **Enregistrer**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

## Activation des actions Sales Insight dans le CRM {#enabling-sales-insight-actions-across-the-crm}

1. Dans Salesforce, cliquez sur l’icône **Configuration de Marketo Sales Insight** .

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Si vous ne voyez pas &quot;Marketo Sales Insight Config&quot; dans votre barre supérieure, cliquez sur le bouton **+** signez et recherchez-le sous Tous les onglets.

1. Sélectionnez la **Activation des actions MSI** .

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Saisissez la clé secrète de l’API.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Si vous ne disposez pas de votre clé de sécurité API, vous pouvez la trouver en suivant les étapes de la section [cet article](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Cliquez sur **Enregistrer** une fois terminé.

Cela activera automatiquement toutes les fonctionnalités des actions MSI décrites dans l’article Présentation des fonctionnalités .

>[!NOTE]
>
>Vous pouvez désactiver toutes les fonctions d’actions MSI en décochant simplement la case &quot;Activer les actions MSI&quot;.

## Gouvernance des MSI-Actions {#msi-actions-governance}

1. Vous pouvez désactiver l’onglet Campagnes de ventes et/ou Tâche dans la section à venir. Cela s’applique aux panneaux de prospect, de contact, de compte et d’opportunité.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Vous pouvez désactiver les actions MSI en décochant les fonctionnalités correspondantes sous les paramètres Actions .

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Les paramètres de gouvernance s’appliquent à tous les utilisateurs MSI.
