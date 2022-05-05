---
description: Étape 2 sur 3 - Création d’un utilisateur CRM Veeva pour Marketo Engage - Documents Marketo - Documentation du produit
title: Étape 2 sur 3 - Création d’un utilisateur CRM Veeva pour Marketo Engage
exl-id: 78945192-36b0-4e0b-830a-f37eb0b83484
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 4%

---

# Étape 2 sur 3 : Création d’un utilisateur CRM Veeva pour Marketo Engage {#step-2-of-3-create-a-veeva-crm-user-for-marketo-engage}

>[!NOTE]
>
>Les étapes de cet article doivent être réalisées par un administrateur CRM Veeva.

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : Ajout de champs Marketo à Salesforce (professionnel)](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-1-of-3-add-marketo-fields-to-veeva-crm.md){target=&quot;_blank&quot;}

Dans cet article, vous allez personnaliser les autorisations de champ avec une mise en page de page CRM Veeva et créer un utilisateur de synchronisation CRM Marketo-Veeva.

## Définition des mises en page {#set-page-layouts}

Suivez ces étapes pour permettre à l’utilisateur de synchronisation Marketo de mettre à jour les champs personnalisés.

1. Cliquez sur les mises en page de la page Compte (compte de personne) dans la barre de recherche de navigation sans appuyer sur Entrée, puis sur Mise en page de page sous Contacts.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-1.png)

1. Cliquez sur **Disposition de page**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-2.png)

1. Cliquez sur **HP - Professionnel**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-3.png)

1. Cliquez et faites glisser un nouveau **Section** dans la mise en page.

1. Saisissez &quot;Marketo&quot; pour le nom de la section, puis cliquez sur **OK**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-4.png)

1. Cliquez sur le champ Score et faites-le glisser dans la section Marketo .

   ![](assets/step-2-of-3-create-a-veeva-crm-user-5.png)

1. Répétez l’étape ci-dessus pour les champs suivants :

   * Ville déduite
   * Société déduite
   * Pays déduit
   * Aire métropolitaine déduite
   * Indicatif téléphonique local déduit
   * Code postal déduit
   * Région déduite

   >[!NOTE]
   >
   >Ces champs doivent être mis en page afin que Marketo puisse y lire/écrire.

   >[!TIP]
   >
   >Créez deux colonnes pour les champs en faisant glisser vers le bas à droite de la page. Vous pouvez déplacer les champs d&#39;un côté à l&#39;autre pour équilibrer la longueur des colonnes.

1. Lorsque vous avez terminé avec la mise en page professionnelle du réseau de gestion de la confidentialité, cliquez sur **Enregistrer**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-6.png)

>[!NOTE]
>
>Répétez cette opération pour les autres mises en page de page de compte.

## Création d’un profil {#create-a-profile}

1. Cliquez sur **Configuration**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-7.png)

1. Saisissez &quot;profils&quot; dans la barre de recherche de navigation, puis cliquez sur le bouton **Profils** lien.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-8.png)

1. Cliquez sur **Nouveau**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-9.png)

1. Sélectionnez Utilisateur standard, nommez le profil &quot;Synchronisation Marketo-Salesforce&quot; et cliquez sur **Enregistrer**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-10.png)

## Définition des autorisations de profil {#set-profile-permissions}

1. Cliquez sur **Modifier** pour définir les autorisations de sécurité.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-11.png)

1. Dans la section Autorisations administratives , assurez-vous que l’option API activée est sélectionnée.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-12.png)

   >[!TIP]
   >
   >Veillez à cocher la case Mot de passe n’expire jamais .

1. Dans la section Autorisations utilisateur générales , assurez-vous que Modifier les événements et Modifier les tâches sont sélectionnés.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-13.png)

1. Dans la section Autorisations d’objet standard , assurez-vous que les autorisations de lecture, de création, de modification et de suppression sont cochées pour les comptes et les contacts.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-14.png)

1. Dans la section Autorisations d’objet personnalisé , assurez-vous que les autorisations de lecture sont cochées pour Appel, Message de clé d’appel et tout autre objet personnalisé de votre choix.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-15.png)

1. Lorsque vous avez terminé, cliquez sur **Enregistrer** au bas de la page.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-16.png)

## Définition des autorisations de champ {#set-field-permissions}

1. Discutez avec vos spécialistes du marketing pour déterminer les champs personnalisés à synchroniser.

>[!NOTE]
>
>Cette étape permet d’éviter que les champs dont vous n’avez pas besoin ne s’affichent dans Marketo, ce qui réduit l’encombrement et accélère la synchronisation.

1. Dans la page des détails du profil, accédez à la section Sécurité au niveau du champ . Cliquez sur Afficher pour modifier l’accessibilité des objets Contact et Compte .

   ![](assets/step-2-of-3-create-a-veeva-crm-user-17.png)

>[!TIP]
>
>Vous pouvez configurer d’autres objets en fonction des besoins de votre entreprise.

1. Pour chaque objet, cliquez sur **Modifier**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-18.png)

Recherchez les champs inutiles, assurez-vous que les options Lecture d’accès et Modifier l’accès sont **un** coché. Cliquez sur **Enregistrer** une fois terminé.

![](assets/step-2-of-3-create-a-veeva-crm-user-19.png)

>[!NOTE]
>
>Modifiez uniquement l’accessibilité pour les champs personnalisés.

1. Une fois tous les champs inutiles désactivés, cochez les cases Lecture de l’accès et Modification de l’accès pour les champs d’objet suivants. Lorsque vous avez terminé, cliquez sur Enregistrer .

<table>
 <tbody>
  <tr>
   <th>Objet
   <th>Champs
  </tr>
  <tr>
   <td>Compte</td>
   <td>Champ de type</td>
  </tr>
  <tr>
   <td>Événement</td>
   <td>Tous les champs</td>
  </tr>
  <tr>
   <td>Tâche</td>
   <td>Tous les champs</td>
  </tr>
 </tbody>
</table>

## Créer un utilisateur de synchronisation {#create-sync-user}

Marketo nécessite des informations d’identification pour accéder à la gestion de la relation client de Veeva. Pour ce faire, il est préférable de créer un utilisateur dédié en suivant les étapes ci-dessous.

>[!NOTE]
>
>Si votre entreprise ne dispose d’aucune licence CRM Veeva supplémentaire, vous pouvez utiliser un utilisateur marketing existant avec le profil Administrateur système.

1. Saisissez &quot;Utilisateurs&quot; dans la barre de recherche de navigation, puis cliquez sur **Utilisateurs** sous Gérer les utilisateurs.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-20.png)

1. Cliquez sur **Nouvel utilisateur**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-21.png)

1. Renseignez les champs obligatoires, puis sélectionnez Licence utilisateur : Salesforce, définissez le profil : Utilisateur de synchronisation Marketo et cliquez sur **Enregistrer**.

   ![](assets/step-2-of-3-create-a-veeva-crm-user-22.png)

>[!TIP]
>
>Assurez-vous que l’adresse électronique saisie est valide. Vous devez vous connecter en tant qu’utilisateur de synchronisation pour réinitialiser le mot de passe.

Excellent ! Vous disposez à présent d’un compte que Marketo Engage peut utiliser pour se connecter à Veeva CRM. Faisons-le.

>[!MORELIKETHIS]
>
>[Étape 3 sur 3 : Connexion à Marketo et Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/setup/step-3-of-3-connect-marketo-engage-and-veeva-crm.md){target=&quot;_blank&quot;}
