---
unique-page-id: 2359414
description: Score simple - Documents Marketo - Documentation du produit
title: Évaluation simple
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 4%

---

# Évaluation simple {#simple-scoring}

>[!PREREQUISITES]
>
>* [Configurer et ajouter une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Étape 1 : Créer une campagne d&#39;évaluation {#step-create-a-scoring-campaign}

1. Accédez à la zone **[!UICONTROL Activités marketing]**.

   ![](assets/simple-scoring-1.png)

1. Cliquez avec le bouton droit de la souris sur votre dossier **Learning** et cliquez sur **[!UICONTROL New Campaign Folder]**.

   ![](assets/simple-scoring-2.png)

1. Nommez le dossier de campagne &quot;Score&quot; et cliquez sur **[!UICONTROL Créer]**.

   ![](assets/simple-scoring-3.png)

   >[!NOTE]
   >
   >Si vous disposez déjà d’un dossier de notation, nommez celui-ci quelque chose de différent, tel que Scoring 1. Les noms de dossier doivent être uniques.

1. Cliquez avec le bouton droit sur votre dossier **Scoring** et sélectionnez **[!UICONTROL New Smart Campaign]**.

   ![](assets/simple-scoring-4.png)

1. Nommez la campagne &quot;Change Score&quot; et cliquez sur **[!UICONTROL Create]**.

   ![](assets/simple-scoring-5.png)

1. Cliquez sur l’onglet **[!UICONTROL Liste dynamique]** .

   ![](assets/simple-scoring-6.png)

   Nous voulons que cette campagne s’exécute chaque fois qu’une personne remplit votre **Formulaire de demande d’évaluation**.

1. Recherchez et faites glisser le déclencheur **[!UICONTROL Remplit le formulaire]** sur le canevas de gauche.

   ![](assets/simple-scoring-7.png)

1. Sélectionnez **Mon formulaire**.

   ![](assets/simple-scoring-8.png)

   >[!NOTE]
   >
   >Si vous avez terminé l’obtention rapide [Landing Page avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}, vous devez disposer du formulaire. Si vous avez utilisé un autre nom pour votre formulaire, sélectionnez-le.

1. Cliquez sur l’onglet **[!UICONTROL Flux]** .

   ![](assets/simple-scoring-9.png)

1. Faites glisser l’action de flux **Changer le score** sur le canevas de gauche.

   ![](assets/simple-scoring-10.png)

1. Vous pouvez saisir n’importe quelle valeur à ajouter au score de la personne. Saisissez &quot;+5&quot; dans le champ **[!UICONTROL Changer]**.

   ![](assets/simple-scoring-11.png)

   >[!TIP]
   >
   >De bonnes campagnes de notation sont essentielles pour fournir des personnes de haute qualité aux ventes. Lisez [**Le Guide Définitif pour la notation des pistes**](https://www.marketo.com/definitive-guides/lead-scoring/){target="_blank"}.

1. Cliquez sur l&#39;onglet **[!UICONTROL Schedule]** et sur le bouton **[!UICONTROL Activer]** .

   ![](assets/simple-scoring-12.png)

1. Cliquez sur **[!UICONTROL Activer]** dans l’écran de confirmation.

   ![](assets/simple-scoring-13.png)

>[!NOTE]
>
>Une fois active, cette campagne s’exécute chaque fois qu’une personne remplit le formulaire. La campagne continue à s’exécuter jusqu’à ce qu’elle soit désactivée.

## Étape 2 : Remplir le formulaire {#step-fill-out-the-form}

1. Sélectionnez la landing page que vous avez créée dans la [Landing Page with a Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} gain rapide.

   ![](assets/simple-scoring-14.png)

1. Cliquez sur **[!UICONTROL Aperçu]**. La landing page s’ouvre dans un nouvel onglet.

   ![](assets/simple-scoring-15.png)

1. Remplissez le formulaire avec votre prénom, votre nom et votre adresse électronique, puis cliquez sur **[!UICONTROL Submit]**.

   ![](assets/simple-scoring-16.png)

   >[!NOTE]
   >
   >Utilisez le même nom et la même adresse email que ceux que vous avez utilisés lors de votre première inscription en tant que personne afin d&#39;appliquer l&#39;augmentation de score &quot;+5&quot;.

## Étape 3 : affichage des informations sur la personne {#step-view-the-person-info}

1. Accédez à la zone **[!UICONTROL Base de données]**.

   ![](assets/simple-scoring-17.png)

1. Recherchez l’adresse électronique que vous avez utilisée lors du remplissage du formulaire.

   ![](assets/simple-scoring-18.png)

1. Double-cliquez sur votre personne.

   ![](assets/simple-scoring-19.png)

Les détails de votre personne s’ouvrent dans un nouvel onglet ou une nouvelle fenêtre. Voyez comment votre score a augmenté de 5 points pour remplir le formulaire ?

![](assets/simple-scoring-20.png)

## Mission terminée ! {#mission-complete}

<br> 

[◄ Mission 2 : page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Mission 4 : ► de réponse automatique aux e-mails](/help/marketo/getting-started/quick-wins/email-auto-response.md)
