---
unique-page-id: 2950555
description: Modifier les paramètres de publication enrichie sur Facebook - Documents Marketo - Documentation du produit
title: Modifier les paramètres de la publication Facebook enrichie
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
hide: true
hidefromtoc: true
feature: Integrations
source-git-commit: 7a8f5146126d6e8a4902be9337eef4d51e108cf0
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Modifier les paramètres de la publication Facebook enrichie {#edit-facebook-rich-post-settings}

Personnalisez les publications lorsque des personnes vous partagent sur Facebook.

>[!AVAILABILITY]
>
>Tous les utilisateurs de Marketo Engage n’ont pas acheté cette fonctionnalité. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

Marketo _applications sociales_ permet à vos prospects de partager vos landing pages avec leurs connexions sur les réseaux sociaux tels que Facebook, Twitter, etc. Les balises OpenGraph de Facebook (balises de journalisation) vous permettent de spécifier quelles informations de votre page de destination sont incluses dans les publications Facebook.

## Sélectionner les options de publication enrichies {#select-rich-post-options}

Vous pouvez spécifier les types d’informations de page à utiliser dans les publications enrichies Facebook générées par des partages de votre page de destination.

1. Sélectionnez **Message Facebook** dans l’éditeur pour votre bouton vidéo ou social **YouTube**.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Sélectionnez l’une des options suivantes pour votre message Facebook.

   * Ajouter du contenu statique : sélectionnez cette option pour saisir manuellement le titre, la légende et la description.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Ajouter du contenu dynamique : votre application de réseau social peut utiliser les balises `<TITLE>`, `<CAPTION>` et `<DESCRIPTION>` de votre page de destination pour remplir votre publication enrichie.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Ces balises doivent déjà exister dans la source de la page. Pour plus de contrôle, vous pouvez toutefois ajouter des balises d’organisation Facebook spécifiques à votre page de destination.

   * N’ajoutez pas de contenu riche : limite les publications Facebook de votre page de destination au message et au lien principaux.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Ajout de balises de connexion Facebook à une page de destination {#add-facebook-og-tags-to-a-landing-page}

Pour contrôler les éléments de page qui seront inclus dans les partages Facebook de votre page de destination, vous pouvez ajouter des balises Facebook OSG (Open Graph) pour le titre, la légende et la description à votre page de destination.

1. Ouvrez la page de destination qui contient votre bouton vidéo **ou social** YouTube.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   La **Landing Page Designer** s’ouvre dans une nouvelle fenêtre.

1. Sélectionnez **Actions de la page de destination** > **Modifier les balises de métadonnées de page**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Ajoutez l’HTML qui définit og:title, og:caption et og:description. Copiez et collez ces lignes et remplacez le texte de l’espace réservé :

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Veillez à utiliser la syntaxe HTML appropriée lors de l’ajout des balises de journalisation.
