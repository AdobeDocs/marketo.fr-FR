---
unique-page-id: 11377945
description: Journal D'Audit] Aperçu - Documents Marketo - Documentation Du Produit
title: Vue d’ensemble du journal d’audit
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 2%

---

# Vue d’ensemble du journal d’audit {#audit-trail-overview}

Le journal d&#39;audit vous permet d&#39;obtenir un historique complet (équivalent à six mois) des modifications apportées à votre instance Marketo.

>[!NOTE]
>
>L&#39;historique des données du journal d&#39;audit a commencé le 14 septembre 2016.

![](assets/audit-trail-overview-1.png)

## Qu&#39;est-ce que le journal d&#39;audit ? {#what-is-audit-trail}

Le journal d&#39;audit capture, en temps réel, une liste complète d&#39;actions et d&#39;événements se produisant dans un abonnement Marketo. Il comprend un accès en libre-service à un historique de données de six mois pour aider à répondre à des questions telles que :

Qu’est-il advenu de cette ressource ou de ce paramètre et qui l’a mis à jour pour la dernière fois ?

Qu’a fait l’utilisateur X ?

Qui se connecte à notre compte ?

## Ce que nous vérifions {#what-we-audit}

Marketo effectuera l’audit des actions [créer, modifier et supprimer](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) pour :

* Ressources Design Studio
* Tous les programmes Marketo
* Campagnes intelligentes
* Listes (dynamiques/statiques)
* Utilisateurs (admin)
* Rôles et autorisations (administrateur)
* Workspace et partitions (admin)
* Historique de connexion de l’utilisateur

>[!NOTE]
>
>Marketo n’effectue _pas_ l’audit des modifications apportées actuellement à Web Personalization, au contenu prédictif ou à Sales Insight.

## Composants du journal d’audit {#audit-trail-components}

Le journal d&#39;audit comprend trois composants.

**1) [Journal d’audit des ressources](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Voir Activité effectuée sur des ressources spécifiques.

**2) [Journal d&#39;audit d&#39;administration](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Surveillez les détails relatifs à l’utilisateur.

**3) [Historique de connexion de l’utilisateur](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Vérifiez qui s&#39;est connecté à votre abonnement et quand. Inclut également les tentatives de connexion ayant échoué.

>[!TIP]
>
>Il y a tant de choses que vous pouvez auditer à l&#39;aide du journal d&#39;audit, veillez à utiliser [Filtrage](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md) !

## Exportation des données {#exporting-data}

Vous ne pouvez afficher que 30 jours de données dans votre instance. Pour obtenir (jusqu&#39;à) six mois d&#39;argent, utilisez l&#39;option d&#39;exportation.

![](assets/two.png)

>[!NOTE]
>
>**Définition**
>
>**Inconnu :** dans [!DNL Webhook], il se peut que le nom et l’adresse électronique d’un utilisateur soient répertoriés comme « Inconnus ». Cela se produit lorsque vous modifiez les valeurs de votre liste de sélection dans votre CRM. Ces valeurs apparaissent dans les formulaires Marketo et les pages de destination. Cette mise à jour du côté du CRM crée automatiquement vos pages de destination qui font référence au formulaire. En [!DNL Webhook], nous allons capturer que la page de destination a été brouillée, mais le nom et l’adresse e-mail de l’utilisateur s’afficheront comme « Inconnu », car nous ne pouvons pas capturer les informations de l’utilisateur du côté du CRM.

>[!MORELIKETHIS]
>
>[Activer le journal d&#39;audit](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
