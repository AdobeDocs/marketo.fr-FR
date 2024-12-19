---
description: Étape 2 sur 3 - Création d’un utilisateur Salesforce pour Marketo (Entreprise/Illimité) - Documents Marketo - Documentation du produit
title: Étape 2 sur 3 - Création d’un utilisateur Salesforce pour Marketo (Entreprise/Illimité)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 2%

---

# Étape 2 sur 3 : création d’un utilisateur Salesforce pour Marketo (Entreprise/Illimité) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Ces étapes doivent être effectuées par un administrateur Salesforce

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : Ajouter des champs Marketo à Salesforce (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}

Dans cet article, vous allez configurer des autorisations d’utilisateur dans le profil Salesforce et créer un compte d’intégration Marketo-Salesforce.

## Création d’un profil {#create-a-profile}

1. Cliquez sur **[!UICONTROL Configurer]**.

   CAPTURE D’ÉCRAN

1. Saisissez « profiles » dans la barre de recherche de navigation, puis cliquez sur le lien Profils .

   CAPTURE D’ÉCRAN

1. Cliquez sur Nouveau profil.

   CAPTURE D’ÉCRAN

1. Sélectionnez Utilisateur standard, nommez le profil « Marketo-Salesforce Sync » et cliquez sur Enregistrer.

   CAPTURE D’ÉCRAN

## Définir les autorisations de profil {#set-profile-permissions}

1. Cliquez sur Modifier pour définir les autorisations de sécurité.

   CAPTURE D’ÉCRAN

1. Sous la section Autorisations administratives , assurez-vous que les cases suivantes sont cochées :

   * API activé
   * Modifier les modèles d&#39;HTML
   * Gérer les documents publics
   * Gérer les modèles publics

   >[!TIP]
   >
   >Veillez à cocher la case Le mot de passe n’expire jamais .

1. Sous la section Autorisations d’utilisateur générales , assurez-vous que les cases suivantes sont cochées :

   * Convertir les leads
   * Modifier les événements
   * Modifier tâches

1. Sous la section Autorisations d’objet standard , assurez-vous que les autorisations de lecture, de création, de modification et de suppression sont cochées pour :

   * Comptes
   * Campagnes
   * Contacts
   * Prospects
   * Opportunités

   >[!NOTE]
   >
   >Octroyez des autorisations pour les campagnes, si vous prévoyez d’utiliser la synchronisation de la campagne.

   CAPTURE D’ÉCRAN

1. Lorsque vous avez terminé, cliquez sur Enregistrer au bas de la page.

   CAPTURE D’ÉCRAN

## Définir les autorisations de champ {#set-field-permissions}

1. Discutez avec vos spécialistes du marketing pour savoir quels champs personnalisés sont nécessaires à la synchronisation.

   >[!NOTE]
   >
   >Cette étape permet d’éviter l’affichage des champs dont vous n’avez pas besoin dans Marketo, ce qui réduit l’encombrement et accélère la synchronisation.

1. Dans la page des détails du profil, accédez à la section Sécurité au niveau du champ . Cliquez sur Affichage pour modifier l’accessibilité des objets :

   * Lead
   * Contact
   * Compte
   * Opportunité

   >[!TIP]
   >
   >Vous pouvez configurer d’autres objets en fonction des besoins de votre entreprise.

1. Pour chaque objet, cliquez sur Modifier.

   CAPTURE D’ÉCRAN

1. Recherchez les champs inutiles et assurez-vous que les options Accès en lecture et Accès en modification ne sont pas cochées. Cliquez sur Enregistrer lorsque vous avez terminé.

   >[!NOTE]
   >
   >Ne modifiez que l’accessibilité des champs personnalisés.

   CAPTURE D’ÉCRAN

1. Une fois que vous avez désactivé tous les champs inutiles, vous devez vérifier l&#39;accès en lecture et l&#39;accès en modification pour les champs d&#39;objet suivants. Cliquez sur Enregistrer lorsque vous avez terminé.

   TABLEAU

   CAPTURE D’ÉCRAN

## Créer un compte de synchronisation Marketo-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Créez un compte Salesforce dédié (par exemple, `marketo@yourcompany.com`) pour distinguer les modifications apportées par Marketo des autres utilisateurs de Salesforce.

1. Saisissez « Gérer les utilisateurs » dans la barre de recherche de navigation, puis cliquez sur Utilisateurs. Cliquez sur Nouvel utilisateur.

   CAPTURE D’ÉCRAN

   CAPTURE D’ÉCRAN

1. Renseignez les champs obligatoires. Sélectionnez ensuite la licence d’utilisateur : Salesforce et le profil que vous avez précédemment créé. Cliquez sur Enregistrer lorsque vous avez terminé.

   CAPTURE D’ÉCRAN

L’étape 2 sur 3 est terminée.
