---
description: Comment personnaliser les en-têtes HTTP pour les domaines de page de destination, y compris Strict-Transport-Security et X-Frame-Options.
title: En-têtes de page de destination
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
TQID: https://experienceleague.adobe.com/ecRuR4V-YCsesHZpm9UrP1rPlOjBCediq-9DtXZRfBo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 147
ht-degree: 4%

---

# En-têtes de page de destination {#landing-page-headers}

Suivez les étapes ci-dessous pour personnaliser certains des en-têtes HTTP sur vos domaines de page de destination.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/landing-page-headers-1.png)

1. Cliquez sur **[!UICONTROL Pages de destination]**.

   ![](assets/landing-page-headers-2.png)

1. Cliquez sur **[!UICONTROL Modifier]** en regard de En-têtes HTTP de page de destination.

   ![](assets/landing-page-headers-3.png)

1. Choisissez les paramètres souhaités et cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[!UICONTROL Strict-Transport-Security]</strong></td>
  <td>Utilisez ceci pour garantir que les connexions aux landing pages seront toujours diffusées via HTTPS (ne doit être défini que pour les abonnements dont les landing pages sont sécurisées par SSL)</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL X-Frame-Options]</strong></td>
  <td>Permet de définir si les ressources hébergées par Marketo Engage peuvent être incorporées dans des pages web externes</td>
 </tr>
</table>

>[!CAUTION]
>
>Il est important de passer en revue ces paramètres avec votre équipe informatique afin de déterminer la stratégie de votre entreprise. Des paramètres incorrects peuvent empêcher certains visiteurs d’accéder à vos pages de destination.
