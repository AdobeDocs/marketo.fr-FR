---
unique-page-id: 18317340
description: Vérification du désabonnement de Marketo - Documents Marketo - Documentation du produit
title: Vérification du désabonnement par Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 3%

---

# Vérification du désabonnement par Marketo {#marketo-unsubscribe-check}

La vérification de désabonnement de [!UICONTROL Marketo] utilise la connexion de votre équipe à Marketo pour empêcher les e-mails d&#39;atteindre les personnes désabonnées dans le système de gestion des leads de Marketo. Lorsqu’un commercial envoie un e-mail avec [!DNL Sales Connect], un appel API est effectué vers Marketo pour vérifier si l’ID d’e-mail est désabonné. Si c’est le cas, nous bloquerons l’envoi de l’e-mail.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## L&#39;activer {#turning-it-on}

1. Dans l’application web, cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/one-2.png)

1. Sous [!UICONTROL Paramètres d’administration], cliquez sur **[!UICONTROL Désabonnements]**.

   ![](assets/two-3.png)

1. Cliquez sur **[!UICONTROL Intégrations]**.

   ![](assets/three-3.png)

1. Dans la section [!UICONTROL Vérification du désabonnement de Marketo], cliquez sur le curseur pour activer la vérification.

   ![](assets/four-2.png)

## Informations à connaître {#things-to-know}

La vérification du désabonnement de Marketo...

* N’est pas comptabilisé par rapport à vos limites d’API
* Nécessite qu’une connexion Marketo soit établie
* Est un paramètre global
* Bloque les e-mails envoyés à partir de l’application web, des clients de messagerie et de Salesforce
* consigne un e-mail en échec ou empêche l’envoi d’un e-mail à un utilisateur ou une utilisatrice lorsqu’il ou elle tente d’envoyer pour tous les workflows (envoi de plug-in d’e-mail, envoi individuel, envoi de campagne commerciale, sélection multiple et envoi) à l’exception des e-mails de [groupe](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), dans lesquels nous empêchons l’envoi silencieux des e-mails.
