---
description: Erreurs de synchronisation Salesforce - Documents Marketo - Documentation du produit
title: Erreurs de synchronisation Salesforce
exl-id: 4819f423-30c6-48e3-8cec-5d298ceb7b56
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 4%

---

# Erreurs de synchronisation Salesforce {#salesforce-sync-errors}

Affichez un résumé des erreurs rencontrées lors du processus de synchronisation. Cela inclut les erreurs provoquées par l’échec de la synchronisation des données incompatibles.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Afficher les erreurs de synchronisation {#view-sync-errors}

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/salesforce-sync-errors-1.png)

1. Sous Intégration, cliquez sur **Salesforce**, puis sur l’onglet **[!UICONTROL Erreurs de synchronisation]** .

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Les erreurs répertoriées vont de l’heure actuelle à cinq jours avant la synchronisation actuelle.

| Champ | Description |
|---|---|
| Échec de | Niveau d’enregistrement _ou_ Niveau de tâche |
| Date/heure de l’échec | Détails de l’erreur |
| Type d&#39;erreur | Message de retour SFDC |

>[!TIP]
>
>Cliquez sur l’enregistrement de niveau enregistrement pour afficher les identifiants Marketo et Salesforce de l’objet associé. Dans certains cas, le message des erreurs au niveau de l’enregistrement et de la tâche provient directement de Salesforce. La recherche en ligne peut fournir des détails supplémentaires.

## Filtrer les erreurs de synchronisation {#filter-sync-errors}

1. Pour filtrer les données, cliquez sur l’icône de filtrage située à l’extrémité droite de la page.

   ![](assets/salesforce-sync-errors-3.png)

1. Sélectionnez la période et la période, puis filtrez par type d’erreur (niveau de tâche ou niveau d’enregistrement). Cliquez sur **[!UICONTROL Apply]** lorsque vous avez terminé.

   ![](assets/salesforce-sync-errors-4.png)

**ÉTAPE FACULTATIVE** : pour exporter des erreurs de synchronisation, cliquez sur **[!UICONTROL Exporter]**. Les données seront exportées au format CSV.

![](assets/salesforce-sync-errors-5.png)
