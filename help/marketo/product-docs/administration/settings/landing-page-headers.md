---
description: En-têtes de page de destination - Documents Marketo - Documentation du produit
title: En-têtes de page de destination
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '131'
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
  <td>Permet de définir si des ressources hébergées par Marketo Engage peuvent être incorporées dans des pages web externes</td>
 </tr>
</table>

>[!CAUTION]
>
>Il est important de passer en revue ces paramètres avec votre équipe informatique afin de déterminer la politique de votre entreprise à définir. Des paramètres incorrects peuvent empêcher certains visiteurs d’accéder à vos pages de destination.
