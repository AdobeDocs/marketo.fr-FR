---
description: En-têtes de page d’entrée - Documents Marketo - Documentation du produit
title: En-têtes de page d’entrée
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---

# En-têtes de page d’entrée {#landing-page-headers}

Suivez les étapes ci-dessous pour personnaliser certains en-têtes HTTP de vos domaines de page d’entrée.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/landing-page-headers-1.png)

1. Cliquez sur **[!UICONTROL Landing Pages]**.

   ![](assets/landing-page-headers-2.png)

1. Cliquez sur **[!UICONTROL Modifier]** en regard des en-têtes HTTP de page d’entrée.

   ![](assets/landing-page-headers-3.png)

1. Choisissez les paramètres souhaités et cliquez sur **[!UICONTROL Enregistrer]** une fois terminé.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[!UICONTROL Strict-Transport-Security]</strong></td>
  <td>Utilisez cette option pour garantir que les connexions aux landing pages seront toujours diffusées via HTTPS (ne doit être définie que pour les abonnements avec des landing pages sécurisées par SSL).</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL X-Frame-Options]</strong></td>
  <td>Permet de définir si des ressources hébergées par des Marketo Engage peuvent être incorporées ou non dans des pages web externes.</td>
 </tr>
</table>

>[!CAUTION]
>
>Il est important de passer en revue ces paramètres avec votre équipe informatique afin de déterminer la stratégie de votre entreprise. Des paramètres incorrects peuvent empêcher certains visiteurs d’accéder à vos pages d’entrée.
