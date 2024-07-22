---
unique-page-id: 11377945
description: Présentation du journal d’audit - Documents Marketo - Documentation du produit
title: Présentation du journal d’audit
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Présentation du journal d’audit {#audit-trail-overview}

Le journal d’audit vous permet d’obtenir un historique complet (six mois) des modifications apportées à votre instance Marketo.

>[!NOTE]
>
>L’historique des données du journal d’audit a commencé le 14 septembre 2016.

![](assets/audit-trail-overview-1.png)

## Présentation du journal d’audit {#what-is-audit-trail}

Le journal d’audit capture, en temps réel, une liste complète d’actions et d’événements se produisant dans un abonnement Marketo. Il comprend un moyen en libre-service d’accéder à un historique de données de six mois afin de répondre à des questions telles que :

Qu’est-il advenu de cette ressource ou de ce paramètre et qui l’a mise à jour pour la dernière fois ?

Qu&#39;est-ce que l&#39;utilisateur X a fait ?

Qui se connecte à notre compte ?

## Ce que nous vérifions {#what-we-audit}

Marketo effectuera le suivi des actions [créer, modifier et supprimer](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) pour :

* Conception de ressources de studio
* Tous les programmes Marketo
* Campagnes intelligentes
* Listes (dynamiques/statiques)
* Utilisateurs (admin)
* Rôles et autorisations (admin)
* Workspace et partitions (admin)
* Historique de connexion des utilisateurs

>[!NOTE]
>
>Marketo n’est _pas_ des modifications de contrôle effectuées actuellement dans Web Personalization, Predictive Content ou Sales Insight.

## Composants de suivi {#audit-trail-components}

Le journal d’audit se compose de trois composants.

**1) [Suivi de la ressource](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Voir l’activité effectuée sur des ressources spécifiques.

**2) [Journal d’audit de l’administrateur](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Surveillez les détails basés sur l’utilisateur.

**3) [Historique de connexion de l’utilisateur](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Découvrez qui s’est connecté à votre abonnement et quand. Inclut également les tentatives de connexion ayant échoué.

>[!TIP]
>
>Il y a tellement de choses que vous pouvez contrôler à l’aide du journal d’audit, veillez à utiliser [Filtrage](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md) !

## Exportation des données {#exporting-data}

Vous ne pouvez afficher que l’équivalent de 30 jours de données dans votre instance. Pour obtenir (jusqu&#39;à) six mois, utilisez l&#39;option d&#39;export.

![](assets/two.png)

>[!NOTE]
>
>**Définition**
>
>**Inconnu :** Dans [!DNL Webhook], le nom et l’adresse électronique d’un utilisateur peuvent être répertoriés comme &quot;Inconnu&quot;. Cela se produit lorsque vous modifiez les valeurs de liste de sélection dans le CRM. Ces valeurs apparaissent dans les formulaires Marketo et les landing pages. Cette mise à jour côté CRM génère automatiquement vos landing pages référençant le formulaire. Dans [!DNL Webhook], nous allons capturer que la landing page a été ébauchée, mais le nom et l’email de l’utilisateur s’afficheront comme &quot;Inconnu&quot;, car nous ne sommes pas en mesure de capturer les informations de l’utilisateur du côté CRM.

>[!MORELIKETHIS]
>
>[Activer le journal d’audit](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
