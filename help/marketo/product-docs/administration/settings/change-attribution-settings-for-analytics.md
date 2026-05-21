---
unique-page-id: 2360217
description: Comment définir les options d’attribution première touche et multipoint, de conversion de piste et d’opportunité influencée par le marketing dans Revenue Cycle Analytics.
title: Modifier les paramètres d’attribution dans Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
TQID: https://experienceleague.adobe.com/AjpEYRzLKRQQsTmYdQUvAVnlcmG-Q6nbVjaZCuQYaUc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2:
  - id: e5d29014-8a81-4c0c-845b-2adc7a5d6258
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 5%

---

# Modifier les paramètres d’attribution dans Analytics {#change-attribution-settings-for-analytics}

Vous pouvez modifier la manière dont Marketo lie les contacts aux opportunités d’attribution première touche et multitouche, aux mesures de conversion des prospects et à l’indicateur d’opportunité influencé par le marketing.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Cliquez sur **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Cliquez sur le lien **[!UICONTROL Modifier]** sous **[!UICONTROL Attribution]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >La modification de ce paramètre ne modifie aucune donnée Marketo ; elle modifie la façon dont vos rapports s’exécutent. Cette opération peut être annulée à tout moment.

1. Sélectionnez une option et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Définition**
   >
   >**[!UICONTROL Explicite]** : contacts avec des rôles uniquement (par défaut).
   >
   >**[!UICONTROL Hybride]** : contacts avec des rôles, le cas échéant. Si aucun contact n’est disponible, il utilise tous les contacts des comptes.
   >
   >**[!UICONTROL Implicite]** : tous les contacts, quel que soit leur rôle.

>[!CAUTION]
>
>Lors de l’utilisation de **[!UICONTROL Implicite]**, Marketo examine toujours tous les contacts associés au compte, quel que soit le rôle. **Marketo recommande vivement d&#39;utiliser le mode [!UICONTROL Explicit]**. L’utilisation de [!UICONTROL Implicite] peut créer des faux positifs, c’est-à-dire des personnes qui ont du crédit pour une opportunité alors qu’elles n’ont aucune influence réelle sur celle-ci. Utilisez [!UICONTROL Implicite] avec précaution.
