---
description: Vérification du désabonnement de Marketo - Documents Marketo - Documentation du produit
title: Vérification du désabonnement par Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%

---

# [!UICONTROL Vérification du désabonnement de Marketo] {#marketo-unsubscribe-check}

La vérification de désabonnement de [!UICONTROL Marketo] utilise la connexion de votre équipe à Marketo pour empêcher les e-mails d&#39;atteindre les personnes désabonnées dans le système de gestion des leads de Marketo. Lorsqu’un commercial envoie un e-mail avec [!DNL Marketo Sales], un appel API est effectué vers Marketo pour vérifier si l’ID d’e-mail est désabonné. Si c’est le cas, nous bloquerons l’envoi de l’e-mail.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## L&#39;activer {#turning-it-on}

1. Cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Sous [!UICONTROL Paramètres d’administration], cliquez sur **[!UICONTROL Désabonnements]**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Intégrations]**. Dans la section [!UICONTROL Vérification du désabonnement de Marketo], cliquez sur le curseur pour activer la vérification.

   ![](assets/marketo-unsubscribe-check-3.png)

## Informations à connaître {#things-to-know}

La vérification du désabonnement de Marketo...

* N’est pas comptabilisé par rapport à vos limites d’API
* Nécessite qu’une connexion Marketo soit établie
* Est un paramètre global
* Bloque les e-mails envoyés à partir de l’application web, des clients de messagerie et des [!DNL Salesforce]
