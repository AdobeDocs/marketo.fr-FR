---
unique-page-id: 18317340
description: Vérification du désabonnement Marketo - Documents Marketo - Documentation du produit
title: Vérification du désabonnement par Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
source-git-commit: 82c75d52caf3a0320cd3e8534b3b0870cf12d660
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

1. Dans l’application web, cliquez sur l’icône représentant un engrenage et sélectionnez **Paramètres**.

   ![](assets/one-2.png)

1. Sous Paramètres d’administration, cliquez sur **Désabonne**.

   ![](assets/two-3.png)

1. Cliquez sur **Intégrations**.

   ![](assets/three-3.png)

1. Dans la section Vérifier le désabonnement de Marketo , cliquez sur le curseur pour activer la vérification.

   ![](assets/four-2.png)

## Informations à connaître {#things-to-know}

Le contrôle Désabonnement de Marketo...

* Ne tient pas compte des limites de votre API
* Nécessite l’établissement d’une connexion Marketo
* est un paramètre global ;
* Blocage les emails envoyés à partir de l’application web, des clients de messagerie et de Salesforce.
* Consigner un message électronique en échec ou empêcher un utilisateur d’envoyer un message lorsqu’il tente d’envoyer pour tous les workflows (envoi de module externe de messagerie, envoi individuel, envoi de campagne de vente, sélection et envoi multiples), à l’exception de [emails de groupe](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), dans laquelle nous empêcherons l’envoi silencieux des emails
