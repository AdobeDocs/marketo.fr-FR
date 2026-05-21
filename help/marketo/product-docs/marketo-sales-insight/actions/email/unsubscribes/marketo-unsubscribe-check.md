---
description: Découvrez la vérification du désabonnement de Marketo afin que les vendeurs ne puissent pas envoyer d’e-mail aux personnes désabonnées dans Marketo.
title: Vérification du désabonnement par Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
TQID: https://experienceleague.adobe.com/RaIYKEVyjdeUlOa4paltYIS8NPZHi1XWTmO4IeLBy-o
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 6%

---

# [!UICONTROL Vérification du désabonnement de &#x200B;] {#marketo-unsubscribe-check}

La vérification de désabonnement de  utilise la connexion de votre équipe à Marketo pour empêcher les e-mails d&#39;atteindre les personnes désabonnées dans le système de gestion des leads de Marketo. Lorsqu’un commercial envoie un e-mail avec [!DNL Marketo Sales], un appel API est effectué vers Marketo pour vérifier si l’ID d’e-mail est désabonné. Si c’est le cas, nous bloquerons l’envoi de l’e-mail.

>[!NOTE]
>
>**Autorisations d’administration requises**

## L&#39;activer {#turning-it-on}

1. Cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Sous [!UICONTROL Paramètres d’administration], cliquez sur **[!UICONTROL Désabonnements]**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Intégrations]**. Dans la section [!UICONTROL Vérification du désabonnement de &#x200B;], cliquez sur le curseur pour activer la vérification.

   ![](assets/marketo-unsubscribe-check-3.png)

## Choses à savoir {#things-to-know}

La vérification du désabonnement de Marketo...

* N’est pas comptabilisé par rapport à vos limites d’API
* Nécessite qu’une connexion Marketo soit établie
* Est un paramètre global
* Bloque les e-mails envoyés à partir de l’application web, des clients de messagerie et des [!DNL Salesforce]
