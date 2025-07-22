---
description: Connecter un nouvel administrateur à Marketo - Documents Marketo - Documentation du produit
title: Connecter le nouvel administrateur à Marketo
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Connecter le nouvel administrateur à Marketo {#connect-new-admin-to-marketo}

Si l’autre administrateur est déjà connecté à Marketo, il lui suffit d’effectuer l’étape 1.

Si le second administrateur n’est pas connecté à Marketo en tant qu’administrateur...

1. L’administrateur principal doit déconnecter le second administrateur de Marketo à partir de [!UICONTROL Paramètres] > Marketo > [!UICONTROL Accès utilisateur].

1. L’administrateur secondaire se connecte à son compte MSC, accède à [!UICONTROL Paramètres] > Marketo, puis clique sur **[!UICONTROL Se connecter]**.

1. Désormais, l’utilisateur secondaire est connecté à Marketo en tant qu’administrateur.

1. L’administrateur principal peut désormais se connecter et se déconnecter de Marketo.

>[!NOTE]
>
>Les autres utilisateurs resteront connectés tant que l’utilisateur B sera connecté en tant qu’administrateur avant que l’utilisateur A ne se déconnecte.

## Mettre À Jour Votre Connexion Marketo {#update-your-marketo-connection}

Si vous décidez de supprimer l’administrateur qui a configuré l’intégration de Marketo, consultez cet article pour savoir comment procéder.

L’intégration de Marketo sera liée à un utilisateur administrateur [!DNL Sales Connect]/actions. En règle générale, il s’agit de l’administrateur qui a cliqué pour la première fois sur le bouton **[!UICONTROL Connect]** sur la page de connexion Marketo et établi la connexion.

Pour supprimer l’administrateur qui a établi la connexion Marketo, une nouvelle connexion doit d’abord être établie par un autre utilisateur administrateur. Nous avons répertorié ci-dessous les tâches qui devront être effectuées pour ce faire.

Dans un souci de simplification des instructions, l’administrateur actuellement connecté est appelé administrateur A et l’administrateur pour lequel vous souhaitez établir une nouvelle connexion à Marketo est appelé administrateur B :

1. L’administrateur A (actuellement administrateur connecté) devra supprimer l’accès à l’intégration avec Marketo de l’administrateur B (nouvel administrateur).

1. Demandez à l’administrateur B (nouvel administrateur) d’établir une nouvelle connexion à Marketo.

1. Déconnectez l’administrateur A (administrateur connecté à l’origine).

>[!NOTE]
>
>L’administrateur d’origine responsable de l’intégration de Marketo voit une option de « Déconnexion » sur laquelle il est possible de cliquer lors de la navigation vers la page d’intégration de Marketo. Les autres administrateurs (qui n’ont pas établi de connexion) ne le feront pas. En outre, les administrateurs auxquels l’accès à l’intégration Marketo a été accordé ne pourront pas cliquer sur Se connecter. Vous devez donc d’abord suivre les étapes de suppression de l’accès à l’intégration.

**Supprimer l’accès Marketo de l’administrateur B**

L’administrateur A (administrateur responsable à l’origine de la connexion) doit suivre les étapes suivantes.

1. Dans l’application web, cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

1. Cliquez sur **Marketo**.

1. Cliquez sur **[!UICONTROL Accès utilisateur]**.

1. Recherchez l’administrateur pour lequel vous souhaitez établir la nouvelle connexion Marketo.

1. Supprimez l’accès.

**Établir une nouvelle connexion pour l’administrateur B**

Ces étapes doivent être suivies par l’administrateur B (nouvel administrateur)

1. Dans l’application web, cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

1. Cliquez sur **Marketo**.

1. Cliquez sur **[!UICONTROL Déconnecter]**.

**Déconnexion de l’intégration Marketo pour l’administrateur A**

Ces étapes doivent être suivies par l’administrateur A (administrateur connecté à l’origine).

1. Dans l’application web, cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

1. Cliquez sur **Marketo**.

1. Cliquez sur **[!UICONTROL Déconnecter]**.

Maintenant qu’un nouvel administrateur a établi une connexion à Marketo et que l’administrateur d’origine a été déconnecté, l’administrateur connecté d’origine peut être supprimé en toute sécurité de l’instance [!DNL Sales Connect]/Actions.
