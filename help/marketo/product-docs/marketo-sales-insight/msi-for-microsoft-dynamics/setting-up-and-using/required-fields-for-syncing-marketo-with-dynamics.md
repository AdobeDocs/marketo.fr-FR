---
unique-page-id: 11375827
description: Champs obligatoires pour la synchronisation de Marketo avec Dynamics - Documents Marketo - Documentation du produit
title: Champs obligatoires pour la synchronisation de Marketo avec Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 3%

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

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Veillez à attendre au moins 10 minutes pour qu’une synchronisation s’exécute avant de vérifier que vous avez résolu le problème.

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de leads/contacts](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
