---
unique-page-id: 42762511
description: Configuration du mappage de l’organisation Adobe - Documents Marketo - Documentation du produit
title: Configuration du mappage de l’organisation Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: 22f46fedc90d064bd7fbe6f7d5e4621de0b83718
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Configuration du mappage de l’organisation Adobe {#set-up-adobe-organization-mapping}

Pour vous synchroniser avec les applications Adobe, telles que Audience Manager, le connecteur Marketo CDP B2B, Dynamic Chat, etc., vous devez d’abord saisir vos informations d’identification Adobe IMS Org dans Marketo.

>[!NOTE]
>
>Un déploiement prêt pour la HIPAA d’une instance Marketo ne peut pas utiliser cette intégration.

>[!CAUTION]
>
>Pour les clients intégrés à Adobe Business Platform et à Identity Management System, l’ID d’organisation associé à l’abonnement sera déjà renseigné et est un champ en lecture seule.

1. Dans Marketo, cliquez sur **Administration**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Sous Intégration, cliquez sur **Mappage de l’organisation Adobe**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Cliquez sur **Modifier**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Saisissez votre identifiant de l’organisation Adobe IMS (découvrez comment le trouver). [here](https://experienceleague.adobe.com/docs/control-panel/using/faq.html)) et cliquez sur **OK**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Cliquez sur **Confirmer**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Cliquez sur **Fermer**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Pour des raisons de sécurité, vous devez être un administrateur d’organisation pour l’organisation Adobe à laquelle vous souhaitez mapper. Si ce n’est pas le cas, l’action échouera. En outre, l’utilisateur Adobe et l’utilisateur Marketo doivent utiliser la même adresse électronique lors de la connexion.

1. Si vous êtes _not_ déjà connecté, une fenêtre contextuelle s’affiche dans un nouvel onglet/fenêtre. Connectez-vous à l’organisation de votre Adobe (cette action valide l’accès de l’organisation).

Et voilà ! Vous pouvez désormais [partage des données d’audience](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target=&quot;_blank&quot;} vers ou [synchronisation d’une audience](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target=&quot;_blank&quot;} à partir de Adobe Experience Cloud.