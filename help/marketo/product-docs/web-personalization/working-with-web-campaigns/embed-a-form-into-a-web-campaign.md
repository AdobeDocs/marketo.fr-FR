---
unique-page-id: 10095554
description: Incorporation d’un formulaire dans une campagne web - Documents Marketo - Documentation du produit
title: Incorporation d’un formulaire dans une campagne web
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
feature: Web Personalization
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 1%

---

# Incorporation d’un formulaire dans une campagne web {#embed-a-form-into-a-web-campaign}

Découvrez comment incorporer un formulaire Marketo dans une campagne web (boîte de dialogue, dans une zone ou un widget).

1. Cliquez avec le bouton droit sur un formulaire approuvé. Sélectionner **Code incorporé**.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. Copiez le code.

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. Dans Personnalisation Web, accédez à **Campagnes Web**.

   ![](assets/web-campaigns-hand-7.jpg)

1. Cliquez sur **Créer une campagne**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. Dans l’éditeur de texte enrichi, cliquez sur l’icône HTML .

   ![](assets/five-1.png)

1. Collez le code incorporé du formulaire dans l’éditeur de source de HTML. Cliquez sur **Mettre à jour**.

   ![](assets/six-1.png)

1. Le formulaire ne s’affiche pas dans la vue de l’éditeur, mais vous pouvez le prévisualiser pour visualiser le rendu dans une campagne.

1. Cliquez sur **Launch** pour lancer la campagne.

   >[!NOTE]
   >
   >Toute modification apportée aux champs du formulaire doit être effectuée dans Marketo Marketing Activities in Edit Draft of the Form.

## Trois manières d’ajouter une image d’arrière-plan à un formulaire {#three-ways-to-add-a-background-image-to-a-form}

Pour ajouter une image d’arrière-plan à votre formulaire, vous pouvez :

* Modification de la page CSS d’un thème de formulaire
* Modifier les couleurs de la boîte de dialogue ou du widget dans Définir la campagne
* Ajout du code CSS au script

Pour modifier la page CSS d’un thème de formulaire, reportez-vous à la section [cet article](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

Pour modifier les couleurs de la boîte de dialogue ou du widget dans Définir la campagne :

1. Dans l’éditeur de texte enrichi, sélectionnez un type de campagne de boîte de dialogue, ainsi qu’un style de boîte de dialogue, une couleur d’en-tête et une couleur d’arrière-plan pour personnaliser les couleurs d’arrière-plan du formulaire. Cliquez sur **Enregistrer**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. Voici un exemple de l’aspect d’un style de boîte de dialogue de rognage moderne avec un en-tête et une couleur d’arrière-plan violets clairs.

   ![](assets/image2015-12-29-18-3a27-3a31.png)

Pour ajouter du code CSS au script :

1. Dans l’éditeur de texte enrichi, cliquez sur l’icône HTML .

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. Collez le code incorporé du formulaire avec le code de style d’arrière-plan dans l’éditeur de source de HTML. Cliquez sur **Mettre à jour**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. Cliquez sur **Aperçu** pour visualiser le rendu dans une campagne (le formulaire ne s’affiche pas dans la vue de l’éditeur). Voici un exemple de la manière dont le code de formulaire ci-dessus s’affiche dans une campagne avec une image d’arrière-plan.

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [Modification de la page CSS d’un thème de formulaire](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [Afficher le message de remerciement sans page d’entrée de relance](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Formulaires 2.0](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference)
