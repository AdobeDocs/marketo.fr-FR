---
unique-page-id: 2360245
description: Suppression du texte de désabonnement de la section E-mail de l’administrateur - Documents Marketo - Documentation du produit
title: Supprimez le texte de désabonnement de la section E-mail de l’administrateur.
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
feature: Email Setup
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Supprimez le texte de désabonnement de la section Admin > Email . {#remove-unsubscribe-text-from-the-admin-email-section}

La seule raison pour laquelle vous devriez supprimer complètement le contenu de désabonnement de la zone **[!UICONTROL Admin]** > **[!UICONTROL E-mail]** est que vous choisissez de créer le lien de désabonnement dans les modèles d’e-mail eux-mêmes. La zone de texte comporte une validation qui ne vous permet pas d’enregistrer sans contenu. Vous pouvez contourner ce problème en ajoutant un petit commentaire HTML. Le commentaire HTML ne s’affichera pas dans le client de messagerie, car il effectue le rendu de l’e-mail dans HTML et les commentaires sont omis. Voici comment procéder.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Sélectionnez tout le texte et appuyez sur la touche **[!UICONTROL Supprimer]**.

   >[!CAUTION]
   >
   >Avant la suppression, copiez/collez ceci dans un document texte en tant que sauvegarde.

1. Saisissez `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Pour le **Texte de désabonnement** vous devez ajouter un seul caractère. Utilisez un tiret ou un point.
