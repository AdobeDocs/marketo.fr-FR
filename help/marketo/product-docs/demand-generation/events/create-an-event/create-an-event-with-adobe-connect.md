---
unique-page-id: 2949865
description: Création d’un événement avec Adobe Connect - Documents Marketo - Documentation du produit
title: Création d’un événement avec Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Création d’un événement avec Adobe Connect {#create-an-event-with-adobe-connect}

La synchronisation avec Adobe Connect vous permet de gérer l’inscription et la participation à vos webinaires dans Marketo, ce qui garantit que l’engagement ne sera pas désuivi.

>[!PREREQUISITES]
>
>* [Lier Adobe Connect et Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Créer un programme d’événement](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)

Tout d’abord, assurez-vous d’avoir créé votre réunion ou séminaire dans Adobe Connect. Si vous avez besoin d’aide, consultez le [Guide de l’utilisateur d’Adobe Connect](https://help.adobe.com/en_US/connect/9.0/using/index.html).

Les réunions et séminaires que vous créez dans Adobe Connect doivent être créés dans le dossier que vous avez spécifié lorsque vous avez saisi vos informations d’identification dans Marketo. Après avoir créé votre réunion ou séminaire, prenez note des informations logistiques pertinentes (telles que le numéro de téléphone), à utiliser dans votre email de confirmation et votre fichier ICS.

>[!CAUTION]
>
>En tant qu’hôte d’événement, veillez à rejoindre depuis l’application et **not** via le lien envoyé aux participants.

>[!NOTE]
>
>Actuellement, Adobe Connect On-Site n’est pas pris en charge.

1. Sur l’accueil d’un nouvel événement, sélectionnez **Actions d’événement**, puis **Paramètres d’événement**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Si vous ne voyez pas **Paramètres d’événement** dans la liste déroulante, assurez-vous que l’option **Événement avec webinaire** est sélectionnée sous &quot;S’applique à&quot; dans le canal de l’événement.

1. Sous **Event Partner**, sélectionnez **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Sélectionnez votre **ID de connexion** et choisissez votre **Événement**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/event-settings-overview.png)

   Beau ! Votre événement Adobe Connect est maintenant synchronisé avec votre événement Marketo.

   >[!NOTE]
   >
   >Les champs que Marketo envoie sont les suivants : Prénom, Nom, Adresse électronique.

   >[!TIP]
   >
   >Pour insérer l’URL unique de la personne dans un email, utilisez ce jeton : `{{member.webinar url}}`. Lorsque l’email est envoyé, ce jeton résout automatiquement l’URL de confirmation unique de la personne à partir d’Adobe Connect.
   >
   >Définissez votre email de confirmation sur **Operational** pour vous assurer que les personnes qui s&#39;inscrivent et peuvent se désabonner reçoivent toujours leurs informations de confirmation.

   Les personnes qui s’inscrivent à votre webinaire seront transférées à votre fournisseur de webinaires via l’étape de flux Modifier l’état du programme lorsque le nouvel état est défini sur &quot;Enregistré&quot;. Aucun autre statut ne repoussera la personne. Assurez-vous également d’effectuer l’étape de flux Modifier l’état du programme #1 et l’étape Envoyer un courrier électronique #2.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Évitez d’utiliser des programmes de messagerie imbriqués pour envoyer vos emails de confirmation. Utilisez plutôt la campagne dynamique du programme d’événements, comme illustré ci-dessus.

   >[!TIP]
   >
   >L’affichage des données dans Marketo peut prendre jusqu’à 48 heures. Si, après avoir attendu si longtemps, rien ne s’affiche toujours, sélectionnez **Actualiser à partir du fournisseur de webinaires** dans le menu Actions d’événement de l’onglet Résumé de votre événement.

   >[!MORELIKETHIS]
   >
   >* [Ajouter Adobe Connect as a LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Modifier un canal d’événement](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)
