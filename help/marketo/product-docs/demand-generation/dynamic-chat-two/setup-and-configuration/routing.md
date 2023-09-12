---
description: Routage - Documents Marketo - Documentation du produit
title: Routage
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: df719d0db50009180e707b88b53115d4a62f35bf
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Routage {#routing}

Les réunions réservées en Dynamic Chat peuvent être routées de deux façons. Arrondir le robin ou utiliser une règle personnalisée.

Tour à tour : les réunions sont assignées aux agents de manière séquentielle. Donc si vous avez cinq agents et l&#39;agent trois qui ont pris la dernière réunion, l&#39;agent quatre aura le suivant, suivi de l&#39;agent cinq, puis revenir à l&#39;agent un.

Règle personnalisée : vous pouvez choisir des agents spécifiques pour recevoir des réunions en fonction des attributs que vous sélectionnez.

>[!NOTE]
>
>Routage de compte a la priorité la plus élevée. Lorsqu’un visiteur atteint le point de la conversation pour réserver une réunion ou lancer une conversation en direct, [Routage de compte](#account-routing) est vérifié avant que d’autres options de routage ne soient prises en compte.

## Création d’une règle personnalisée {#create-a-custom-rule}

Dans cet exemple, nous envoyons toutes les réunions des états déduits de CA, OU et WA à l’agent John.

1. Sous Configuration, cliquez sur **Règles de routage**.

   ![](assets/routing-1.png)

1. Cliquez sur le bouton **Règles personnalisées** .

   ![](assets/routing-2.png)

1. Cliquez sur **Créer une règle**.

   ![](assets/routing-3.png)

1. Nommez votre règle. Vous pouvez éventuellement ajouter une description et définir son niveau de priorité. Cliquez sur **Suivant**.

   ![](assets/routing-4.png)

1. Sélectionnez le ou les agents souhaités.

   ![](assets/routing-5.png)

1. Faites glisser le pointeur de la souris sur le ou les attributs souhaités.

   ![](assets/routing-6.png)

1. Recherchez et sélectionnez la ou les valeurs souhaitées.

   ![](assets/routing-7.png)

1. Lorsque toutes les valeurs souhaitées sont sélectionnées, cliquez sur **Enregistrer**.

   ![](assets/routing-8.png)

## Routage de compte {#account-routing}

Identifiez et chargez votre compte cible et les propriétaires de ventes respectifs et acheminez les visiteurs provenant de ces comptes directement vers le propriétaire du compte correspondant.

![](assets/routing-9.png)

### Ajout d’un compte {#add-an-account}

Dans cet exemple, nous acheminerons tous les employés de Lego directement vers l’agent Steven.

1. Dans l’onglet Routage de compte , cliquez sur **+ Ajouter un compte**.

   ![](assets/routing-10.png)

   >[!TIP]
   >
   >Vous pouvez créer plusieurs comptes en même temps en cliquant sur **Télécharger la liste des comptes** et télécharger un fichier CSV.

1. Saisissez le nom, le domaine et l’agent de votre choix.

   ![](assets/routing-11.png)
