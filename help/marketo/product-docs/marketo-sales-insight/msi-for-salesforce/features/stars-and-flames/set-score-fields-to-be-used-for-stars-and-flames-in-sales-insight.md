---
unique-page-id: 2360301
description: Découvrez comment définir des champs de score pour les étoiles et les flammes dans Sales Insight. Mappez les champs de score Marketo à l’affichage MSI dans Salesforce.
title: Définir les champs de score à utiliser pour les étoiles et les flammes dans Informations sur les ventes
exl-id: 640f6d53-71ee-4a6d-b28a-82f3825b8f8e
feature: Marketo Sales Insights
source-git-commit: 03f984d4049c119267c7b2c2baa4e68c7db34ad0
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 10%

---

# Définir les champs de score à utiliser pour [!UICONTROL Stars] et [!UICONTROL Flames] dans [!DNL Sales Insight] {#set-score-fields-to-be-used-for-stars-and-flames-in-sales-insight}

>[!NOTE]
>
>**Autorisations d’administration requises**

Par défaut, [!DNL Marketo Sales Insight] utilise le champ **[!UICONTROL Score du lead]** pour calculer les étoiles et les flammes. Mais si vous souhaitez sélectionner un autre champ, procédez comme suit :

>[!TIP]
>
>Si vous ne disposez pas déjà de vos champs de score personnalisés, voici comment les [créer](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!NOTE]
>
>**Définition**
>
>* **[!UICONTROL Étoiles]** : les étoiles représentent le score total des prospects par rapport aux autres prospects.
>* **[!UICONTROL Flames]** : les flammes représentent l’urgence - à quel point le score d’un prospect a changé récemment.
>

1. Sous **[!UICONTROL Admin]**, cliquez sur **[!UICONTROL Insight commerciale]**.

   ![](assets/image2014-9-16-13-3a27-3a19.png)

1. Sous **[!UICONTROL Paramètres de notation des leads]**, cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/image2014-9-16-13-3a27-3a33.png)

1. Sélectionnez le champ à utiliser pour **[!UICONTROL Étoiles]**.

   ![](assets/image2014-9-16-13-3a27-3a45.png)

1. Sélectionnez le champ à utiliser pour **[!UICONTROL Flammes]**.

   ![](assets/image2014-9-16-13-3a28-3a1.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/image2014-9-16-13-3a28-3a18.png)

   >[!NOTE]
   >
   >[!DNL Sales insight] faudra un certain temps pour le recalculer. Vous pouvez vérifier votre CRM plus tard pour voir les étoiles et les flammes.

   >[!MORELIKETHIS]
   >
   >[Priorité, urgence, score relatif et meilleurs résultats](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
