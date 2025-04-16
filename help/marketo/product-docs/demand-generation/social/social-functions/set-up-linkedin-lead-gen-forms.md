---
unique-page-id: 12976798
description: Configuration de LinkedIn Lead Gen Forms - Documents Marketo - Documentation du produit
title: Configuration de LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 7a8f5146126d6e8a4902be9337eef4d51e108cf0
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Configuration de LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Utilisez LinkedIn Lead Gen Forms pour exécuter des campagnes publicitaires dans LinkedIn et générer des prospects pour Marketo.

>[!IMPORTANT]
>
>LinkedIn met à niveau ses API marketing utilisées par les intégrations LinkedIn de Marketo Engage. Ces modifications nécessiteront une réauthentification de tous les services LinkedIn LaunchPoint dans votre menu **Admin** > **LaunchPoint** entre le 7 juin et le 15 décembre 2024, afin d’éviter l’interruption du service. Pour plus d’informations, consultez le [FAQ sur la migration](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Un prospect LinkedIn n’apparaît pas dans Marketo Engage s’il correspond à un enregistrement de personne existant dans Marketo associé à un enregistrement d’entreprise créé à l’aide des API de l’entreprise et si l’abonnement à Marketo n’est pas associé à un CRM.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/set-up-linkedin-lead-gen-forms-1.png)

1. Accédez à **[!UICONTROL LaunchPoint]**, cliquez sur **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouveau service]**.

   ![](assets/set-up-linkedin-lead-gen-forms-2.png)

1. Saisissez un _Nom d’affichage_ pour votre service, sélectionnez le service **[!UICONTROL LinkedIn Lead Gen]** dans la liste déroulante, puis cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/set-up-linkedin-lead-gen-forms-3.png)

1. Marketo ouvre un nouvel onglet dans le même navigateur sur [linkedin.com](https://www.linkedin.com){target="_blank"}. Connectez-vous à LinkedIn à l’aide du compte que vous souhaitez utiliser pour l’intégration.

   >[!NOTE]
   >
   >Le compte LinkedIn doit avoir accès à tous les comptes professionnels LinkedIn pour lesquels vous créez des campagnes sponsorisées.

   ![](assets/set-up-linkedin-lead-gen-forms-4.png)

1. Une fois connecté à LinkedIn, revenez à Marketo et cliquez sur **[!UICONTROL Autoriser]**.

   ![](assets/set-up-linkedin-lead-gen-forms-5.png)

1. Lorsque vous y êtes invité, cliquez sur **[!UICONTROL Autoriser]** pour accepter l’installation de l’application Marketo dans LinkedIn.

   ![](assets/set-up-linkedin-lead-gen-forms-6.png)

1. Vous remarquerez que vous êtes désormais autorisé. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/set-up-linkedin-lead-gen-forms-7.png)

   >[!CAUTION]
   >
   >Le service expire automatiquement un an après l’autorisation. Pour récupérer l’accès, cliquez simplement sur **[!UICONTROL Réautoriser]**. Il se peut que vous deviez saisir à nouveau votre mot de passe LinkedIn, selon les paramètres de votre navigateur.

1. Sélectionnez le ou les comptes depuis lesquels vous souhaitez que les leads LinkedIn de génération de leads arrivent dans Marketo et cliquez sur **[!UICONTROL Suivant]**.

   >[!TIP]
   >
   >Si vous ne voyez pas les comptes professionnels attendus, assurez-vous que le compte LinkedIn de l’utilisateur autorisé dispose des autorisations de gestionnaire de formulaires gén. de leads pour le compte professionnel dans LinkedIn.

   ![](assets/set-up-linkedin-lead-gen-forms-8.png)

1. Pour accepter les mappages LinkedIn/champs Marketo par défaut, cliquez simplement sur **[!UICONTROL Créer]**. Si vous souhaitez modifier le mappage des champs par défaut, supprimer un mappage des champs ou ajouter un nouveau mappage des champs, vous pouvez le faire par champ à l’aide de la boîte de dialogue modale ci-dessous.

   >[!CAUTION]
   >
   >Marketo prend en charge le mappage de deux champs LinkedIn à un seul champ Marketo, _mais uniquement lorsque_ les deux champs LinkedIn ne se trouvent pas sur le même formulaire. Si vous mappez deux champs du même formulaire LinkedIn à un seul champ Marketo, il se peut que les utilisateurs ne saisissent pas votre base de données Marketo.

   ![](assets/set-up-linkedin-lead-gen-forms-9.png)

   >[!NOTE]
   >
   >Seuls les champs LinkedIn qui ont déjà été enregistrés dans un [modèle de formulaire](https://www.linkedin.com/help/lms/answer/79634){target="_blank"} dans LinkedIn Campaign Manager s’affichent sous la forme de champs LinkedIn pouvant être mappés sur des champs Marketo.

   ![](assets/set-up-linkedin-lead-gen-forms-10.png)

Bien joué ! Les personnes qui envoient des formulaires LinkedIn de génération de leads commenceront à affluer dans Marketo lorsque vous exécuterez des campagnes réussies du côté LinkedIn.

>[!NOTE]
>
>Vous ne pouvez autoriser qu’un seul compte utilisateur LinkedIn. Si vous souhaitez lier plusieurs comptes professionnels à Marketo, assurez-vous que le compte LinkedIn de l’utilisateur autorisé dispose des autorisations de gestionnaire de formulaires gén. de leads pour le compte professionnel dans LinkedIn.

>[!MORELIKETHIS]
>
>[Utilisation de filtres et de triggers de formulaires de génération de leads LinkedIn dans une campagne dynamique](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md){target="_blank"}
