---
unique-page-id: 2950549
description: Configuration du flux recommandé par Social - Documents Marketo - Documentation du produit
title: Configuration du flux recommandé par Social
exl-id: 01b54215-4a0c-4639-80d2-ec30603b3695
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# Configuration du flux recommandé par Social {#configure-social-recommend-flow}

Lorsque vous créez une application sociale, vous pouvez configurer les choix de réseau social et les invites qu’un utilisateur rencontre lorsqu’il s’inscrit.

>[!IMPORTANT]
>
>Le 31 juillet 2024, nous avons commencé à abandonner cette fonctionnalité. Il n’est plus possible de créer de nouvelles ressources. Les ressources existantes continueront à fonctionner jusqu’au 31 janvier 2025. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Sélectionner des réseaux à partager {#select-networks-for-sharing}

>[!NOTE]
>
>Cette opération est très similaire à [la configuration du flux d’inscription/partage sur les réseaux sociaux](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-social-sign-up-share-flow.md), mais elle concerne les liens de partage _sous_ de l’application sociale.

1. Accédez à **Activités marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Sélectionnez l’application et cliquez sur **Modifier le brouillon**.

   ![](assets/image2014-9-22-11-3a51-3a6.png)

1. Dans l’éditeur d’applications sociales, accédez à **Flux recommandé** > **Réseaux sociaux**.

   ![](assets/recommendedflow.png)

1. Sélectionnez les réseaux vers lesquels un utilisateur peut partager.

   ![](assets/socialnetworkschoose.png)

## Configuration du message Facebook {#configure-the-facebook-message}

1. Configurez le message qui s’affichera dans les publications Facebook.

   ![](assets/image2014-9-22-11-3a53-3a21.png)

   >[!NOTE]
   >
   >Dans un partage vidéo, la miniature est générée automatiquement.

   Si vous choisissez **Ajouter du contenu dynamique**, les valeurs des balises OpenGraph de la page (og:title, og:caption et og:description) et la miniature sont automatiquement ajoutées aux publications Facebook. Voir l’étape suivante.

   Si vous choisissez **Ajouter du contenu statique**, saisissez le titre, la légende et la description, puis téléchargez une image. Voir les deux étapes suivantes.

1. Dans la fenêtre Afficher et modifier, cliquez sur **Afficher les modifications** pour personnaliser l’invite de partage et le message qui s’afficheront dans les publications Facebook.

   >[!TIP]
   >
   >Pour plus d’informations, voir [Modifier les paramètres de publication enrichie Facebook](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md).

   ![](assets/image2014-9-22-11-3a54-3a36.png)

   >[!NOTE]
   >
   >L’ [URL de partage](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) est automatiquement ajouté à tous les messages de partage.

1. Si vous avez choisi **Ajouter du contenu statique** ci-dessus, modifiez le titre, la légende et la description, puis chargez une image personnalisée (à partir de vos images et fichiers Marketo).

   ![](assets/image2014-9-22-11-3a55-3a14.png)

   Voir [Ajout d’images et de fichiers à Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Si vous chargez une image, vous ne la verrez pas ici tant que vous ne fermez pas et rouvrez l’éditeur d’applications sociales.

1. Cliquez sur **Suivant**.

Si vous choisissez , les valeurs des balises OpenGraph de la page (og:title, og:caption et og:description) et la miniature sont automatiquement ajoutées aux publications Facebook. Voir l’étape suivante.

## Configuration du message de Twitter {#configure-the-twitter-message}

1. Cliquez pour modifier l’invite de partage et le message qui s’afficheront dans les tweets de Twitter.

   ![](assets/image2014-9-22-12-3a2-3a40.png)

   >[!TIP]
   >
   >Utilisez {html_title} dans votre texte de tweet pour afficher automatiquement le titre de la page.

1. Cliquez sur **Suivant**.

## Configuration du message LinkedIn {#configure-the-linkedin-message}

1. Configurez le message qui s’affichera dans les publications LinkedIn.

   ![](assets/image2014-9-22-12-3a3-3a21.png)

   Si vous choisissez le contenu **Ajouter dynamique** , les valeurs des balises de pages (titre et description) et la miniature sont automatiquement ajoutées aux publications LinkedIn. Voir l’étape suivante.

   Si vous choisissez le contenu **Ajouter statique**, saisissez le titre, la légende et la description, puis téléchargez une image. Voir les deux étapes suivantes.

1. Dans la fenêtre **Afficher et modifier**, cliquez sur **Afficher les modifications** et modifiez l’invite de partage et le message qui s’afficheront dans les publications LinkedIn.

   ![](assets/image2014-9-22-12-3a3-3a38.png)

   >[!TIP]
   >
   >Utilisez {html_title} dans votre texte de publication pour afficher automatiquement le titre de la page.

1. Si vous avez sélectionné le contenu **Ajouter statique** ci-dessus, modifiez le titre et la description, puis téléchargez une image personnalisée (à partir de vos images et fichiers Marketo).

   ![](assets/image2014-9-22-12-3a4-3a43.png)

   Voir [Ajout d’images et de fichiers à Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Si vous chargez une image, vous ne la verrez pas ici tant que vous ne fermez pas et rouvrez l’éditeur d’applications sociales.

1. Cliquez sur **Suivant**.

## Configuration du message de confirmation {#configure-the-confirmation-message}

1. Modifiez le texte de la confirmation du partage.

   ![](assets/image2014-9-22-12-3a5-3a30.png)

1. Cliquez sur **Terminer** > **Approuver** et **Fermer**.

   ![](assets/image2014-9-22-12-3a5-3a45.png)

>[!MORELIKETHIS]
>
>L’étape suivante consiste à [ajouter votre partage vidéo](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-video-share-flow.md) ou [poll](/help/marketo/product-docs/demand-generation/social/creating-a-poll/create-a-poll.md) à une page d’entrée, à Facebook ou à votre propre site web.
