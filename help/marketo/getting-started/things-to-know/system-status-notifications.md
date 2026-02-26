---
description: Abonnement aux notifications de statut du système - Documentation de Marketo Engage - Documentation du produit
title: Abonnement aux notifications d’état du système
feature: Getting Started
hide: true
hidefromtoc: true
source-git-commit: cf60167b9e9ee2ea2a2861a3cd3c661781dbf0b0
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Abonnement aux notifications d’état du système {#subscribe-to-system-status-notifications}

TEXTE D’INTRODUCTION

>[!PREREQUISITES]
>
>Avant de pouvoir créer un abonnement, vous devez d’abord identifier le centre de données et le pod/serveur dans lesquels se trouve votre abonnement.

## Identification de votre datacenter {#identify}

+++Identifier votre datacenter et votre pod/serveur

1. Dans la section **Admin** de Marketo Engage, cliquez sur **Mon compte**.

   ![](assets/subscribe-to-system-status-notifications-1.png)

1. Faites défiler jusqu’à _Informations d’assistance_.

   ![](assets/subscribe-to-system-status-notifications-2.png)

Dans le champ _Centre de données_, les lettres correspondent au centre de données et les chiffres au pod. Dans l’exemple ci-dessus, l’utilisateur se trouve dans notre centre de données Ashburn sur la capsule 49.

À l’étape 7 de la [création d’un abonnement](#create-a-subscription), cet utilisateur sélectionne l’emplacement régional **Marketo Ashburn** et le pod **ab49**.

<table style="width:225px;">
  <tr>
    <th colspan="2">Abréviations des centres de données</th>
  </tr>
  <tr>
    <td style="width:25%;">ab</td>
    <td>Ashburn</td>
  </tr>
  <tr>
    <td style="width:25%;">sj</td>
    <td>San José</td>
  </tr>
  <tr>
    <td style="width:25%;">sn</td>
    <td>Sydney</td>
  </tr>
  <tr>
    <td style="width:25%;">long</td>
    <td>Londres</td>
  </tr>
  <tr>
    <td style="width:25%;">nld</td>
    <td>Amsterdam</td>
  </tr>
</table>

>[!TIP]
>
>Cette méthode peut également être utilisée pour identifier le pod/serveur Real Time Personalization (RTP) dans lequel se trouve votre abonnement.

+++

## Créer un abonnement {#create-a-subscription}

Après [identification de votre centre de données et de votre pod/serveur](#identify), suivez les étapes ci-dessous pour créer un abonnement.

1. Sur [status.adobe.com](https://status.adobe.com/fr), cliquez sur **Gérer les abonnements**.

   ![](assets/subscribe-to-system-status-notifications-3.png)

1. Connectez-vous (si ce n’est pas déjà fait) à l’aide de vos identifiants Adobe ou cliquez sur **Créer un compte** si vous n’en avez pas.

   ![](assets/subscribe-to-system-status-notifications-4.png)

1. Restez dans l’onglet _Description des produits_ et cliquez sur **Créer des abonnements**.

   ![](assets/subscribe-to-system-status-notifications-5.png)

1. Cliquez sur l’icône ![icône représentant un signe plus](assets/icon-plus-sign.png) située en regard de _Experience Cloud_ pour développer le menu. Faites de même pour _Adobe Marketo Engage_.

   ![](assets/subscribe-to-system-status-notifications-6.png){width="800" zoomable="yes"}

1. Sélectionnez les offres/services de produit sur lesquels vous souhaitez recevoir des notifications et cliquez sur **Continuer**.

   >[!TIP]
   >
   >Cochez _Adobe Marketo Engage_ pour tout sélectionner.

   ![](assets/subscribe-to-system-status-notifications-7.png){width="800" zoomable="yes"}

1. Sélectionnez les types d’événements souhaités.

   ![](assets/subscribe-to-system-status-notifications-8.png)

   <table style="width:600px;">
   <tr>
   <td style="width:30%;"><b>Problème de service majeur</b></td>
   <td>Indisponibilité du service ou dégradation sévère des performances pour plusieurs utilisateurs sur les systèmes d’exploitation.</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Problème mineur de service</b></td>
   <td>Indisponibilité partielle du service ou dégradation modérée des performances pour plusieurs utilisateurs sur les systèmes d’exploitation.</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Maintenance des services</b></td>
   <td>Texte</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Annonces</b></td>
   <td>Annonces relatives à...</td>
   </tr>
   </table>

1. Sélectionnez l’emplacement régional et l’environnement souhaités. Cliquez sur **Continuer**.

   ![](assets/subscribe-to-system-status-notifications-9.png){width="800" zoomable="yes"}

1. Choisissez votre préférence d’abonnement, **E-mail** ou **Slack**, puis cliquez sur **Continuer**.

   ![](assets/subscribe-to-system-status-notifications-10.png)

1. Vérifiez vos sélections et cliquez sur **Confirmer les préférences**.

   ![](assets/subscribe-to-system-status-notifications-11.png)
