---
unique-page-id: 14746177
description: Réabonnement et désabonnement - Documents Marketo - Documentation du produit
title: Réabonnement après un désabonnement
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 1%

---

# Réabonnement à un [!UICONTROL Désabonnement] {#resubscribing-an-unsubscribe}

Parfois, les personnes souhaitent refuser de recevoir des e-mails. Voici comment rendre les désabonnements à nouveau envoyables par e-mail.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!CAUTION]
>
>Avant de réabonner quelqu’un, vous devez être en mesure de démontrer que l’autorisation de réabonner cette personne est documentée et conforme à toutes les lois applicables.

>[!NOTE]
>
>Si la synchronisation des désabonnements est activée, vous devez supprimer le désabonnement de ToutApp et décocher l’option d’opt-out dans [!DNL Salesforce] pour que l’enregistrement de la personne ne soit pas resynchronisé.

1. Accédez à l’[application web](https://toutapp.com/login) puis cliquez sur **[!UICONTROL Personnes]**.

1. Sélectionnez la personne pour ouvrir la vue des détails de la personne.

   ![](assets/two.png)

1. Cliquez sur les trois points de la vue Détails de la personne et sélectionnez **[!UICONTROL Supprimer le désabonnement]**.

   ![](assets/three.png)

1. Sélectionnez la raison pour laquelle la personne est de nouveau inscrite pour recevoir des e-mails, puis cliquez sur **[!UICONTROL Supprimer le désabonnement]**.

   ![](assets/four.png)

>[!NOTE]
>
>Si la synchronisation de désabonnement est activée, vous devez également décocher la case d’opt-out dans l’enregistrement dans Salesforce, sinon la synchronisation nocturne désabonnera à nouveau la personne dans [!DNL Sales Connect], car elle détectera que la personne a été désabonnée dans [!DNL Salesforce]. Si l’un des enregistrements fait l’objet d’une désinscription, la synchronisation marque l’enregistrement lié comme tel.
