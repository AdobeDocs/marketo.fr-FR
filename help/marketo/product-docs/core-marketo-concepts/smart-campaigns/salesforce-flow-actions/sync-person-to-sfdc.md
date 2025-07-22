---
unique-page-id: 1147027
description: Synchroniser la personne avec SFDC - Documents Marketo - Documentation du produit
title: Synchroniser individu dans SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 6%

---

# Synchroniser individu dans SFDC {#sync-person-to-sfdc}

Cette étape de flux insérera des personnes créées par Marketo en tant que prospects dans votre CRM Salesforce.

>[!NOTE]
>
>Disponible uniquement lorsqu’il est intégré à [!DNL Salesforce].

1. Par défaut, cette étape de flux est affectée aux propriétaires de prospect en fonction des règles d’affectation automatique de Salesforce.

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >[!DNL Salesforce] nécessite que la personne ait renseigné les champs Société et Nom . Dans le cas contraire, l’enregistrement du prospect sera rejeté.

1. Vous pouvez définir un utilisateur [!DNL Salesforce] ou une file d’attente de prospects spécifique en tant que propriétaire de prospects.

   ![](assets/sync-person-to-sfdc-2.png)

   Lors de l’utilisation de cette étape de flux, la personne est synchronisée immédiatement en tant que prospect [!DNL Salesforce] et n’a pas besoin d’attendre la synchronisation normale.

   >[!CAUTION]
   >
   >[!DNL Salesforce] n’autorise pas l’affectation de « contacts » aux files d’attente de prospects. Dans ce cas, Marketo crée un « Lead » en double dans [!DNL Salesforce].
