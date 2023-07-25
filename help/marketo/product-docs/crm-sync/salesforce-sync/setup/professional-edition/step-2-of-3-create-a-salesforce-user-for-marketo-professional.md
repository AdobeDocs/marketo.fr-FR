---
unique-page-id: 3571797
description: Étape 2 sur 3 - Création d’un utilisateur Salesforce pour Marketo (professionnel) - Documents Marketo - Documentation du produit
title: Étape 2 sur 3 - Création d’un utilisateur Salesforce pour Marketo (professionnel)
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 9%

---

# Étape 2 sur 3 : Création d’un utilisateur Salesforce pour Marketo (professionnel) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Ces étapes doivent être effectuées par un administrateur Salesforce

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : Ajout de champs Marketo à Salesforce (professionnel)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

Dans cet article, vous allez personnaliser les autorisations de champ avec une mise en page Salesforce et créer un utilisateur de synchronisation Marketo-Salesforce.

## Définition des mises en page {#set-page-layouts}

Salesforce Professional définit l’accessibilité au niveau du champ avec des mises en page, contrairement aux profils de Salesforce Enterprise/Unlimited. Suivez ces étapes pour permettre à l’utilisateur de synchronisation Marketo de mettre à jour les champs personnalisés.

1. Type **dispositions de page** dans la barre de recherche de navigation sans appuyer sur **Entrée**, puis cliquez sur **Disposition de page** under **Pistes**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Cliquez sur **Modifier** en regard de l’option Mise en page des pistes.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Cliquez et faites glisser un nouveau **Section** dans la mise en page.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Saisissez &quot;Marketo&quot; pour **Nom de la section** et cliquez sur **OK**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Cliquez et faites glisser le champ. **Date d’acquisition** dans la **Marketo** .

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Répétez l’étape ci-dessus pour les champs suivants :

   * Programme d&#39;acquisition
   * Identifiant du programme d’acquisition
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
   >Ces champs doivent être mis en page afin que Marketo puisse y lire/écrire.

   >[!TIP]
   >
   >Créez deux colonnes pour les champs en faisant glisser vers le bas à droite de la page. Vous pouvez déplacer les champs d&#39;un côté à l&#39;autre pour équilibrer la longueur des colonnes.

1. Cliquez sur **Enregistrer** lorsque vous avez terminé d’ajouter des champs.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Répétez toutes les étapes ci-dessus pour Salesforce **Disposition de la page de contact**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. N’oubliez pas de cliquer sur **Enregistrer** lorsque vous avez terminé avec la variable **Disposition de la page de contact**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >Assurez-vous que la variable **Événement de toute la journée** a été ajouté au champ **Disposition de la page Événement**.

## Créer un utilisateur de synchronisation {#create-sync-user}

Marketo nécessite des informations d’identification pour accéder à Salesforce. Pour ce faire, il est préférable de créer un utilisateur dédié en suivant les étapes ci-dessous.

>[!NOTE]
>
>Si votre entreprise ne dispose d’aucune licence Salesforce supplémentaire, vous pouvez utiliser une **Utilisateur marketing** avec le **Administrateur système** profile.

1. Saisissez &quot;Utilisateurs&quot; dans la barre de recherche de navigation, puis cliquez sur **Utilisateurs** under **Gestion des utilisateurs**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Cliquez sur **Nouvel utilisateur**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Renseignez les champs obligatoires, puis sélectionnez la variable **Licence utilisateur : Salesforce**, définissez la variable **Profil : Administrateur système**, vérifier **Utilisateur marketing** et cliquez sur **Enregistrer**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Assurez-vous que l’adresse électronique saisie est valide. Vous devez vous connecter en tant qu’utilisateur de synchronisation pour réinitialiser le mot de passe.

Excellent ! Vous disposez maintenant d’un compte que Marketo peut utiliser pour se connecter à Salesforce. Faisons-le.

>[!MORELIKETHIS]
>
>[Étape 3 sur 3 : Connexion de Marketo et Salesforce (professionnel)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
