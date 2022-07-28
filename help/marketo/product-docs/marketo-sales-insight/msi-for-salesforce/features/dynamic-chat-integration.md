---
description: Intégration Dynamic Chat - Documents Marketo - Documentation du produit
title: Intégration de tchat dynamique
hide: true
hidefromtoc: true
source-git-commit: ea2ee32a4c8805154f17717d515bb994dbfbe982
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 5%

---

# Intégration de tchat dynamique {#dynamic-chat-integration}

En savoir plus sur l’intégration de Dynamic Chat à Sales Insight.

>[!PREREQUISITES]
>
>* Votre package SFDC Sales Insight doit être une version [1.9 ou version ultérieure](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;}
>
>* Vous devez avoir la variable [Intégration de la messagerie dynamique](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md)Configuration de {target=&quot;_blank&quot;}


## Onglet Configuration des statistiques sur les ventes Marketo {#marketo-sales-insight-configuration-tab}

1. Connectez-vous à votre compte Salesforce, cliquez sur le signe + à la fin de la barre d’onglets, puis cliquez sur **Configuration de Marketo Sales Insight**.

1. Cliquez sur pour développer le &quot;panneau Visualforce&quot;.

   ![](assets/dynamic-chat-integration-1.png)

1. Sélectionnez la **Activation des données de conversation dynamique** .

   ![](assets/dynamic-chat-integration-2.png)

## Présentation des fonctionnalités {#feature-overview}

Les activités de conversation dynamique ci-dessous peuvent être exploitées par les utilisateurs de Sales Insight.

Dialogue engagé : Connecté à Marketo et renseigné dans Sales Insight lorsqu’un visiteur clique sur un chatterbot et engage le dialogue.

* Nom de la conversation
* URL de la page
* État (initié/abandonné/terminé)

Rendez-vous planifié : Connecté à Marketo et renseigné dans Sales Insight lorsqu’un visiteur parvient à planifier un rendez-vous via le chatbot.

* Nom de la conversation
* Agent
* URL de la page
* Planifié le (ajout d’un horodatage et d’une date)
* État (planifié, replanifié, annulé)

Objectif atteint : Connecté à Marketo et renseigné dans Sales Insight lorsqu’un visiteur atteint un objectif dans un flux de dialogue.

* Nom de la conversation
* Nom de l’objectif
* URL de la page

Un onglet Conversation est disponible dans les panneaux Prospérité et Contact. Elle comprend les colonnes Type d’activité, Nom de la boîte de dialogue et Date.

![](assets/dynamic-chat-integration-3.png)

Pour en savoir plus sur un type d’activité, cliquez dessus.

![](assets/dynamic-chat-integration-4.png)

De même, les panneaux Compte et Opportunité incluent les colonnes Nom, Type d’activité, Nom de la boîte de dialogue et Date.

![](assets/dynamic-chat-integration-5.png)

L’onglet Conversation est également inclus dans votre onglet Marketo globale. Il comprend trois types d’activité (Dialogue engagé, Rendez-vous planifié, Objectif atteint), ainsi que les colonnes suivantes :

* Individu
* Compte
* Type d’activité (Dialogue engagé, Rendez-vous planifié, Objectif atteint)
* Nom de la conversation
* Date et heure (horodatage)

Encore une fois, vous pouvez en savoir plus sur un type d’activité en cliquant dessus.

![](assets/dynamic-chat-integration-6.png)

>[!NOTE]
>
>L’activité &quot;Interagi avec le document&quot; sera disponible dans MSI dans une prochaine version.
