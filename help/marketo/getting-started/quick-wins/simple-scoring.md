---
unique-page-id: 2359414
description: Scores simples - Documents marketing - Documentation du produit
title: Score simple
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Score simple {#simple-scoring}

>[!PREREQUISITES]
>
>* [Configurer et Ajouter une personne](get-set-up-and-add-a-person.md)
>* [landing page avec un formulaire](landing-page-with-a-form.md)


## Étape 1 : Créer un Campaign de score {#step-create-a-scoring-campaign}

1. Accédez à la zone **Activités marketing**.

   ![](assets/ma-1.png)

1. Cliquez avec le bouton droit sur votre dossier **Apprentissage** et cliquez sur **Nouveau dossier de campagne**.

   ![](assets/two-2.png)

1. Nommez le dossier de campagne &quot;Score&quot;.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Si vous disposez déjà d’un dossier Scoring, nommez celui-ci quelque chose de différent, tel que Scoring 1. Les noms de dossiers doivent être uniques.

1. Cliquez ensuite avec le bouton droit de la souris sur votre nouveau dossier **Scoring** et sélectionnez **New Smart Campaign**.

   ![](assets/four.png)

1. **Nommez** la campagne &quot;Changer de note&quot; et cliquez sur  **Créer**.

   ![](assets/five-1.png)

1. Cliquez sur l&#39;onglet **Liste intelligente**.

   ![](assets/six-1.png)

   Nous voulons que cette campagne s’exécute chaque fois qu’une personne remplit votre **Formulaire de demande d’évaluation**.

1. Recherchez et faites glisser le déclencheur **Remplit le formulaire** sur le canevas de gauche.

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. Sélectionnez **Mon formulaire**.

   >[!NOTE]
   >
   >Si vous avez complété le [Landing page avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) gain rapide, vous devez avoir le formulaire. Si vous avez utilisé un autre nom pour votre formulaire, sélectionnez-le.

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. Cliquez sur l&#39;onglet **Flux**.

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. Faites glisser l’action d’enchaînement **Changer la note** sur le canevas de gauche.

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. Vous pouvez entrer n’importe quelle valeur à ajouter à la note de la personne. Saisissez &quot;+5&quot; dans le champ **Modifier**.

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >Les campagnes de notation de qualité sont essentielles pour fournir des personnes de qualité aux ventes. Consultez le [**Guide de définition du score de piste**](https://www.marketo.com/definitive-guides/lead-scoring/).

1. Cliquez sur l&#39;onglet **Planification** et sur le bouton **Activer**.

   ![](assets/twelve-1.png)

1. Cliquez sur **Activer** dans l’écran de confirmation.

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>Une fois principale, cette campagne s’exécute chaque fois qu’une personne remplit le formulaire. La campagne continue à s’exécuter jusqu’à ce qu’elle soit désactivée.

## Étape 2 : Remplir le formulaire {#step-fill-out-the-form}

1. Sélectionnez le landing page que vous avez créé dans le Landing page [avec une victoire rapide Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md).

   ![](assets/fourteen-1.png)

1. Cliquez sur **Vue Page approuvée**. Le landing page s’ouvre dans un nouvel onglet.

   ![](assets/image2014-9-24-11-3a47-3a51.png)

1. Remplissez le formulaire avec votre prénom, votre nom et votre adresse électronique, puis cliquez sur **Envoyer**.

   ![](assets/image2014-9-24-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Utilisez le même nom et la même adresse électronique que ceux que vous avez utilisés lors de votre première inscription en tant que personne afin d’appliquer l’augmentation de score &quot;+5&quot;.

## Étape 3 : Vue des informations sur la personne {#step-view-the-person-info}

1. Accédez à la zone Base de données.

   ![](assets/db-2.png)

1. Recherchez l’adresse électronique que vous avez utilisée lors du remplissage du formulaire.

   ![](assets/eighteen.png)

1. Doublon-cliquez sur votre personne.

   ![](assets/nineteen.png)

Les détails de votre personne s&#39;ouvriront dans un nouvel onglet ou une nouvelle fenêtre. Voyez comment votre score a augmenté de 5 points pour remplir le formulaire ? !

![](assets/twenty.png)

**Félicitations !** Vous avez créé une campagne de score.
[Mission 2 : landing page avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Mission 4 : ► Réponse automatique par courriel](/help/marketo/getting-started/quick-wins/email-auto-response.md)
