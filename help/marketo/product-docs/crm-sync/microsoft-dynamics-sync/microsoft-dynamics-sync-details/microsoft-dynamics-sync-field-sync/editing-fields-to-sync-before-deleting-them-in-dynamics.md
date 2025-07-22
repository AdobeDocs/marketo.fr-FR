---
description: Modification des champs à synchroniser avant de les supprimer dans Dynamics - Documents Marketo - Documentation du produit
title: Modifier les champs à synchroniser avant de les supprimer dans Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Modification des champs à synchroniser avant leur suppression dans [!DNL Dynamics] {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Il peut arriver que vous souhaitiez supprimer des champs dans [!DNL Dynamics]. Marketo conserve la liste de champs comme référence pour la synchronisation. Si un champ est supprimé dans [!DNL Dynamics] alors que la synchronisation est activée, la synchronisation peut rencontrer des erreurs. Avant de supprimer des champs, procédez comme suit.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Sous [!UICONTROL Intégration], cliquez sur **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Cliquez sur **[!UICONTROL Désactiver la synchronisation]**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. Dans un nouvel onglet de votre navigateur, connectez-vous à [!DNL Dynamics] et supprimez les champs souhaités.

1. De retour dans Marketo, sous [!DNL Microsoft Dynamics], cliquez sur **[!UICONTROL Modifier]** en regard de « [!UICONTROL Étape 2 : sélectionner les champs à synchroniser] ».

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Vérifiez les champs et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Pour enregistrer le schéma mis à jour pour la synchronisation, même si aucune modification n’a été apportée, cliquez sur **[!UICONTROL Enregistrer]**.

>[!NOTE]
>
>Si la synchronisation n’est pas arrêtée avant la suppression d’un champ dans [!DNL Dynamics], elle peut rencontrer des erreurs. Si c’est le cas, la synchronisation s’arrête. Avant de reprendre, l’administrateur Marketo doit vérifier « [!UICONTROL &#x200B; Sélectionner les champs à synchroniser &#x200B;] » (décrit ci-dessus) et cliquer sur **[!UICONTROL Enregistrer]** pour que la synchronisation accepte les modifications du schéma.

N’oubliez pas d’activer la synchronisation après l’enregistrement des modifications.
