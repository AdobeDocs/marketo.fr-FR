---
unique-page-id: 14746188
description: Synchronisation des désabonnements avec Salesforce - Documents Marketo - Documentation du produit
title: Synchronisation des désabonnements avec Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 2%

---

# Synchronisation des désabonnements avec [!DNL Salesforce] {#syncing-unsubscribes-with-salesforce}

## Conditions requises pour les désabonnements à la synchronisation avec [!DNL Salesforce] {#requirements-for-unsubscribes-to-sync-to-salesforce}

* La synchronisation du désabonnement doit être activée (pour la synchronisation de nuit).
* Le champ Opt-out doit être installé dans [!DNL Salesforce]
* Les enregistrements de personne dans [!DNL Sales Connect] doivent avoir un ID [!DNL Salesforce]

**Désabonnements des notifications push**

Lorsqu’un désabonnement est collecté dans [!DNL Sales Connect], nous le poussons à [!DNL Salesforce] en temps réel et mettons à jour l’un des champs d’exclusion que vous avez sélectionnés pour la synchronisation. Si vous avez désactivé la synchronisation [!DNL Salesforce], nous transmettrons toujours le désabonnement à l’option de désinscription à l’e-mail.

**Synchronisation du désabonnement**

Lorsque vous avez activé la synchronisation de désabonnement (étape 3 ci-dessous), vous activez la synchronisation de nuit. La synchronisation a lieu une fois par jour vers 20 :00 PST. Elle synchronise de manière bidirectionnelle tous les désabonnements dans les ventes Marketo avec le champ Désinscription dans Salesforce.

## Configurer la synchronisation du désabonnement sur [!DNL Salesforce] {#configure-unsubscribe-sync-to-salesforce}

Les utilisateurs peuvent décider de synchroniser leurs désabonnements avec le champ d’opt-out d’e-mail standard que Marketo peut également synchroniser, ou avec le champ d’opt-out des ventes Marketo afin de différencier les désabonnements des ventes et les désabonnements marketing.

1. Accédez à l’[application web](https://toutapp.com/login), cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/one-1.png)

1. Sous [!UICONTROL Paramètres d’administration] sélectionnez **[!UICONTROL Désabonnements]**.

   ![](assets/two-2.png)

1. Cliquez sur **[!UICONTROL Synchronisation avec Salesforce]**, puis activez la synchronisation nocturne.

   ![](assets/three-2.png)

1. Sélectionnez le champ vers lequel vous souhaitez effectuer la synchronisation.

   ![](assets/4.png)

   | Champ | Description |
   |---|---|
   | **[!UICONTROL Champ Synchroniser avec le processus d’opt-out Salesforce]** | Sélectionné par défaut, ne met à jour que [!DNL Salesforce] champ Opt-out. |
   | **[!UICONTROL Champ d’exclusion de la synchronisation avec Marketo Sales]** | Si vous souhaitez séparer les désabonnements aux ventes et au marketing, choisissez cette option pour mettre à jour un champ d’[opt-out des ventes Marketo supplémentaire.](#msoo) |

## Installation du champ d’opt-out dans la mise en page {#installing-the-opt-out-field-in-the-page-layout}

**Désinscription Aux E-Mails**

L’Opt-out des e-mails est un champ standard dans [!DNL Salesforce] qui peut être installé à partir de [!DNL Salesforce]. Vous devez être un administrateur [!DNL Salesforce] pour l’installer.

1. Accédez à [Salesforce.com](https://salesforce.com) et connectez-vous.

   ![](assets/five-1.png)

1. Cliquez sur votre nom d’utilisateur et sélectionnez **[!UICONTROL Configuration]**.

   ![](assets/six-1.png)

1. Dans la zone de recherche rapide, recherchez le contact ou le prospect. Dans ce scénario, nous installons le champ sur la mise en page Page de contact, mais vous souhaiterez l’installer pour les deux enregistrements de personne.

   ![](assets/seven-1.png)

1. Sélectionnez **[!UICONTROL Mises En Page]**.

   ![](assets/eight-1.png)

1. Sélectionnez **[!UICONTROL Modifier]** en regard de la mise en page à laquelle vous souhaitez ajouter le champ.

   ![](assets/nine.png)

1. Sélectionnez **[!UICONTROL Champs]**.

   ![](assets/ten.png)

1. Effectuez un glisser-déposer [!UICONTROL Désinscription par e-mail] dans la disposition de la page.

   ![](assets/11.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**

   ![](assets/twelve.png)

## Désabonnement Marketo Sales {#marketo-sales-opt-out}

Le champ Désinscription (opt-out) des ventes Marketo est un champ personnalisé disponible pour les utilisateurs qui ont installé les personnalisations de [!DNL Sales Connect] Marketo.

Une fois que vous avez installé Marketo [!DNL Sales Connect] Customisations dans [!DNL Salesforce], le champ Désinscription (opt-out) aux ventes Marketo est disponible.
