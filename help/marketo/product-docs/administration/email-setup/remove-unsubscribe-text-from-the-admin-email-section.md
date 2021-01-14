---
unique-page-id: 2360245
description: Supprimer le texte de désabonnement de la section Courriel de l’administrateur - Documents marketing - Documentation du produit
title: Supprimer le texte de désabonnement de la section Courriel de l’administrateur
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Supprimer le texte Désabonner de la section Courriel de l’administrateur {#remove-unsubscribe-text-from-the-admin-email-section}

La seule raison pour laquelle vous devriez supprimer complètement le contenu de désabonnement de la zone &quot;Admin > Courriel&quot; est que vous choisissez de créer le lien de désabonnement dans les modèles de courrier électronique eux-mêmes. La zone de texte possède une validation qui ne vous permet pas d’enregistrer sans contenu. Vous pouvez contourner ce problème en ajoutant un petit commentaire HTML. Le commentaire HTML ne s’affiche pas dans le client de messagerie, car il affiche le courrier électronique en HTML et les commentaires sont omis. Voici comment le faire.

1. Accédez à **Admin** et cliquez sur **Courriel**.

   ![](assets/image2016-8-26-13-3a57-3a9.png)

1. Sélectionnez tout le texte et appuyez sur la touche **Supprimer**.

   >[!CAUTION]
   >
   >Avant la suppression, copiez/collez-le dans un document de texte en tant que sauvegarde.

1. Saisissez `<!--This is a comment -->`.

   ![](assets/image2016-8-26-13-3a53-3a15.png)

1. Cliquez sur **Enregistrer les modifications**.

   ![](assets/image2016-8-26-13-3a59-3a40.png)

>[!NOTE]
>
>Pour le **texte de désabonnement**, vous devez ajouter un caractère unique. Utilisez un tiret ou un point.
