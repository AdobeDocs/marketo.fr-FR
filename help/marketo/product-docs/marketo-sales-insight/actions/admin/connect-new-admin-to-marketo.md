---
description: Connexion du nouvel administrateur à Marketo - Documents Marketo - Documentation du produit
title: Connexion d’un nouvel administrateur à Marketo
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Connexion d’un nouvel administrateur à Marketo {#connect-new-admin-to-marketo}

Si l’autre administrateur est déjà connecté à Marketo, il doit uniquement effectuer l’étape 1.

Si le second administrateur n’est pas connecté à Marketo en tant qu’administrateur...

1. L’administrateur principal doit déconnecter le second administrateur de Marketo de Paramètres > Marketo > Accès utilisateur.

1. L’administrateur secondaire se connecte à son compte MSC, accède à Paramètres > Marketo, puis clique sur **Se connecter**.

1. Désormais, l’utilisateur secondaire est connecté à Marketo en tant qu’administrateur.

1. L’administrateur principal peut désormais se connecter et se déconnecter de Marketo.

>[!NOTE]
>
>Les autres utilisateurs resteront connectés tant que l’utilisateur B est connecté en tant qu’administrateur avant que l’utilisateur A ne se déconnecte.

## Mettre à jour votre connexion Marketo {#update-your-marketo-connection}

Si vous décidez de supprimer l’administrateur qui a configuré l’intégration Marketo, consultez cet article pour en savoir plus.

L’intégration de Marketo sera liée à un utilisateur administrateur de Connect de vente/Actions. En règle générale, il s’agit de l’administrateur qui a cliqué pour la première fois sur le bouton &quot;Se connecter&quot; sur la page de connexion de Marketo et qui a établi la connexion.

Pour supprimer l’administrateur qui a établi la connexion Marketo, une nouvelle connexion doit d’abord être établie par un autre utilisateur administrateur. Nous avons répertorié ci-dessous les tâches qui doivent être terminées pour ce faire.

Pour simplifier les instructions, nous nous référerons à l’administrateur actuellement connecté en tant qu’administrateur A et à l’administrateur que vous souhaitez établir une nouvelle connexion à Marketo avec en tant qu’administrateur B :

1. L’administrateur A (administrateur actuellement connecté) devra supprimer de l’administrateur B (nouvel administrateur) l’accès à l’intégration avec Marketo.

1. Demandez à l’administrateur B (nouvel administrateur) d’établir une nouvelle connexion à Marketo.

1. Déconnectez l’administrateur A (administrateur initialement connecté).

>[!NOTE]
>
>L’administrateur d’origine responsable de l’intégration Marketo voit apparaître une option &quot;Déconnecter&quot; sur laquelle il est possible de cliquer lors de l’accès à la page d’intégration de Marketo. Les autres administrateurs (qui n’ont pas établi de connexion) ne le feront pas. En outre, les administrateurs qui ont reçu l’accès à l’intégration Marketo ne pourront pas cliquer sur Se connecter. C’est pourquoi vous devez d’abord suivre les étapes pour supprimer l’accès à l’intégration.

**Supprimer l’accès Marketo de l’administrateur B**

L’administrateur A (administrateur responsable à l’origine de la connexion) doit suivre ces étapes.

1. Dans l’application web, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

1. Cliquez sur **Marketo**.

1. Cliquez sur **Accès utilisateur**.

1. Recherchez l’administrateur pour lequel vous souhaitez établir la nouvelle connexion Marketo.

1. Supprimez l’accès.

**Établissement d’une nouvelle connexion pour l’administrateur B**

Ces étapes doivent être suivies par l’administrateur B (nouvel administrateur).

1. Dans l’application web, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

1. Cliquez sur **Marketo**.

1. Cliquez sur **Déconnecter**.

**Déconnecter l’intégration Marketo pour l’administrateur A**

Ces étapes doivent être suivies par l’administrateur A (administrateur connecté à l’origine).

1. Dans l’application web, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

1. Cliquez sur **Marketo**.

1. Cliquez sur **Déconnecter**.

Maintenant qu’un nouvel administrateur a établi une connexion à Marketo et que l’administrateur d’origine a été déconnecté, l’administrateur d’origine peut être supprimé de l’instance Connect/Actions de vente en toute sécurité.
