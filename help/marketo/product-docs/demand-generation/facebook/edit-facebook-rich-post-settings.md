---
unique-page-id: 2950555
description: Modifier les paramètres de publication enrichis Facebook - Documents marketing - Documentation du produit
title: Modifier les paramètres de publication enrichie Facebook
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# Modifier les paramètres de publication enrichie Facebook {#edit-facebook-rich-post-settings}

Personnalisez les publications lorsque des personnes vous [partagent](http://docs.marketo.com/display/docs/social) sur Facebook.

>[!NOTE]
>
>**Disponibilité**
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus de détails.

Les applications [sociales Marketing](http://docs.marketo.com/display/docs/social) permettent à vos prospects de partager vos landings page avec leurs connexions sur les réseaux sociaux tels que Facebook, Twitter, etc. Les balises Facebook OpenGraph (balises OG) vous permettent de spécifier les informations de votre landing page qui sont incluses dans les publications Facebook.

## Sélectionner les options de publication enrichie {#select-rich-post-options}

Vous pouvez spécifier les types d’informations de page à utiliser dans les publications enrichies Facebook générées par des partages à partir de votre landing page.

1. Sélectionnez Message **** Facebook dans l’éditeur pour votre vidéo **YouTube** ou bouton social.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Sélectionnez l’une des options suivantes pour votre message Facebook.

   * Ajouter le contenu statique : Sélectionnez cette option pour saisir manuellement le titre, la légende et la description.

      ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Ajouter le contenu dynamique : Votre application sociale peut utiliser vos landings page `<TITLE>`, `<CAPTION>`et `<DESCRIPTION>` balises pour renseigner votre publication enrichie.

      ![](assets/image2014-9-22-16-3a48-3a9.png)
   >[!NOTE]
   >
   >Elles doivent déjà exister dans la source de la page, mais pour un meilleur contrôle, vous pouvez [ajouter des balises OG Facebook spécifiques à votre landing page](edit-facebook-rich-post-settings.md).

   * N’ajoutez pas de contenu enrichi : Limite les publications Facebook de votre landing page au message principal et au lien principal.

      ![](assets/image2014-9-22-16-3a48-3a18.png)



## Ajouter les balises OG Facebook à un Landing page {#add-facebook-og-tags-to-a-landing-page}

Pour contrôler les éléments de page qui seront inclus dans les partages Facebook de votre landing page, vous pouvez ajouter des balises Facebook OG (Open Graph) pour le titre, la légende et la description de votre landing page.

1. Ouvrez le landing page contenant votre vidéo **** YouTube ou votre bouton social.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   Le Concepteur **de** Landings page s’ouvre dans une nouvelle fenêtre.

1. Sélectionnez Actions **** Landing page > **Modifier les métadonnées de page****.**

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Ajoutez le code HTML qui définit og:title, og:caption et og:description. Copiez et collez ces lignes et remplacez le texte d’espace réservé :

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Veillez à utiliser la syntaxe HTML appropriée lors de l’ajout de balises OG.
