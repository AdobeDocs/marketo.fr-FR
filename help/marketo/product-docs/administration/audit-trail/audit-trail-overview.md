---
unique-page-id: 11377945
description: Aperçu de la piste d’audit - Documentation Marketo - Documentation du produit
title: Aperçu de la piste d’audit
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Aperçu de la piste d&#39;audit {#audit-trail-overview}

La piste d’audit vous permet d’obtenir un historique complet (d’une durée de six mois) des modifications effectuées dans votre instance Marketo.

>[!NOTE]
>
>L’historique des données des pistes d’audit a commencé le 14 septembre 2016.

![](assets/one.png)

## Qu’est-ce que la piste d’audit {#what-is-audit-trail}

La piste de vérification capture, en temps réel, une liste complète d&#39;actions et de événements survenant dans un abonnement Marketo. Il comprend un moyen en libre-service d&#39;accéder à un historique de données de six mois pour vous aider à répondre à des questions telles que :

Qu’est-il advenu de cet actif ou paramètre et qui l’a mis à jour en dernier ?

Qu&#39;est-ce que l&#39;utilisateur X a fait ?

Qui se connecte à notre compte ?

## Ce que nous vérifions {#what-we-audit}

Marketo va contrôler les actions [créer, modifier et supprimer](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) pour :

* Création de fichiers studio
* Tous les programmes Marketo
* Campagnes dynamiques
* Listes (dynamiques/statiques)
* Utilisateurs (admin)
* Rôles et autorisations (admin)
* Espace de travail et partitions (admin)
* Historique de connexion des utilisateurs

>[!NOTE]
>
>Marketo _n’effectue pas pour l’instant_ les modifications apportées au contrôle dans la personnalisation Web, le contenu prédictif ou les statistiques de ventes.

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

## Exportation des données {#exporting-data}

Vous ne pouvez vue que 30 jours de données dans votre instance. Pour obtenir (jusqu&#39;à) six mois d&#39;exportation, utilisez l&#39;option d&#39;exportation.

![](assets/two.png)

>[!NOTE]
>
>**Définition**
>
>**Inconnu :** dans la piste d’audit, le nom et l’adresse électronique d’un utilisateur peuvent être répertoriés comme &quot;Inconnu&quot;. Cela se produit lorsque vous modifiez les valeurs de la liste de sélection dans votre gestion de la relation client. Ces valeurs s’affichent dans les formulaires et landings page Marketo. Si vous effectuez cette mise à jour du côté CRM, vos landings page référençant le formulaire seront automatiquement rédigés. Dans la piste d’audit, nous allons capturer que le landing page a été rédigé, mais le nom et l’adresse électronique de l’utilisateur s’afficheront comme &quot;Inconnu&quot;, car nous ne sommes pas en mesure de capturer les informations de l’utilisateur du côté CRM.

>[!MORELIKETHIS]
>
>[Activer la piste d&#39;audit](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
