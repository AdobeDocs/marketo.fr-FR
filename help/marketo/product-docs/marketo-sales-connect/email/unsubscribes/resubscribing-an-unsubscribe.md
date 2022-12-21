---
unique-page-id: 14746177
description: Réabonnement à un désabonnement - Documents Marketo - Documentation du produit
title: Réabonnement à un désabonnement
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Réabonnement à un désabonnement {#resubscribing-an-unsubscribe}

Parfois, les gens veulent se reconnecter pour recevoir des emails. Voici comment rendre à nouveau les désabonnements publiables.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!CAUTION]
>
>Avant de vous réinscrire, vous devriez être en mesure de démontrer que l&#39;autorisation de vous réinscrire est documentée et conforme à toutes les lois applicables.

>[!NOTE]
>
>Si la synchronisation de désabonnement est activée, vous devez supprimer le désabonnement de ToutApp et décocher l’exclusion dans Salesforce pour que l’enregistrement de personne ne se synchronise plus.

1. Accédez au [application web](https://toutapp.com/login) et cliquez sur **Personnes**.

1. Sélectionnez la personne à ouvrir la vue Détails de la personne.

   ![](assets/two.png)

1. Cliquez sur les trois points dans la vue des détails de la personne et sélectionnez **Supprimer le désabonnement**.

   ![](assets/three.png)

1. Sélectionnez la raison pour laquelle la personne fait l’objet d’un abonnement pour recevoir des emails, puis cliquez sur **Supprimer le désabonnement**.

   ![](assets/four.png)

>[!NOTE]
>
>Si la synchronisation de désabonnement est activée, vous devez également décocher la case d’exclusion sur l’enregistrement dans Salesforce. Sinon, la synchronisation de nuit réabonnera la personne dans Sales Connect, car elle détectera que la personne est désabonnée dans Salesforce. Si l’un des enregistrements est désactivé/désabonné, la synchronisation marquera l’enregistrement lié comme tel.
