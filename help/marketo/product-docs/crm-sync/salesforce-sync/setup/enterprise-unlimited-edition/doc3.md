---
description: Découvrez comment connecter Marketo et Salesforce lors de l’étape finale Entreprise ou Illimité. Récupérez le jeton de sécurité de synchronisation des utilisateurs et définissez les informations d’identification dans Marketo Admin.
title: Étape 3 sur 3 - Connecter Marketo et Salesforce (Entreprise/Illimité)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 8%

---

# Étape 3 sur 3 : connecter Marketo et Salesforce (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

Dans cet article, vous allez configurer Marketo Engage pour qu’il se synchronise avec l’instance Salesforce configurée.

>[!PREREQUISITES]
>
>* [Étape 1 sur 3 : Ajouter des champs Marketo à Salesforce (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [Étape 2 sur 3 : création d’un utilisateur Salesforce pour Marketo (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}

## Récupérer le jeton de sécurité de l’utilisateur de synchronisation {#retrieve-sync-user-security-token}

>[!TIP]
>
>Si vous disposez déjà du jeton de sécurité, passez directement à Définition des informations d’identification de l’utilisateur de synchronisation et félicitations pour la préparation !

1. Connectez-vous à Salesforce avec l’utilisateur de synchronisation Marketo, cliquez sur le nom de l’utilisateur de synchronisation, puis sur **[!UICONTROL Mes paramètres]**.
