---
unique-page-id: 2950530
description: Configuration de l’inscription à Social/du partage de flux - Documents Marketo - Documentation du produit
title: Configuration du flux d’inscription/de partage sur les réseaux sociaux
exl-id: 521187d1-2228-42e7-a87b-3b20a45adb03
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Configuration du flux d’inscription/de partage sur les réseaux sociaux {#configure-social-sign-up-share-flow}

Lorsque vous créez une application sociale, vous pouvez configurer les choix de réseau social et les invites qu’un utilisateur rencontre lorsqu’il s’inscrit.

>[!IMPORTANT]
>
>Le 31 juillet 2024, nous avons commencé à abandonner cette fonctionnalité. Vous ne pourrez pas créer de nouvelles ressources. Les ressources existantes continueront à fonctionner jusqu’au 31 janvier 2025. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Sélectionner des réseaux à partager {#select-networks-for-sharing}

1. Accédez à **Activités marketing**.

   ![](assets/ma-1.png)

1. Sélectionnez l’application et cliquez sur **Modifier le brouillon**.

   ![](assets/image2014-9-22-13-3a57-3a43.png)

1. Dans l’éditeur d’applications sociales, cliquez sur **Flux d’inscription** > **Réseaux sociaux**.

   ![](assets/three.png)

1. Sélectionnez (ou désélectionnez) les réseaux vers lesquels une personne peut partager.

   ![](assets/four.png)

## Configuration du message Facebook {#configure-the-facebook-message}

1. Accédez à **Flux d’inscription** > **Partager les messages**.

   ![](assets/five.png)

1. Configurez le message qui s’affichera dans les publications Facebook.

   ![](assets/image2014-9-22-13-3a58-3a54.png)

   >[!NOTE]
   >
   >Dans un partage vidéo, la miniature est générée automatiquement.

   Si vous choisissez **Ajouter du contenu dynamique**, les valeurs des balises **OpenGraph** de la page (og:title, og:caption et og:description) et la miniature sont automatiquement ajoutées aux publications Facebook. Voir l’étape suivante.

   Si vous choisissez **Ajouter du contenu statique**, saisissez le titre, la légende, la description et téléchargez une image. Voir les deux étapes suivantes.

1. Dans la fenêtre Afficher et modifier, cliquez sur **Afficher les modifications** et modifiez l’invite de partage et le message qui s’afficheront dans les publications Facebook.

   >[!TIP]
   >
   >Pour plus d’informations, voir [Modifier les paramètres de publication enrichie Facebook](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md).

   ![](assets/image2014-9-22-13-3a59-3a57.png)

   >[!NOTE]
   >
   >L’ [URL de partage](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) est automatiquement ajouté à tous les messages de partage.

1. Si vous avez choisi **Ajouter du contenu statique** ci-dessus, modifiez le titre, la légende et la description, puis téléchargez une image personnalisée (à partir de vos [**fichiers et images Marketo**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)).

   ![](assets/image2014-9-22-14-3a1-3a11.png)

   Voir [Ajout d’images et de fichiers à Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Si vous chargez une image, vous ne la verrez pas ici tant que vous ne fermez pas et rouvrez l’éditeur d’applications sociales.

1. Cliquez sur **Suivant**.

Si vous choisissez les valeurs des balises de la page (og:title, og:caption et og:description), la miniature est automatiquement ajoutée aux publications Facebook. Voir l’étape suivante.

## Configuration du message de Twitter {#configure-the-twitter-message}

1. Modifiez l’invite de partage et le message qui apparaîtront dans les tweets de Twitter.

   ![](assets/image2014-9-22-14-3a2-3a31.png)

   >[!TIP]
   >
   >Utilisez {html_title} dans votre texte de tweet pour afficher automatiquement le titre de la page.

1. Cliquez sur **Suivant**.

## Configuration du message LinkedIn {#configure-the-linkedin-message}

1. Configurez le message qui s’affichera dans les publications LinkedIn.

   ![](assets/image2014-9-22-14-3a3-3a8.png)

   Si vous choisissez **Ajouter du contenu dynamique**, les valeurs des balises de pages (titre et description) et la miniature sont automatiquement ajoutées aux publications LinkedIn. Voir l’étape suivante.

   Si vous choisissez **Ajouter du contenu statique**, saisissez le titre, la légende et la description, puis téléchargez une image. Voir les deux étapes suivantes.

1. Dans la fenêtre **Afficher et modifier**, cliquez sur **Afficher les modifications** et modifiez l’invite de partage et le message qui s’afficheront dans les publications LinkedIn.

   ![](assets/image2014-9-22-14-3a4-3a6.png)

   >[!TIP]
   >
   >Utilisez {html_title} dans votre texte de publication pour afficher automatiquement le titre de la page.

1. Si vous avez choisi **Ajouter du contenu statique** ci-dessus, modifiez le titre et la description, puis téléchargez une image personnalisée (à partir de vos [**fichiers et images Marketo**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)).

   ![](assets/image2014-9-22-13-3a55-3a17.png)

>[!NOTE]
>
>Si vous chargez une image, vous ne la verrez pas ici tant que vous ne fermez pas et rouvrez l’éditeur d’applications sociales.

>[!MORELIKETHIS]
>
>Ensuite, vous pouvez cliquer sur **Terminer** > **Approuver et fermer** et mettre votre application sociale sur une page d’entrée. Vous pouvez également configurer la [capture de personne](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-person-capture-for-a-social-app.md) ou l’ [invite de repartage](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-re-share-email-and-prompt-for-a-social-app.md).
