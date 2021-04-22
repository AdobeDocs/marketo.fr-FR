---
unique-page-id: 3571797
description: Étape 2 sur 3 - Créer un utilisateur Salesforce pour Marketo (Professional) - Marketo Docs - Documentation sur les produits
title: Etape 2 sur 3 - Création d’un utilisateur Salesforce pour Marketo (Professional)
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 9%

---

# Étape 2 sur 3 : Créer un utilisateur Salesforce pour Marketo (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Ces étapes doivent être effectuées par un administrateur Salesforce.

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : Ajouter les champs Marketo à Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

Dans cet article, vous allez personnaliser les autorisations de champ avec une mise en page de page Salesforce et créer un utilisateur de synchronisation Marketo-Salesforce.

## Définir les mises en page {#set-page-layouts}

Salesforce Professional définit l&#39;accessibilité au niveau des champs avec les mises en page, contrairement aux Profils de Salesforce Enterprise/Unlimited. Suivez ces étapes pour permettre à l’utilisateur de la synchronisation Marketo de mettre à jour les champs personnalisés.

1. Tapez **dispositions de page** dans la barre de recherche Nav sans appuyer sur **Entrée**, puis cliquez sur **Mise en page** sous **Pistes**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Cliquez sur **Modifier** en regard de Disposition de piste.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Cliquez et faites glisser une nouvelle **section** dans la mise en page.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Saisissez &quot;Marketo&quot; pour **Nom de la section** et cliquez sur **OK**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Cliquez et faites glisser le champ **Date d’acquisition** dans la section **Marketo**.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Répétez l’étape ci-dessus pour les champs suivants :

   * Programme d&#39;acquisition
   * ID de Programme d’acquisition
   * Désabonnement par e-mail
   * Ville déduite
   * Société déduite
   * Pays déduit
   * Aire métropolitaine déduite
   * Indicatif téléphonique local déduit
   * Code postal déduit
   * Région déduite
   * Évaluation des leads
   * Référent d&#39;origine
   * Moteur de recherche d&#39;origine
   * Phrase de recherche d&#39;origine
   * Info source d&#39;origine
   * Type source d&#39;origine

   >[!NOTE]
   >
   >Ces champs doivent figurer sur la mise en page pour que Marketo puisse les lire/écrire.

   >[!TIP]
   >
   >Créez deux colonnes pour les champs en faisant glisser le curseur vers le côté droit de la page. Vous pouvez déplacer les champs d’un côté à l’autre pour équilibrer les longueurs de colonne.

1. Cliquez sur **Enregistrer** une fois l’ajout de champs terminé.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Répétez toutes les étapes ci-dessus pour le Salesforce **Mise en page de la page de contact**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Pensez à cliquer sur **Enregistrer** lorsque vous avez terminé avec la **Mise en page de la page de contact**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >Assurez-vous que le champ **Événement de toute la journée** a été ajouté à la **Mise en page du Événement**.

## Créer un utilisateur de synchronisation {#create-sync-user}

Marketo a besoin d&#39;informations d&#39;identification pour accéder à Salesforce. Pour ce faire, il est préférable d’utiliser un utilisateur dédié créé en suivant les étapes ci-dessous.

>[!NOTE]
>
>Si votre entreprise ne dispose pas de licences Salesforce supplémentaires, vous pouvez utiliser un **utilisateur marketing** existant avec le profil **Administrateur système**.

1. Saisissez &quot;users&quot; dans la barre de recherche Nav, puis cliquez sur **Utilisateurs** sous **Gérer les utilisateurs**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Cliquez sur **Nouvel utilisateur**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Renseignez les champs obligatoires, sélectionnez la **Licence utilisateur : Salesforce**, définissez le **Profil : Administrateur système**, cochez **Utilisateur marketing** et cliquez sur **Enregistrer**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Assurez-vous que l’adresse électronique saisie est valide. Vous devez vous connecter en tant qu’utilisateur de synchronisation pour réinitialiser le mot de passe.

Excellent ! Vous disposez maintenant d’un compte que Marketo peut utiliser pour se connecter à Salesforce. Faisons-le.

>[!MORELIKETHIS]
>
>[Étape 3 sur 3 : Connecter Marketo et Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
