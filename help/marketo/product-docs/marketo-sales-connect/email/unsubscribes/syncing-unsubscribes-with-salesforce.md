---
unique-page-id: 14746188
description: Synchronisation des désabonnements avec Salesforce - Marketo Docs - Documentation du produit
title: Synchronisation des désabonnements avec Salesforce
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Synchronisation des désabonnements avec Salesforce {#syncing-unsubscribes-with-salesforce}

## Conditions requises pour le désabonnement de la synchronisation avec Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Désabonner la synchronisation doit être activée (pour la synchronisation nocturne)
* opt-out champ doit être installé dans Salesforce
* Les enregistrements de personne dans Sales Connect doivent avoir un identifiant Salesforce.

**Désabonnements Push**

Lorsqu&#39;un désabonnement est collecté dans Sales Connect, nous l&#39;envoyons à Salesforce en temps réel et mettons à jour l&#39;un ou l&#39;autre des champs Opt-out que vous avez sélectionnés pour la synchronisation. Si vous avez désactivé la synchronisation Salesforce, nous pousserons toujours la désinscription à l&#39;opt-out de courriel.

**Désabonner la synchronisation**

Lorsque vous avez activé la synchronisation de désabonnement (étape 3 ci-dessous), vous activez la synchronisation de nuit. La synchronisation a lieu une fois par jour vers 20h00 PST. Il synchronise bidirectionnellement tous les désabonnements dans MSE/ToutApp avec le champ Opt-out de Salesforce.

## Configurer la synchronisation de désabonnement à Salesforce {#configure-unsubscribe-sync-to-salesforce}

Les utilisateurs peuvent décider s&#39;ils souhaitent synchroniser leurs désabonnements avec le champ de Opt-out de courriel standard avec lequel Marketo peut également synchroniser, ou s&#39;ils peuvent synchroniser avec le champ de Opt-out ventes de Marketo afin que les désabonnements des ventes et les désabonnements marketing puissent être différenciés.

1. Accédez à l&#39;[application Web](http://toutapp.com/login), cliquez sur l&#39;icône d&#39;engrenage et sélectionnez **Paramètres**.

   ![](assets/one-1.png)

1. Sous Paramètres d’administration, sélectionnez **Désabonnement**.

   ![](assets/two-2.png)

1. Cliquez sur **Synchronisation avec Salesforce**, puis activez la synchronisation de nuit.

   ![](assets/three-2.png)

1. Sélectionnez le champ à synchroniser.

   ![](assets/4.png)

   | **Champ Synchroniser avec Salesforce Opt-out** | Sélectionné par défaut, met uniquement à jour le champ Opt-out Salesforce. |
   |---|---|
   | **Champ Synchroniser avec le Opt-out des ventes du marketing** | Si vous souhaitez séparer les ventes et les désabonnements marketing, sélectionnez cette option pour mettre à jour le champ [Opt-out ventes marketing.](#msoo) |

## Installation du champ Opt-out dans la mise en page {#installing-the-opt-out-field-in-the-page-layout}

**Opt-out par courriel**

Le Opt-out de courriel est un champ standard de Salesforce qui peut être installé à partir de Salesforce. Vous devez être un administrateur Salesforce pour l’installer.

1. Accédez à [Salesforce.com](http://Salesforce.com) et connectez-vous.

   ![](assets/five-1.png)

1. Cliquez sur votre nom d’utilisateur et sélectionnez **Configuration**.

   ![](assets/six-1.png)

1. Dans la zone de recherche rapide, recherchez Contact ou Piste. Dans ce scénario, nous installons le champ dans la mise en page de la page Contact, mais vous voudrez installer pour les deux enregistrements de personne.

   ![](assets/seven-1.png)

1. Sélectionnez **Mise en page**.

   ![](assets/eight-1.png)

1. Sélectionnez **Modifier** en regard de la mise en page à laquelle vous souhaitez ajouter le champ.

   ![](assets/nine.png)

1. Sélectionnez **Champs**.

   ![](assets/ten.png)

1. Faites glisser et déposez Opt-out e-mail dans la mise en page.

   ![](assets/11.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/twelve.png)

## Opt-out des ventes du marketing {#marketo-sales-opt-out}

Le champ  Ventes du marketing est un champ personnalisé qui est disponible pour les utilisateurs qui ont installé les personnalisations de Marketing to Sales Connect.

Une fois que vous avez installé avec succès les Personnalisations de Marketing Connect Sales dans Salesforce, vous verrez le champ Marketo Sales Opt-out disponible.
