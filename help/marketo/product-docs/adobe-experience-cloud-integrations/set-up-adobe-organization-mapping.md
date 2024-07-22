---
unique-page-id: 42762511
description: Configuration du mappage de l’organisation Adobe - Documents Marketo - Documentation du produit
title: Configuration du mappage de l’organisation Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Configuration du mappage de l’organisation Adobe {#set-up-adobe-organization-mapping}

Pour vous synchroniser avec les applications Adobe, telles que l’Audience Manager, le connecteur Marketo CDP B2B, [!DNL Dynamic Chat], etc., vous devez d’abord saisir vos informations d’identification Adobe IMS Org dans Marketo Engage.

>[!NOTE]
>
>* Un déploiement prêt pour la HIPAA d’une instance Marketo ne peut pas utiliser cette intégration.
>* Pour que l’intégration fonctionne, Marketo et vos autres applications Adobe doivent se trouver dans la même organisation.

>[!IMPORTANT]
>
>Pour les utilisateurs intégrés à Adobe Business Platform et à Identity Management System, l’ID d’organisation associé à l’abonnement sera déjà renseigné et est un champ en lecture seule. Les étapes du présent article ne s&#39;appliqueraient donc pas.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Sous Intégration, cliquez sur **[!UICONTROL Adobe le mappage de l’organisation]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Saisissez votre ID d’organisation Adobe IMS (apprenez à trouver cet [ici](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"}) et cliquez sur **[!UICONTROL OK]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Cliquez sur **[!UICONTROL Confirmer]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Pour des raisons de sécurité, vous devez être un administrateur d’organisation pour l’organisation Adobe à laquelle vous souhaitez mapper. Si ce n’est pas le cas, l’action échouera. En outre, l’utilisateur Adobe et l’utilisateur Marketo doivent utiliser la même adresse électronique lors de la connexion.

1. Si vous n’êtes _pas_ déjà connecté, une fenêtre contextuelle s’affiche dans un nouvel onglet/fenêtre. Connectez-vous à l’organisation de votre Adobe (cette action valide l’accès de l’organisation).

Et c&#39;est tout ! Vous pouvez désormais [ partager des données d’audience](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} sur ou [synchroniser une audience](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} à partir de Adobe Experience Cloud.
