---
description: Vérification du désabonnement Marketo - Documents Marketo - Documentation du produit
title: Vérification du désabonnement par Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 4%

---

# Vérification du désabonnement par Marketo {#marketo-unsubscribe-check}

La vérification de désabonnement de Marketo utilise la connexion de votre équipe à Marketo pour empêcher les courriers électroniques d’atteindre les personnes qui sont désabonnées dans le système de gestion des prospects Marketo. Lorsqu’un utilisateur commercial envoie un courrier électronique avec les ventes Marketo, un appel API est effectué à Marketo pour vérifier si l’ID de courrier électronique est désabonné. Si c&#39;est le cas, nous empêcherons l&#39;envoi de l&#39;email.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Activation {#turning-it-on}

1. Cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Sous Paramètres d’administration, cliquez sur **Se désabonner**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Cliquez sur l’onglet **Intégrations** . Dans la section Vérifier le désabonnement de Marketo , cliquez sur le curseur pour activer la vérification.

   ![](assets/marketo-unsubscribe-check-3.png)

## Informations à connaître {#things-to-know}

Le contrôle Désabonnement de Marketo...

* Ne tient pas compte des limites de votre API
* Nécessite une connexion Marketo
* est un paramètre global ;
* Blocage les emails envoyés depuis l’application web, les clients de messagerie et Salesforce
