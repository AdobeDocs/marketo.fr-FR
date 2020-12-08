---
unique-page-id: 12976798
description: Configuration de LinkedIn Lead Gen Forms - Marketo Docs - Documentation du produit
title: Configurer LinkedIn Lead Gen Forms
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Configurer LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Utilisez LinkedIn Lead Gen Forms pour exécuter des campagnes publicitaires dans LinkedIn et générer des pistes pour Marketo.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à **l’administrateur** du marketing.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Accédez à **LaunchPoint**, cliquez sur **New** et sélectionnez **New Service**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Saisissez un nom **** d’affichage pour votre service, sélectionnez le service **LinkedIn Lead Gen **dans la liste déroulante, puis cliquez sur **Suivant**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo ouvre un nouvel onglet dans le même navigateur sur [www.linkedin.com](http://www.linkedin.com). Connectez-vous à LinkedIn en utilisant le compte que vous souhaitez utiliser pour l’intégration.

   >[!NOTE]
   >
   >Le compte LinkedIn doit avoir accès à tous les comptes professionnels LinkedIn pour lesquels vous créez des campagnes sponsorisées.

   ![](assets/linkedin-login.png)

1. Après vous être connecté à LinkedIn, retournez à Marketo et cliquez sur **Autoriser**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Lorsque vous y êtes invité, cliquez sur **Autoriser **pour accepter l’installation de l’application Marketo dans LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Vous remarquerez que vous êtes maintenant autorisé. Cliquez sur **Suivant**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Le service expire automatiquement un an après l&#39;autorisation. Pour récupérer l’accès, il vous suffit de cliquer sur **Réautorisation**. Vous devrez peut-être entrer de nouveau votre mot de passe LinkedIn, en fonction des paramètres de votre navigateur.

1. Sélectionnez le(s) compte(s) à partir duquel vous souhaitez que LinkedIn Lead Gen arrive sur le marché et cliquez sur **Suivant**.

   >[!TIP]
   >
   >Si vous ne voyez pas les comptes professionnels que vous attendez, assurez-vous que le compte LinkedIn de l&#39;utilisateur qui est autorisé dispose des autorisations du Gestionnaire de formulaires de génération de pistes sur le compte professionnel de LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Pour accepter les mappages de champs LinkedIn vers Marketo par défaut, cliquez simplement sur **Créer**. Si vous souhaitez modifier le mappage de champs par défaut, supprimer un mappage de champs ou ajouter un nouveau mappage de champs, vous pouvez le faire par champ via le modal ci-dessous.

   >[!CAUTION]
   >
   >Marketo prend en charge le mappage de deux champs LinkedIn sur un seul champ Marketo, **mais uniquement lorsque** les deux champs LinkedIn ne se trouvent pas sur le même formulaire. Si vous mappez deux champs du même formulaire LinkedIn à un seul champ Marketo, il se peut que les utilisateurs n’entrent pas dans votre base de données Marketo.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Seuls les champs LinkedIn qui ont déjà été enregistrés dans un modèle [de](https://www.linkedin.com/help/lms/answer/79634) formulaire dans LinkedIn Campaign Manager s’affichent en tant que champs LinkedIn qui peuvent être mappés aux champs Marketo.

   ![](assets/linkedin-installed-services.png)

Bien joué ! Les personnes qui envoient des formulaires de génération de pistes LinkedIn début vers Marketo lorsque vous exécutez des campagnes réussies du côté de LinkedIn.

>[!NOTE]
>
>Vous ne pouvez autoriser qu’un seul compte utilisateur LinkedIn. Si vous souhaitez lier plusieurs comptes professionnels à Marketo, assurez-vous que le compte LinkedIn de l’utilisateur qui est autorisé dispose des autorisations du Gestionnaire de formulaires de génération de pistes sur le compte professionnel dans LinkedIn.

>[!NOTE]
>
>**Articles connexes**
>
>* [Utiliser des Filtres de formulaire de génération de pistes LinkedIn et des déclencheurs dans un Campaign dynamique](use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)

>



