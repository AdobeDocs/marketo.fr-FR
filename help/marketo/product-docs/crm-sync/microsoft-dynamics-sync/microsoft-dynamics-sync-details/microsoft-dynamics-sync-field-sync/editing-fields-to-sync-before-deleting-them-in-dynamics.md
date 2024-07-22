---
description: Modification de champs à synchroniser avant leur suppression dans Dynamics - Documents Marketo - Documentation du produit
title: Modification de champs à synchroniser avant de les supprimer dans Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Modification de champs à synchroniser avant de les supprimer dans Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Parfois, vous pouvez vouloir supprimer des champs dans Dynamics. Marketo Engage conserve la liste des champs en tant que référence pour la synchronisation. Si un champ est supprimé dans Dynamics pendant la synchronisation, la synchronisation peut rencontrer des erreurs. Avant de supprimer des champs, procédez comme suit.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Sous Intégration, cliquez sur **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Cliquez sur **[!UICONTROL Désactiver la synchronisation]**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. Dans un nouvel onglet de votre navigateur, connectez-vous à Dynamics et supprimez les champs de votre choix.

1. De retour dans Marketo, sous Microsoft Dynamics, cliquez sur **[!UICONTROL Modifier]** en regard de &quot;Étape 2 : sélectionner les champs à synchroniser&quot;.

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Vérifiez les champs et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Cliquez sur **[!UICONTROL Enregistrer]** pour enregistrer le schéma mis à jour pour la synchronisation, même si aucune modification n’a été apportée.

>[!NOTE]
>
>Si la synchronisation n’est pas arrêtée avant la suppression d’un champ dans Dynamics, la synchronisation peut rencontrer des erreurs. Si c’est le cas, la synchronisation s’arrête. Avant de reprendre, l’administrateur de Marketo doit passer en revue &quot;Sélectionner les champs à synchroniser&quot; (voir ci-dessus) et cliquer sur **[!UICONTROL Enregistrer]** pour que la synchronisation accepte les modifications du schéma.

N’oubliez pas d’activer la synchronisation une fois les modifications enregistrées.
