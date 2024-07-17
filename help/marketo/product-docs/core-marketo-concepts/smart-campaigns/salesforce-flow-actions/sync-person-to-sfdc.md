---
unique-page-id: 1147027
description: Synchronisation de la personne avec SFDC - Documents Marketo - Documentation du produit
title: Synchroniser individu dans SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 6%

---

# Synchroniser individu dans SFDC {#sync-person-to-sfdc}

Cette étape de flux insère les personnes créées par Marketo comme prospects dans votre Salesforce CRM.

>[!NOTE]
>
>Disponible uniquement lorsqu’il est intégré à Salesforce.

1. Par défaut, cette étape de flux assignera les propriétaires de prospect en fonction des règles d’affectation automatique Salesforce.

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >Salesforce exige que les champs Société et Nom de la personne soient renseignés. Sinon, il rejettera l’enregistrement de piste.

1. Vous pouvez définir un utilisateur Salesforce ou une file d’attente de piste spécifique comme propriétaire de piste.

   ![](assets/sync-person-to-sfdc-2.png)

   Lors de l’utilisation de cette étape de flux, la personne est synchronisée en tant que prospect Salesforce immédiatement et n’a pas besoin d’attendre la synchronisation régulière.

   >[!CAUTION]
   >
   >Salesforce n’autorise pas l’affectation de &quot;contacts&quot; aux files d’attente de piste. Dans ce cas, Marketo crée un &quot;prospect&quot; en double dans Salesforce.
