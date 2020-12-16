---
unique-page-id: 2359644
description: Afficher un formulaire HTML personnalisé pour les personnes connues - Documents marketing - Documentation du produit
title: Afficher un formulaire HTML personnalisé pour les personnes connues
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# Afficher un formulaire HTML personnalisé pour les personnes connues {#show-custom-html-form-for-known-people}

Si un visiteur fait l&#39;objet d&#39;un cookie (personne connue qui a fourni une adresse électronique dans le passé), pourquoi se soucier du formulaire ? Donnez-leur juste le bouton de téléchargement. Voici comment.

1. Accédez à **Marketing** **Activités**.

   ![](assets/login-marketing-activities-5.png)

1. Sous **Activités** **marketing**, sélectionnez votre formulaire, puis cliquez sur **Modifier** **le formulaire.**

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Sous **Paramètres** du formulaire **, cliquez sur** Paramètres ****.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Définissez Si **Connu** **Visiteur, Afficher**: au **code HTML** **personnalisé**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Cliquez sur le ![—](assets/image2014-9-25-14-3a1-3a26.png) pour modifier le **code HTML** **personnalisé** qui sera présenté aux personnes connues.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. Il y a du contenu par défaut, mais n&#39;hésitez pas à le modifier.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Jetons disponibles :

   | Jeton | Description |
   |---|---|
   | `{{lead.FirstName}}` | Le prénom de la personne s&#39;affichera. |
   | `{{lead.LastName}}` | Le nom de famille de la personne s&#39;affichera alors. |
   | `{{form.Button:default=Download}}` | Le bouton du formulaire s’affiche alors. Remplacez la zone située après le bouton `=` pour modifier le texte du bouton. |
   | `{{form.NotYou:default=Not you?}}` | Ceci affiche un lien au cas où la personne serait une autre. Remplacez la zone située après le `=` pour modifier le texte du lien. |

   >[!CAUTION]
   >
   >Seuls les quatre jetons ci-dessus peuvent être utilisés. Aucun autre jeton ne fonctionnera ici.

1. Cliquez sur **Terminer**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Cliquez sur **Approuver et fermer**.

   >[!NOTE]
   >
   >Le formulaire doit être approuvé pour être utilisé sur les landings page.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >
   >Pensez à [approuver le brouillon](../../../../product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) de landing page créé par les modifications apportées au formulaire.

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >Vous pouvez diriger le clic sur le bouton vers la ressource en définissant la page de suivi de formulaire sur l’URL du fichier.

Un morceau de gâteau ! Voyez ce qu&#39;une personne verrait s&#39;elle revenait sur le même formulaire :