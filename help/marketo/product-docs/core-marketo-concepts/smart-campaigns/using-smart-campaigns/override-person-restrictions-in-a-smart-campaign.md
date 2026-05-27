---
unique-page-id: 1147066
description: Découvrez comment remplacer les restrictions de personne dans une campagne dynamique. Autoriser les utilisateurs à exécuter même s’ils atteignent les limites de communication.
title: Ignorer les restrictions de personnes dans une campagne intelligente
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/GUIwrHBCrtl5NONZAqCY9sXt1FaLfjBwe3N3t1u98a4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 9%

---

# Ignorer les restrictions de personnes dans une campagne intelligente {#override-person-restrictions-in-a-smart-campaign}

Marketo Engage vous permet de définir le nombre maximal de personnes pouvant se qualifier pour une campagne dynamique. Vous pouvez ainsi éviter d’envoyer accidentellement par e-mail l’ensemble de votre base de données. Si vous souhaitez _contourner_ cette limite, procédez comme suit.

>[!PREREQUISITES]
>
>Veillez à [activer les restrictions de personne pour les campagnes intelligentes](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} dans Marketo Admin.

1. Dans **[!UICONTROL Activités marketing]**, accédez à votre campagne intelligente et cliquez sur **[!UICONTROL Planifier]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. Dans les paramètres de campagne intelligente, cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >La limite par défaut est celle définie dans Admin.

1. Saisissez une nouvelle limite et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   La campagne intelligente ne s’exécute pas si le nombre de personnes remplissant les conditions requises dépasse la limite définie.

   >[!CAUTION]
   >
   >Faites attention avec cette fonctionnalité afin de ne pas inclure accidentellement trop de personnes.
