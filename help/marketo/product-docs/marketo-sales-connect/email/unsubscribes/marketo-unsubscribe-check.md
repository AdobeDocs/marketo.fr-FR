---
unique-page-id: 18317340
description: Vérification du désabonnement Marketo - Documents Marketo - Documentation du produit
title: Vérification du désabonnement par Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---

# Vérification du désabonnement par Marketo {#marketo-unsubscribe-check}

La vérification de désabonnement de Marketo utilise la connexion de votre équipe à Marketo pour empêcher les courriers électroniques d’atteindre les personnes qui sont désabonnées dans le système de gestion des prospects Marketo. Lorsqu’un utilisateur commercial envoie un courrier électronique avec Sales Connect, un appel API est effectué à Marketo pour vérifier si l’ID de courrier électronique est désabonné. Si c&#39;est le cas, nous empêcherons l&#39;envoi de l&#39;email.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Activation {#turning-it-on}

1. Dans l’application web, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/one-2.png)

1. Sous Paramètres d’administration, cliquez sur **Se désabonner**.

   ![](assets/two-3.png)

1. Cliquez sur **Intégrations**.

   ![](assets/three-3.png)

1. Dans la section Vérifier le désabonnement de Marketo , cliquez sur le curseur pour activer la vérification.

   ![](assets/four-2.png)

## Informations à connaître {#things-to-know}

Le contrôle Désabonnement de Marketo...

* Ne tient pas compte des limites de votre API
* Nécessite une connexion Marketo
* est un paramètre global ;
* Blocage les emails envoyés depuis l’application web, les clients de messagerie et Salesforce
* Enregistre un message électronique en échec ou empêche un utilisateur d’envoyer un message lorsqu’il tente d’envoyer pour tous les workflows (envoi de module externe de messagerie, envoi individuel, envoi de campagne de vente, sélection et envoi multiples), à l’exception des [emails de groupe](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), dans lesquels nous empêcherons l’envoi silencieux des messages électroniques
