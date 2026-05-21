---
description: Découvrez comment créer des tâches dans Veeva à partir de Marketo pour informer les ventes de ce qu’il faut faire et quand. Utilisez l’étape Créer un flux de tâches et personnalisez l’objet, la description et la date d’échéance.
title: Créez une tâche dans  [!DNL Veeva]
exl-id: 342e45dd-2038-432d-a6b6-1740c8f0b58e
feature: Veeva CRM
TQID: https://experienceleague.adobe.com/W4zIWswN64cHyqA7oQ9iku0iMC7Q6NqIpWiAcSgvD04
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 0%

---

# Créer une tâche dans [!DNL Veeva] {#create-task-in-veeva}

En tant que spécialiste marketing, vous disposez d’informations qui peuvent aider les ventes à conclure des offres. Vous pouvez créer des tâches pour leur indiquer ce qu’elles doivent faire et quand elles doivent le faire.

![](assets/create-task-in-veeva-1.png)

>[!NOTE]
>
>Lorsque l’utilisateur de la synchronisation Marketo crée des tâches, le champ **[!UICONTROL Échéance en cours]** est obligatoire pour que la tâche soit créée en [!DNL Veeva]. Marketo saisit cinq jours par défaut s’il n’existe aucune valeur.

Par défaut, l’étape de flux se présente comme suit :

![](assets/create-task-in-veeva-2.png)

Personnalisez tous les champs pour créer la tâche comme vous le souhaitez.

![](assets/create-task-in-veeva-3.png)

>[!TIP]
>
>Vous pouvez utiliser `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` et `{{system.tokens}}` dans les [!UICONTROL Objet] et [!UICONTROL Description]. Voir [Jetons pour les étapes de flux](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} pour plus d’informations.
