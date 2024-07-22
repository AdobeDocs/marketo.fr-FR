---
description: Synchronisation des désabonnements avec Salesforce - Documents Marketo - Documentation du produit
title: Synchronisation des désabonnements avec Salesforce
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Synchronisation des désabonnements avec Salesforce {#syncing-unsubscribes-with-salesforce}

Si vous souhaitez synchroniser les désabonnements avec un champ d’exclusion dans Salesforce, vous pouvez utiliser la synchronisation de désabonnement Salesforce.

## Conditions requises pour le désabonnement à la synchronisation avec Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* La synchronisation du désabonnement doit être activée (pour la synchronisation nocturne).
* Le champ Exclusion doit être installé dans Salesforce
* Les enregistrements de personne dans les ventes Marketo doivent avoir un identifiant Salesforce

**Désabonnements push**

Lorsqu’un désabonnement est collecté dans les ventes Marketo, nous le poussons vers Salesforce en temps réel et mettons à jour l’un des champs d’exclusion que vous avez sélectionnés pour la synchronisation. Si vous avez désactivé la synchronisation Salesforce, nous continuerons à transmettre le désabonnement au désabonnement par courrier électronique.

**Désabonner la synchronisation**

Lorsque vous avez activé la synchronisation de désabonnement (Étape 3 ci-dessous), vous activez la synchronisation nocturne. La synchronisation a lieu une fois par jour vers 20 h (heure du Pacifique). Elle synchronise de manière bidirectionnelle tous les désabonnements dans les ventes Marketo avec le champ Exclusion de Salesforce.

>[!NOTE]
>
>La synchronisation du désabonnement avec Salesforce synchronise les désabonnements, mais ne synchronise pas les réabonnements. Si vous souhaitez supprimer un désabonnement de Marketo Sales et Salesforce, désélectionnez le désabonnement dans Salesforce et supprimez le désabonnement dans Marketo Sales.

## Configurer la synchronisation du désabonnement à Salesforce {#configure-unsubscribe-sync-to-salesforce}

Les utilisateurs peuvent décider s’ils souhaitent synchroniser leurs désabonnements avec le champ Email Opt Out standard avec lequel Marketo peut également se synchroniser, ou s’ils peuvent se synchroniser avec le champ Opposition de vente de Marketo afin que les désabonnements des ventes et les désabonnements marketing puissent être différenciés.

1. Cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. Sous Paramètres d’administration, sélectionnez **Se désabonner**.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. Cliquez sur l’onglet **Intégrations** . Sous Synchroniser avec Salesforce, activez la synchronisation nocturne.

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. Sélectionnez le champ auquel vous souhaitez effectuer la synchronisation.

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | Champ | Description |
   |---|---|
   | **Champ d’exclusion de la synchronisation avec Salesforce** | Sélectionné par défaut, met uniquement à jour le champ Option d’Opt-out Salesforce. |
   | **Champ d’exclusion de la synchronisation avec les ventes Marketo** | Si vous souhaitez séparer les ventes et les désabonnements marketing, sélectionnez cette option pour mettre à jour le [champ d&#39;exclusion des ventes Marketo.](#msoo) |

## Installation du champ Exclusion dans la mise en page {#installing-the-opt-out-field-in-the-page-layout}

**Email Opt Out**

Opt-out des emails est un champ standard de Salesforce qui peut être installé à partir de Salesforce. Vous devez être un administrateur Salesforce pour l’installer.

1. Accédez à [Salesforce.com](https://salesforce.com) et connectez-vous.

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. Cliquez sur votre nom d&#39;utilisateur et sélectionnez **Setup**.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. Dans la zone de recherche rapide, recherchez Contact ou Lead. Dans ce scénario, nous installons le champ dans la mise en page de la page Contact, mais vous souhaiterez l’installer pour les deux enregistrements de personne.

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. Sélectionnez **Mise en page**.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. Sélectionnez **Modifier** en regard de la mise en page à laquelle vous souhaitez ajouter le champ.

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. Sélectionnez **Fields**.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. Faites glisser et déposez Opt-out Email dans la mise en page.

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Désabonnement Marketo Sales {#marketo-sales-opt-out}

Le champ Opposition de vente Marketo est un champ personnalisé qui est disponible pour les utilisateurs qui ont installé le package Marketo Sales Insight [ à partir de l’AppExchange ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

Une fois que vous avez installé le package Marketo Sales Insight de l’AppExchange vers Salesforce, vous pouvez voir le champ Marketo Sales Opt Out (Exclusion des ventes de) disponible.
