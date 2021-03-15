---
description: Erreurs de synchronisation de Salesforce - Docs marketing - Documentation du produit
title: Erreurs de synchronisation Salesforce
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# Erreurs de synchronisation Salesforce {#salesforce-sync-errors}

Vue d’un résumé des erreurs survenues pendant le processus de synchronisation. Ceci inclut les erreurs provoquées par les échecs de synchronisation de données incompatibles.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

## Erreurs de synchronisation des vues {#view-sync-errors}

1. Cliquez sur **Admin**.

   ![](assets/salesforce-sync-errors-1.png)

1. Sous Intégration, cliquez sur **Salesforce**, puis sur l&#39;onglet **Erreurs de synchronisation**.

   ![](assets/salesforce-sync-errors-2.png)

>[!NOTE]
>
>Les erreurs répertoriées vont de l’heure actuelle à cinq jours avant la synchronisation actuelle.

| Champ | Description |
|---|---|
| Échec le | Niveau d&#39;enregistrement _ou_ Niveau de travail |
| Date/heure de l&#39;échec | Détails de l’erreur |
| Type d’erreur | Message de retour SFDC |

>[!TIP]
>
>Un clic sur l’enregistrement de niveau enregistrement affiche les identifiants Marketo et Salesforce de l’objet associé. Dans certains cas, le message figurant au dossier et les erreurs au niveau de la tâche proviennent directement de Salesforce. Leur recherche en ligne peut fournir des détails supplémentaires.

## Erreurs de synchronisation des filtres {#filter-sync-errors}

1. Pour filtrer les données, cliquez sur l’icône de filtre située à l’extrémité droite de la page.

   ![](assets/salesforce-sync-errors-3.png)

1. Sélectionnez la date et l’heure, puis filtrez par type d’erreur (niveau tâche ou niveau enregistrement). Cliquez sur **Appliquer** lorsque vous avez terminé.

   ![](assets/salesforce-sync-errors-4.png)

**Étape** facultative : Pour exporter les erreurs de synchronisation, cliquez sur  **Exporter**. Les données seront exportées au format CSV.

![](assets/salesforce-sync-errors-5.png)
