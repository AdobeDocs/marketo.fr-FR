---
unique-page-id: 2950555
description: Modifier les paramètres de publication enrichie sur Facebook - Documents Marketo - Documentation du produit
title: Modifier les paramètres de publication enrichie Facebook
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
hide: true
hidefromtoc: true
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 1%

---

# Modifier [!DNL Facebook] paramètres de publication enrichie {#edit-facebook-rich-post-settings}

Personnaliser les publications lorsque des personnes vous partagent sur [!DNL Facebook].

>[!AVAILABILITY]
>
>Tous les utilisateurs de Marketo Engage n’ont pas acheté cette fonctionnalité. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).

Marketo _applications sociales_ permet à vos prospects de partager vos landing pages avec leurs connexions sur les réseaux sociaux tels que Facebook, Twitter, etc. Les balises OpenGraph de Facebook (balises de journalisation) vous permettent de spécifier quelles informations de votre page de destination sont incluses dans les publications Facebook.

## Sélectionner les options de publication enrichies {#select-rich-post-options}

Vous pouvez spécifier les types d’informations de page à utiliser dans les publications riches en [!DNL Facebook] générées par des partages de votre page de destination.

1. Sélectionnez **[!UICONTROL Message Facebook]** dans l’éditeur pour votre bouton vidéo ou social _&#x200B;_[!DNL YouTube_]_.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Sélectionnez l’une des options suivantes pour votre Message [!DNL Facebook].

   * Ajouter du contenu statique : sélectionnez cette option pour saisir manuellement le titre, la légende et la description.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Ajouter du contenu dynamique : votre application de réseau social peut utiliser les balises `<TITLE>`, `<CAPTION>` et `<DESCRIPTION>` de votre page de destination pour remplir votre publication enrichie.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Ils doivent déjà exister dans la source de la page, mais pour plus de contrôle, vous pouvez ajouter des balises d’organisation du [!DNL Facebook] spécifiques à votre page de destination.

   * Ne pas ajouter de contenu riche : limite les publications [!DNL Facebook] de votre page de destination au message et au lien principaux.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Ajout de balises d’organisation [!DNL Facebook] à une page de destination {#add-facebook-og-tags-to-a-landing-page}

Pour contrôler les éléments de page qui seront inclus dans les partages [!DNL Facebook] de votre page de destination, vous pouvez ajouter des balises [!DNL Facebook] (Open Graph) pour le titre, la légende et la description à votre page de destination.

1. Ouvrez la page de destination contenant votre bouton **[!DNL YouTube]vidéo** ou social.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   La **[!UICONTROL Landing Page Designer]** s’ouvre dans une nouvelle fenêtre.

1. Sélectionnez **[!UICONTROL Actions de la page de destination]** > **[!UICONTROL Modifier les balises de métadonnées de page]**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Ajoutez l’HTML qui définit og:title, og:caption et og:description. Copiez et collez ces lignes et remplacez le texte de l’espace réservé :

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Veillez à utiliser la syntaxe HTML appropriée lors de l’ajout des balises de journalisation.
