---
unique-page-id: 2360245
description: Supprimer le texte de désabonnement de la section Admin Email - Documents Marketo - Documentation du produit
title: Supprimer le texte Désabonner de la section Courrier électronique d’administration
exl-id: 2961a9b6-8b35-4227-bf8a-a07b2664a6c4
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 3%

---

# Supprimer le texte Désabonner de la section Courrier électronique d’administration {#remove-unsubscribe-text-from-the-admin-email-section}

La seule raison pour laquelle vous devriez supprimer complètement le contenu de désabonnement de la zone &quot;Admin > Email&quot; est si vous choisissez de créer le lien de désabonnement dans les modèles d’email eux-mêmes. La zone de texte comporte une validation qui ne vous permet pas d’enregistrer sans contenu. Vous pouvez contourner ce problème en ajoutant un petit commentaire de HTML. Le commentaire de HTML ne s’affiche pas dans le client de messagerie, car il affiche l’email en HTML et les commentaires sont omis. Voici comment le faire.

1. Cliquez sur l&#39;icône **Admin**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-1.png)

1. Cliquez sur **Email**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-2.png)

1. Sélectionnez tout le texte et appuyez sur la touche **Supprimer** clé.

   >[!CAUTION]
   >
   >Avant la suppression, copiez/collez-le dans un document texte en tant que sauvegarde.

1. Saisissez `<!--This is a comment -->`.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-3.png)

1. Cliquez sur **Enregistrer les modifications**.

   ![](assets/remove-unsubscribe-text-from-the-admin-email-section-4.png)

>[!NOTE]
>
>Pour le **Désabonner le texte** vous devez ajouter un seul caractère. Utilisez un tiret ou un point.
