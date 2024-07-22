---
unique-page-id: 14746188
description: Synchronisation des désabonnements avec Salesforce - Documents Marketo - Documentation du produit
title: Synchronisation des désabonnements avec Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 1%

---

# Synchronisation des désabonnements avec Salesforce {#syncing-unsubscribes-with-salesforce}

## Conditions requises pour le désabonnement à la synchronisation avec Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* La synchronisation du désabonnement doit être activée (pour la synchronisation nocturne).
* Le champ Exclusion doit être installé dans Salesforce
* Les enregistrements de personne dans Sales Connect doivent avoir un identifiant Salesforce

**Désabonnements push**

Lorsqu’un désabonnement est collecté dans Sales Connect, nous l’envoyons à Salesforce en temps réel et mettons à jour l’un des champs d’exclusion que vous avez sélectionnés pour la synchronisation. Si vous avez désactivé la synchronisation Salesforce, nous continuerons à transmettre le désabonnement au désabonnement par courrier électronique.

**Désabonner la synchronisation**

Lorsque vous avez activé la synchronisation de désabonnement (Étape 3 ci-dessous), vous activez la synchronisation de nuit. La synchronisation a lieu une fois par jour vers 20 h (heure du Pacifique). Elle synchronise de manière bidirectionnelle tous les désabonnements dans les ventes Marketo avec le champ Exclusion de Salesforce.

## Configurer la synchronisation du désabonnement à Salesforce {#configure-unsubscribe-sync-to-salesforce}

Les utilisateurs peuvent décider s’ils souhaitent synchroniser leurs désabonnements avec le champ Email Opt Out standard avec lequel Marketo peut également se synchroniser, ou s’ils peuvent se synchroniser avec le champ Opposition de vente de Marketo afin que les désabonnements des ventes et les désabonnements marketing puissent être différenciés.

1. Accédez à l’ [application web](https://toutapp.com/login), cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/one-1.png)

1. Sous Paramètres d’administration, sélectionnez **Se désabonner**.

   ![](assets/two-2.png)

1. Cliquez sur **Synchronisation avec Salesforce**, puis activez la synchronisation nocturne.

   ![](assets/three-2.png)

1. Sélectionnez le champ auquel vous souhaitez effectuer la synchronisation.

   ![](assets/4.png)

   | Champ | Description |
   |---|---|
   | **Champ d’exclusion de la synchronisation avec Salesforce** | Sélectionné par défaut, met uniquement à jour le champ Option d’Opt-out Salesforce. |
   | **Champ d’exclusion de la synchronisation avec les ventes Marketo** | Si vous souhaitez séparer les ventes et les désabonnements marketing, sélectionnez cette option pour mettre à jour le [champ d&#39;exclusion des ventes Marketo.](#msoo) |

## Installation du champ Exclusion dans la mise en page {#installing-the-opt-out-field-in-the-page-layout}

**Email Opt Out**

Opt-out des emails est un champ standard de Salesforce qui peut être installé à partir de Salesforce. Vous devez être un administrateur Salesforce pour l’installer.

1. Accédez à [Salesforce.com](https://salesforce.com) et connectez-vous.

   ![](assets/five-1.png)

1. Cliquez sur votre nom d&#39;utilisateur et sélectionnez **Setup**.

   ![](assets/six-1.png)

1. Dans la zone de recherche rapide, recherchez Contact ou Lead. Dans ce scénario, nous installons le champ dans la mise en page de la page Contact, mais vous souhaiterez l’installer pour les deux enregistrements de personne.

   ![](assets/seven-1.png)

1. Sélectionnez **Mise en page**.

   ![](assets/eight-1.png)

1. Sélectionnez **Modifier** en regard de la mise en page à laquelle vous souhaitez ajouter le champ.

   ![](assets/nine.png)

1. Sélectionnez **Fields**.

   ![](assets/ten.png)

1. Faites glisser et déposez Opt-out Email dans la mise en page.

   ![](assets/11.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/twelve.png)

## Désabonnement Marketo Sales {#marketo-sales-opt-out}

Le champ Opposition de vente Marketo est un champ personnalisé qui est disponible pour les utilisateurs qui ont installé les personnalisations de Marketo Sales Connect.

Une fois que vous avez installé avec succès les personnalisations de Marketo Sales Connect dans Salesforce, le champ Marketo Sales Opt Out (Exclusion des ventes) s’affiche.
