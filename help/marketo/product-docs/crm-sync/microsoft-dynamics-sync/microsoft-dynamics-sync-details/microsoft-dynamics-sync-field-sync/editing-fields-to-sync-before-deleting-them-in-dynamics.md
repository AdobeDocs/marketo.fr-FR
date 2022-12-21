---
description: Modification de champs à synchroniser avant leur suppression dans Dynamics - Documents Marketo - Documentation du produit
title: Modification des champs à synchroniser avant leur suppression dans Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Modification des champs à synchroniser avant leur suppression dans Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Parfois, vous pouvez vouloir supprimer des champs dans Dynamics. Marketo conserve la liste des champs en tant que référence sur laquelle baser la synchronisation. Si un champ est supprimé dans Dynamics pendant la synchronisation, la synchronisation peut rencontrer des erreurs. Avant de supprimer des champs, procédez comme suit.

1. Dans Marketo, cliquez sur **Administration**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Sous Intégration, cliquez sur **Microsoft Dynamics**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Cliquez sur **Désactiver la synchronisation**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. Dans un nouvel onglet de votre navigateur, connectez-vous à Dynamics et supprimez les champs de votre choix.

1. De retour dans Marketo, sous Microsoft Dynamics, cliquez sur **Modifier** en regard de &quot;Étape 2 : Sélectionnez Champs à synchroniser.&quot;

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Vérifiez les champs et cliquez sur **Enregistrer**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Cliquer **Enregistrer** est nécessaire pour enregistrer le schéma mis à jour pour la synchronisation, même si aucune modification n’a été apportée.

>[!NOTE]
>
>Si la synchronisation n’est pas arrêtée avant la suppression d’un champ dans Dynamics, la synchronisation peut rencontrer des erreurs. Si c’est le cas, la synchronisation s’arrête. Avant de reprendre, l’administrateur de Marketo doit consulter &quot;Sélectionner les champs à synchroniser&quot; (dont il est question ci-dessus) et cliquer sur **Enregistrer** pour que la synchronisation accepte les modifications du schéma.

N’oubliez pas d’activer la synchronisation une fois les modifications enregistrées.
