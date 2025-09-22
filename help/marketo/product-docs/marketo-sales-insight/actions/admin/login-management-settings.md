---
description: Paramètres de gestion des connexions - Documents Marketo - Documentation du produit
title: Paramètres de gestion des connexions
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 2%

---

# Paramètres de gestion des connexions {#login-management-settings}

Les paramètres de gestion des connexions permettent aux administrateurs de définir les préférences d’authentification des utilisateurs des actions Sales Insight à un niveau global.

>[!NOTE]
>
>Par défaut, l&#39;option [!UICONTROL Salesforce uniquement] sera sélectionnée pour les instances [!DNL Sales Insight Actions]. Nous recommandons ce paramètre afin que les utilisateurs puissent [se connecter automatiquement](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) depuis [!DNL Salesforce].

## Mettre à jour les paramètres de gestion des connexions {#update-login-management-settings}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

Pour mettre à jour vos préférences de gestion des connexions, procédez comme suit.

1. Cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/login-management-settings-1.png)

1. Sous [!UICONTROL Paramètres d’administration], cliquez sur **[!UICONTROL Général]**.

   ![](assets/login-management-settings-2.png)

1. Faites défiler jusqu’à la vignette [!UICONTROL Gestion des connexions] et sélectionnez le paramètre souhaité (dans cet exemple, nous choisissons Salesforce uniquement). Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   ![](assets/login-management-settings-3.png)

## FAQ sur Salesforce uniquement {#salesforce-only-faq}

Salesforce uniquement signifie que les utilisateurs peuvent uniquement s’authentifier pour utiliser [!DNL Sales Insight Actions] avec [!DNL Salesforce]. Il s’agit de la sélection par défaut pour les instances [!DNL Sales Insight Actions]. Elle est recommandée en raison de sa capacité à permettre aux utilisateurs de s’authentifier de manière transparente sans avoir à gérer un nom d’utilisateur et un mot de passe.

### Comment un nouvel utilisateur de mon instance active-t-il son compte lorsque « [!UICONTROL Salesforce uniquement] » est sélectionné ? {#activate-when-salesforce-only-is-selected}

Lorsqu’ils cliquent sur le bouton **[!UICONTROL Prise en main]** dans l’e-mail d’invitation, les nouveaux utilisateurs sont envoyés à un écran d’activation du compte où ils doivent se connecter à leur instance Salesforce pour activer leur compte [!DNL Sales Insight Actions].

![](assets/login-management-settings-4.png)

### Avec quelles méthodes d&#39;authentification mes utilisateurs sont-ils autorisés à s&#39;authentifier lorsque « [!UICONTROL Salesforce uniquement] » est sélectionné ? {#what-authentication-methods}

Lorsque vous accédez à notre écran de connexion, les utilisateurs saisissent d’abord leur adresse e-mail. Ils cliqueront ensuite sur le bouton Salesforce One Click [!UICONTROL Connexion], où ils pourront s’authentifier à l’aide du compte Salesforce auquel ils sont connectés.

>[!NOTE]
>
>Cela ne concerne que les utilisateurs qui accèdent directement à l’écran de connexion. Les utilisateurs qui accèdent aux actions à partir de [!DNL Salesforce] seront connectés à l’aide de l’option [Connexion automatique](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### Comment l’authentification des utilisateurs est-elle gérée pour les actions lorsqu’un utilisateur accède à une fonctionnalité Actions à partir de Salesforce et que « Salesforce uniquement » est sélectionné ? {#how-is-user-authentication-handled}

Lorsqu’un utilisateur clique sur l’une des actions (Appel, E-mail, Campagne, Tâches, Liste des campagnes, etc.), nous utilisons son authentification SFDC pour le connecter automatiquement à son compte [!DNL Sales Insight Actions]. Nous appelons cette authentification [connexion automatique](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## FAQ sur toutes les méthodes de connexion {#all-login-methods-faq}

### Comment un nouvel utilisateur de mon instance active-t-il son compte lorsque « Toutes les méthodes de connexion » est sélectionné ? {#activate-when-all-login-methods-is-selected}

Lorsqu’un nouvel utilisateur est invité à une instance, il reçoit un e-mail d’activation du compte. Ils cliqueront sur le bouton « Commencer » qui les amènera à une page qui leur demande de créer et de confirmer un mot de passe. Une fois ceci créé, leur compte sera activé et ils seront pris en compte via le workflow d’intégration.

![](assets/login-management-settings-6.png)

### Avec quoi les utilisateurs de mon instance sont-ils autorisés à se connecter lorsque « [!UICONTROL Toutes les méthodes de connexion] » est sélectionné ? {#what-are-users-allowed-to-log-in-with-all-login}

Lorsque vous utilisez notre page de connexion, les utilisateurs saisissent d&#39;abord leur adresse e-mail. Ils sont ensuite envoyés à une page qui leur propose toutes les options de connexion (nom d’utilisateur/mot de passe, SFDC, Gmail, SSO) avec lesquelles s’authentifier.
