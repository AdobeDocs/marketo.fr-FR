---
description: En-têtes de page d’entrée - Documents Marketo - Documentation du produit
title: En-têtes de page d’entrée
hide: true
hidefromtoc: true
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
source-git-commit: 7950fb6ef4a0f653b3125ec381c652056bd47327
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 2%

---

# En-têtes de page d’entrée {#landing-page-headers}

Suivez les étapes ci-dessous pour personnaliser certains en-têtes HTTP de vos domaines de page d’entrée.

1. Dans Marketo, cliquez sur **Administration**.

   ![](assets/landing-page-headers-1.png)

1. Cliquez sur **Pages de destination**.

   ![](assets/landing-page-headers-2.png)

1. Cliquez sur **Modifier** en regard des en-têtes HTTP de page d’entrée.

   ![](assets/landing-page-headers-3.png)

1. Sélectionnez les paramètres de votre choix, puis cliquez sur **Enregistrer** une fois terminé.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>Strict Transport-Security</strong></td>
  <td>Utilisez cette option pour garantir que les connexions aux landing pages seront toujours diffusées via HTTPS (ne doit être définie que pour les abonnements avec des landing pages sécurisées par SSL).</td>
 </tr>
 <tr>
  <td><strong>X-Frame-Options</strong></td>
  <td>Permet de définir si des ressources hébergées par des Marketo Engage peuvent être incorporées ou non dans des pages web externes.</td>
 </tr>
</table>

>[!CAUTION]
>
>Il est important de passer en revue ces paramètres avec votre équipe informatique afin de déterminer la stratégie de votre entreprise. Des paramètres incorrects peuvent empêcher certains visiteurs d’accéder à vos pages d’entrée.
