---
unique-page-id: 2360245
description: Supprimer le texte de désabonnement de la section Admin Email - Documents Marketo - Documentation du produit
title: Supprimer le texte Désabonner de la section Courrier électronique d’administration
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: d635fbd4807890266429d4a257cf7d6588736bb5
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Supprimer le texte Désabonner de la section Admin > Email {#remove-unsubscribe-text-from-the-admin-email-section}

La seule raison pour laquelle vous devriez supprimer complètement le contenu de désabonnement de la zone **[!UICONTROL Admin]** > **[!UICONTROL Email]** est si vous choisissez de créer le lien de désabonnement dans les modèles d’email eux-mêmes. La zone de texte comporte une validation qui ne vous permet pas d’enregistrer sans contenu. Vous pouvez contourner ce problème en ajoutant un petit commentaire d’HTML. Le commentaire d’HTML ne s’affiche pas dans le client de messagerie, car il affiche l’email en HTML et les commentaires sont omis. Voici comment le faire.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Sélectionnez tout le texte et appuyez sur la touche **[!UICONTROL Supprimer]**.

   >[!CAUTION]
   >
   >Avant la suppression, copiez/collez-le dans un document texte en tant que sauvegarde.

1. Saisissez `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Pour le **texte de désabonnement**, vous devez ajouter un caractère unique. Utilisez un tiret ou un point.
