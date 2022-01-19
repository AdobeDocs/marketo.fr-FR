---
description: Clone push - Documents Marketo - Documentation du produit
title: Clonage push
hide: true
hidefromtoc: true
source-git-commit: 8920bc525075923b32e7330da20debb7b8f47b06
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Clonage push {#push-clone}

Cette fonctionnalité vous permet de transférer les segments situés dans votre Adobe Experience Platform vers Marketo sous la forme d’une liste statique.

>[!PREREQUISITES]
>
>* [Création d’un utilisateur API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) dans Marketo.
>* Ensuite, accédez à **Administration** > **Launchpoint**. Recherchez le nom du rôle que vous venez de créer, puis cliquez sur **Afficher les détails**. Copiez et enregistrez les informations dans **ID client** et **Secret du client**, car vous en aurez besoin pour cette fonctionnalité.


1. Connectez-vous à [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. Cliquez sur l’icône de grille et sélectionnez **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. Dans le volet de navigation de gauche, cliquez sur **Destinations**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. Cliquez sur **Catalogue**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. Recherchez la mosaïque Marketo Engage et cliquez sur **Activation des segments**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. Cliquez sur **Configuration d’une nouvelle destination**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. Sous Type de compte, sélectionnez le bouton radio Compte existant ou Nouveau compte (dans cet exemple, nous choisissons **Compte existant**). Cliquez sur l’icône Sélectionner un compte .

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

1. Sélectionnez le compte de destination et cliquez sur **Sélectionner**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

Vous devrez ensuite choisir si vous souhaitez faire correspondre uniquement les personnes Marketo existantes ou les personnes Marketo existantes et créer les personnes manquantes dans Marketo. Vous trouverez, ci-dessous, des sections décrivant la procédure à suivre.

## Faire correspondre les personnes Marketo existantes et créer des personnes manquantes dans Marketo {#match-existing-marketo-people-create-missing-people}

Après les étapes 1 à 8 ci-dessus...

1. Entrer une destination **Nom** et une description facultative. Cliquez sur la liste déroulante Création de personne et sélectionnez **Faire correspondre les personnes Marketo existantes et créer des personnes manquantes dans Marketo**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

1. Cette section est facultative. Cliquez sur **Créer** pour ignorer.

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. Sélectionnez la destination que vous avez créée, puis cliquez sur **Suivant**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Sélectionnez le segment à envoyer à Marketo, puis cliquez sur **Suivant**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

1. Cliquez sur **Ajouter un nouveau mappage**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. Cliquez sur l’icône de mappage.

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. Faites correspondre le prénom en sélectionnant **firstName** et clic **Sélectionner**.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

1. Faites correspondre le nom de famille et le nom de la société en cliquant sur **Ajouter un nouveau mappage** et répétez l’étape 7 deux fois, en choisissant lastName , puis companyName.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. Il est maintenant temps de mapper l&#39;adresse email. Cliquez sur **Ajouter un nouveau mappage** encore une fois.

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. Cliquez sur l’icône de mappage.

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. Cliquez sur le bouton radio Sélectionner un espace de noms d’identité , choisissez  **Email**, puis cliquez sur **Sélectionner**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

1. Il est maintenant temps de choisir les champs sources. Pour envoyer un courrier électronique, cliquez sur l’icône représentant un curseur.

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. Cliquez sur le bouton radio Sélectionner un espace de noms d’identité , recherchez et sélectionnez **Email**, puis cliquez sur **Sélectionner**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

MORREEEE

## Correspondance avec les personnes Marketo existantes uniquement {#match-existing-marketo-people-only}

>[!NOTE]
>
>Les identités sont utilisées pour rechercher des correspondances dans Marketo. Si une correspondance est trouvée, la personne est ajoutée à la liste statique. Si aucune correspondance n’est trouvée, ces personnes sont ignorées (c’est-à-dire qu’elles ne sont pas créées dans Marketo).

1. _Dans Marketo_, créez une liste statique ou recherchez et sélectionnez-en une que vous avez déjà créée. Copiez l’ID de mappage à partir de la fin de l’URL.

PICC

>[!NOTE]
>
>Pour de meilleurs résultats, assurez-vous que la liste que vous référencez dans Marketo est vide.

1. De retour dans Adobe Experience Platform, saisissez l’identifiant que vous venez de copier. Sélectionnez votre Date de début. Les utilisateurs se synchronisent en permanence jusqu’à la date de fin choisie. Pour une synchronisation indéfinie, laissez la date de fin vide. Cliquez sur **Suivant** une fois terminé.

PICC

1. Confirmez vos modifications et cliquez sur **Terminer**.

PICC
