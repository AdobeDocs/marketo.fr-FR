---
unique-page-id: 11375827
description: Découvrez les champs requis pour synchroniser Marketo avec Dynamics. Assurez-vous que les champs appropriés sont mappés pour que MSI fonctionne correctement.
title: Champs requis pour la synchronisation de Marketo avec Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
TQID: 'https://experienceleague.adobe.com/2MpYFkohrwAJ20pKL9zISg2b0jTqougMaRLYJFYHbQs'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: 62f69a42-2389-532a-9af6-0e08fdaa397f
    internal-label: Marketo Sales Insights
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 7%
---
# Champs obligatoires pour la synchronisation de Marketo avec [!DNL Dynamics] {#required-fields-for-syncing-marketo-with-dynamics}

Ces champs *doivent* doivent être synchronisés avec Marketo pour [!UICONTROL Lead] et [!UICONTROL Contact] pour que [!DNL Sales Insight] fonctionne :

* Priorité
* Urgence
* Évaluation relative

Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour résoudre ce problème, archivez votre instance afin de vous assurer que les champs sont synchronisés pour **[!UICONTROL Lead]** et **[!UICONTROL Contact]**. Sinon, ajoutez-les.

Voici comment vérifier et ajouter des champs de synchronisation.

1. Accédez à [!UICONTROL Admin] et cliquez sur **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **[!UICONTROL Modifier]** sur [!UICONTROL Détails de la synchronisation des champs].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Sous [!UICONTROL Lead], cochez la case [!UICONTROL Priorité].

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Maintenant, faites défiler vers le bas et cochez la case [!UICONTROL Urgence]...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...et la case [!UICONTROL Score relatif].

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Ensuite, cochez les cases correspondant à [!UICONTROL Priorité], [!UICONTROL Urgence] et [!UICONTROL Score relatif] pour [!UICONTROL Contact].

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Veillez à attendre au moins 10 minutes pour qu’une synchronisation s’exécute avant de vérifier que vous avez résolu le problème.

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de leads/contacts](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
