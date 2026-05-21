---
unique-page-id: 1147027
description: Découvrez comment synchroniser une personne avec Salesforce à l’aide d’une étape de flux. Intégrer les données de lead ou de contact à SFDC lorsqu’elles entrent dans le flux.
title: Synchroniser une personne dans SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/jU7Hg1x8TUfxR4GnO1oxvJXh-8X3LVXll9z8k5Eck80
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 143
ht-degree: 5%

---

# Synchroniser une personne dans SFDC {#sync-person-to-sfdc}

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
