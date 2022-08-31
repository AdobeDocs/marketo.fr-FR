---
unique-page-id: 2359414
description: Score simple - Documents Marketo - Documentation du produit
title: Évaluation simple
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
source-git-commit: 10637f7853c5b0f8a076779d95b8163b2de8abcb
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 8%

---

# Évaluation simple {#simple-scoring}

>[!PREREQUISITES]
>
>* [Configuration et ajout d’une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}


## Étape 1 : Créer une campagne d&#39;évaluation {#step-create-a-scoring-campaign}

1. Accédez au **Activités marketing** zone.

   ![](assets/simple-scoring-1.png)

1. Cliquez avec le bouton droit de la souris sur votre **Formation** et cliquez sur **Nouveau dossier Campaign**.

   ![](assets/simple-scoring-2.png)

1. Nommez le dossier de campagne &quot;Notation&quot; et cliquez sur **Créer**.

   ![](assets/simple-scoring-3.png)

   >[!NOTE]
   >
   >Si vous disposez déjà d’un dossier de notation, nommez celui-ci quelque chose de différent, tel que Scoring 1. Les noms de dossier doivent être uniques.

1. Cliquez avec le bouton droit de la souris sur votre **Notation** et sélectionnez **Nouvelle campagne dynamique**.

   ![](assets/simple-scoring-4.png)

1. Nommez la campagne &quot;Changer de score&quot; et cliquez sur **Créer**.

   ![](assets/simple-scoring-5.png)

1. Cliquez sur l&#39;onglet **Liste intelligente**.

   ![](assets/simple-scoring-6.png)

   Nous voulons que cette campagne s’exécute chaque fois qu’une personne remplit votre **Formulaire de demande d’évaluation**.

1. Recherchez et faites glisser le **Remplir le formulaire** se déclenche sur la zone de travail de gauche.

   ![](assets/simple-scoring-7.png)

1. Sélectionner **Mon formulaire**.

   ![](assets/simple-scoring-8.png)

   >[!NOTE]
   >
   >Si vous avez terminé la [Page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} gain rapide, vous devez avoir le formulaire. Si vous avez utilisé un autre nom pour votre formulaire, sélectionnez-le.

1. Cliquez sur l&#39;onglet **Flux**.

   ![](assets/simple-scoring-9.png)

1. Faites glisser le **Modifier le score** action de flux sur la zone de travail de gauche.

   ![](assets/simple-scoring-10.png)

1. Vous pouvez saisir n’importe quelle valeur à ajouter au score de la personne. Entrons &quot;+5&quot; dans le **Modifier** champ .

   ![](assets/simple-scoring-11.png)

   >[!TIP]
   >
   >De bonnes campagnes de notation sont essentielles pour fournir des personnes de haute qualité aux ventes. Lecture [**Guide définitif pour la notation des pistes**](https://www.marketo.com/definitive-guides/lead-scoring/){target=&quot;_blank&quot;}.

1. Cliquez sur le bouton **Planification** et le **Activer** bouton .

   ![](assets/simple-scoring-12.png)

1. Cliquez sur **Activer** sur l’écran de confirmation.

   ![](assets/simple-scoring-13.png)

>[!NOTE]
>
>Une fois principale, cette campagne s’exécute chaque fois qu’une personne remplit le formulaire. La campagne continue à s’exécuter jusqu’à ce qu’elle soit désactivée.

## Étape 2 : Remplir le formulaire {#step-fill-out-the-form}

1. Sélectionnez la landing page que vous avez créée dans le [Page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} gain rapide.

   ![](assets/simple-scoring-14.png)

1. Cliquez sur **Aperçu**. La landing page s’ouvre dans un nouvel onglet.

   ![](assets/simple-scoring-15.png)

1. Remplissez le formulaire avec votre prénom, votre nom et votre adresse électronique, puis cliquez sur **Envoyer**.

   ![](assets/simple-scoring-16.png)

   >[!NOTE]
   >
   >Utilisez le même nom et la même adresse email que ceux que vous avez utilisés lors de votre première inscription en tant que personne afin d&#39;appliquer l&#39;augmentation de score &quot;+5&quot;.

## Étape 3 : Affichage des informations sur la personne {#step-view-the-person-info}

1. Accédez à la zone Base de données .

   ![](assets/simple-scoring-17.png)

1. Recherchez l’adresse électronique utilisée lors du remplissage du formulaire.

   ![](assets/simple-scoring-18.png)

1. Double-cliquez sur votre personne.

   ![](assets/simple-scoring-19.png)

Les détails de votre personne s’ouvrent dans un nouvel onglet ou une nouvelle fenêtre. Voyez comment votre score a augmenté de 5 points pour remplir le formulaire ?

![](assets/simple-scoring-20.png)

## Mission accomplie! {#mission-complete}

<br> 

[◄ Mission 2 : Page de destination avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Mission 4 : Réponse e-mail automatique ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
