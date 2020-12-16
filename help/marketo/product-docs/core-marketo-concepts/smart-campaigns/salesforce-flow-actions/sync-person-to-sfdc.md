---
unique-page-id: 1147027
description: Synchroniser une personne avec SFDC - Documents marketing - Documentation du produit
title: Synchroniser la personne avec SFDC
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# Synchroniser la personne avec SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>Disponible uniquement lorsqu&#39;il est intégré à Salesforce.

## Présentation {#overview}

Cette étape de flux va insérer des personnes créées par Marketing comme pistes dans votre logiciel de gestion de la relation client Salesforce.

![](assets/sync-person-to-sfdc.png)

## Utilisation {#usage}

1. Par défaut, cette étape de flux est attribuée aux propriétaires de pistes en fonction des règles d&#39;affectation automatique Salesforce.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforce exige que les champs Société et Nom de la personne soient remplis. Sinon, il rejettera l&#39;enregistrement de piste.

1. Vous pouvez définir un utilisateur Salesforce ou une file d&#39;attente de pistes spécifique comme propriétaire de piste.

   ![](assets/sync-person-to-sfdc-2.png)

   Lors de l’utilisation de cette étape de flux, la personne est synchronisée immédiatement en tant que piste Salesforce et n’a pas besoin d’attendre la synchronisation régulière.

   >[!CAUTION]
   >
   >Salesforce n&#39;autorise pas l&#39;affectation de &quot;contacts&quot; aux files d&#39;attente de piste. Dans ce cas, Marketo créera un duplicata &quot;Lead&quot; dans Salesforce.

