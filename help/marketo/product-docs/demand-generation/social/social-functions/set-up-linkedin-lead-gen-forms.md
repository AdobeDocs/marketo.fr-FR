---
unique-page-id: 12976798
description: Configuration de LinkedIn Lead Gen Forms - Documentation Marketo - Documentation du produit
title: Configuration de LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: e1254c8156557b27d066a4482076becbd03fc774
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Configuration de LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Utilisez LinkedIn Lead Gen Forms pour exécuter des campagnes publicitaires dans LinkedIn et générer des pistes pour Marketo.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Un prospect LinkedIn n’apparaîtra pas dans Marketo Engage s’il correspond à un enregistrement de personne existant dans Marketo associé à un enregistrement de société créé à l’aide des API de société et que l’abonnement Marketo n’est pas connecté à un CRM.

1. Accéder à Marketo **Administration**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Accédez à **LaunchPoint**, cliquez sur **Nouveau** et sélectionnez **Nouveau service**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Saisissez un **Nom d’affichage** pour votre service, sélectionnez la variable **Gestionnaire de pistes linkedIn** dans la liste déroulante, puis cliquez sur **Suivant**.

   ![](assets/linkedin-lead-gen.png)

1. Marketo ouvre un nouvel onglet dans le même navigateur pour [linkedin.com](https://www.linkedin.com). Connectez-vous à LinkedIn à l’aide du compte que vous souhaitez utiliser pour l’intégration.

   >[!NOTE]
   >
   >Le compte LinkedIn doit avoir accès à tous les comptes commerciaux LinkedIn pour lesquels vous créez des campagnes sponsorisées.

   ![](assets/linkedin-login.png)

1. Une fois connecté à LinkedIn, revenez à Marketo et cliquez sur **Autoriser**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Lorsque vous y êtes invité, cliquez sur **Autoriser** pour accepter l’installation de l’application Marketo dans LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Vous remarquerez que vous êtes maintenant autorisé. Cliquez sur **Suivant**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >Le service expire automatiquement un an après l’autorisation. Pour récupérer l’accès, cliquez simplement sur **Réautorisation**. Vous devrez peut-être saisir à nouveau votre mot de passe LinkedIn, en fonction des paramètres de votre navigateur.

1. Sélectionnez le ou les comptes desquels vous souhaitez que les prospects LinkedIn viennent dans Marketo et cliquez sur **Suivant**.

   >[!TIP]
   >
   >Si vous ne voyez pas les comptes professionnels que vous attendez, assurez-vous que le compte LinkedIn de l’utilisateur autorisé dispose des autorisations du gestionnaire de formulaires Lead Gen sur le compte professionnel dans LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Pour accepter les mappages de champs LinkedIn vers Marketo par défaut, cliquez simplement sur **Créer**. Si vous souhaitez modifier le mapping de champ par défaut, supprimer un mapping de champ ou ajouter un nouveau mapping de champ, vous pouvez le faire par champ via le modal ci-dessous.

   >[!CAUTION]
   >
   >Marketo prend en charge le mappage de deux champs LinkedIn à un seul champ Marketo, **mais uniquement lorsque** les deux champs LinkedIn ne se présentent pas sous la même forme. Si vous mappez deux champs du même formulaire LinkedIn à un seul champ Marketo, il se peut que les utilisateurs ne puissent pas entrer dans votre base de données Marketo.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Seuls les champs LinkedIn qui ont déjà été enregistrés dans une [modèle de formulaire](https://www.linkedin.com/help/lms/answer/79634) dans LinkedIn Campaign Manager s’affichera sous forme de champs LinkedIn pouvant être mappés aux champs Marketo.

   ![](assets/linkedin-installed-services.png)

C&#39;est joli ! Les personnes qui envoient des formulaires de génération de pistes LinkedIn commencent à circuler dans Marketo lorsque vous lancez des campagnes réussies du côté LinkedIn.

>[!NOTE]
>
>Vous ne pouvez autoriser qu’un seul compte utilisateur LinkedIn. Si vous souhaitez lier plusieurs comptes professionnels à Marketo, assurez-vous que le compte LinkedIn de l’utilisateur autorisé dispose des autorisations du gestionnaire de formulaires Lead Gen sur le compte professionnel dans LinkedIn.

>[!MORELIKETHIS]
>
>[Utilisation des filtres de formulaire de génération de piste LinkedIn et des déclencheurs dans une campagne dynamique](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
