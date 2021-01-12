---
unique-page-id: 11377945
description: Aperçu de la piste d’audit - Documents marketing - Documentation du produit
title: Aperçu de la piste d’audit
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---


# Aperçu de la piste d&#39;audit {#audit-trail-overview}

La piste d’audit vous permet d’obtenir un historique complet (d’une durée de six mois) des modifications apportées à votre instance de marché.

>[!NOTE]
>
>L’historique des données des pistes d’audit a commencé le 14 septembre 2016.

![](assets/one.png)

## Qu’est-ce que la piste d’audit {#what-is-audit-trail}

La piste d’audit capture, en temps réel, une liste complète d’actions et de événements survenant au sein d’un abonnement de marketing. Il comprend un moyen en libre-service d&#39;accéder à un historique de données de six mois pour vous aider à répondre à des questions telles que :

Qu’est-il advenu de cet actif ou paramètre et qui l’a mis à jour en dernier ?

Qu&#39;est-ce que l&#39;utilisateur X a fait ?

Qui se connecte à notre compte ?

## Ce que nous vérifions {#what-we-audit}

Marketo contrôlera les actions [créer, modifier et supprimer](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) pour :

* Création de fichiers studio
* Tous les programmes du marketing
* Campagnes dynamiques
* Listes (dynamiques/statiques)
* Utilisateurs (admin)
* Rôles et autorisations (admin)
* Espace de travail et partitions (admin)
* Historique de connexion des utilisateurs

>[!NOTE]
>
>Marketo est _différent de_ modifications d’audit effectuées pour l’instant dans la personnalisation Web, le contenu prédictif ou les statistiques de ventes.

## Composants de piste d&#39;audit {#audit-trail-components}

La piste d’audit comprend trois composantes.

**1) Suivi de la vérification  [des ressources](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Reportez-vous à la page activité effectuée pour des ressources spécifiques.

**2) Piste de vérification  [de l&#39;administrateur](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Surveillez les détails utilisateur.

**3) Historique de connexion  [des utilisateurs](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Voyez qui s&#39;est connecté à votre abonnement et quand. Inclut également les tentatives de connexion ayant échoué.

>[!TIP]
>
>Il y a tellement de choses que vous pouvez contrôler à l&#39;aide de la piste d&#39;audit, veillez à utiliser [Filtrage](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md) !

## Exportation de données {#exporting-data}

Vous ne pouvez vue que 30 jours de données dans votre instance. Pour obtenir (jusqu&#39;à) six mois d&#39;exportation, utilisez l&#39;option d&#39;exportation.

![](assets/two.png)

>[!NOTE]
>
>**Définition**
>
>**Inconnu :** dans la piste d’audit, le nom et l’adresse électronique d’un utilisateur peuvent être répertoriés comme &quot;Inconnu&quot;. Cela se produit lorsque vous modifiez les valeurs de la liste de sélection dans votre gestion de la relation client. Ces valeurs s’affichent dans les landings page et formulaires marketing. Si vous effectuez cette mise à jour du côté CRM, vos landings page référençant le formulaire seront automatiquement rédigés. Dans la piste d’audit, nous allons capturer que le landing page a été rédigé, mais le nom et l’adresse électronique de l’utilisateur s’afficheront comme &quot;Inconnu&quot;, car nous ne sommes pas en mesure de capturer les informations de l’utilisateur du côté CRM.

>[!MORELIKETHIS]
>
>[Activer la piste d&#39;audit](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
