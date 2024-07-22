---
description: Intégration de Dynamic Chat - Documents Marketo - Documentation du produit
title: Intégration du Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 6e81a8891f7d6e5916549d453a694b42e08cd496
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 6%

---

# Intégration du Dynamic Chat {#dynamic-chat-integration}

En savoir plus sur l’intégration du Dynamic Chat à Sales Insight.

>[!PREREQUISITES]
>
>* Votre package SFDC Sales Insight doit être la version [2.4.0 ou ultérieure ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* Vous devez configurer l’ [intégration de Dynamic Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}
>
>* Assurez-vous que le champ &quot;Clé secrète API&quot; est renseigné dans vos [Paramètres opérationnels](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"} de Sales Insight. Si ce n&#39;est pas le cas, découvrez comment le récupérer [ici](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}.

## Onglet Configuration des statistiques sur les ventes Marketo {#marketo-sales-insight-configuration-tab}

Suivez les étapes ci-dessous pour activer l’intégration du Dynamic Chat.

1. Connectez-vous à votre compte Salesforce, cliquez sur + à la fin de la barre d’onglets et cliquez sur **Marketo Sales Insight Config**.

1. Cliquez sur pour développer le &quot;panneau Visualforce&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Cochez la case **Activer les données de Dynamic Chat** .

   ![](assets/dynamic-chat-integration-2.png)

## Présentation des fonctionnalités {#feature-overview}

Les activités de Dynamic Chat suivantes peuvent être exploitées par les utilisateurs de Sales Insight..

Dialogue engagé : connecté à Marketo et renseigné dans Sales Insight lorsqu’un visiteur clique sur un chatterbot et engage le dialogue.

* Nom du dialogue
* URL de la page
* État (initié/abandonné/terminé)

Rendez-vous planifié : connecté à Marketo et renseigné dans Sales Insight lorsqu’un visiteur planifie un rendez-vous avec succès via le chatterbot.

* Nom du dialogue
* Agent
* URL de la page
* Planifié le (ajout d’un horodatage)
* État (planifié, replanifié, annulé)

Objectif atteint : Connecté à Marketo et renseigné dans Sales Insight lorsqu’un visiteur atteint un objectif dans n’importe quel flux de dialogue.

* Nom du dialogue
* Nom de l&#39;objectif
* URL de la page

Interaction avec le document : connecté à Marketo et renseigné dans Sales Insight lorsqu’un visiteur interagit avec un document partagé via le chatterbot.

* Nom du dialogue
* Document
* Statut

Les activités de conversation sont disponibles dans le tableau de bord des connaissances.

![](assets/dynamic-chat-integration-3.png)

Un onglet Conversation est disponible dans les panneaux Prospérité et Contact. Elle comprend les colonnes Type d’activité, Nom de la boîte de dialogue et Date.

![](assets/dynamic-chat-integration-4.png)

Pour en savoir plus sur un type d’activité, cliquez dessus.

![](assets/dynamic-chat-integration-5.png)

De même, les panneaux Compte et Opportunité incluent les colonnes Nom, Type d’activité, Nom de la boîte de dialogue et Date.

![](assets/dynamic-chat-integration-6.png)

L’onglet Conversation est également inclus dans votre onglet Marketo globale. Il comprend trois types d’activité (Dialogue engagé, Rendez-vous planifié, Objectif atteint), ainsi que les colonnes suivantes :

* Individu
* Compte
* Type d’activité (Dialogue engagé, Rendez-vous planifié, Objectif atteint)
* Nom du dialogue
* Date et heure (horodatage)

Encore une fois, vous pouvez en savoir plus sur un type d’activité en cliquant dessus.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Si la case &quot;Activer les données du Dynamic Chat&quot; est désactivée, les fonctionnalités suivantes sont désactivées :
>
>* Rangée avec les activités de conversation dans le tableau de bord des statistiques (grille dynamique et affichage de liste hebdomadaire)
>* Onglet Chat dans les panneaux &quot;Plomb, Contact, Compte et Opportunité&quot;
>* Onglet Conversation dans l’onglet Marketo globale
>
>Il n’est pas possible de désactiver une seule de ces fonctionnalités.

