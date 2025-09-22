---
description: Intégration de Dynamic Chat - Documents Marketo - Documentation du produit
title: Intégration de Dynamic Chat
exl-id: b2e3b4da-9ca7-4299-9c50-f52e0de91e36
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 7%

---

# Intégration de Dynamic Chat {#dynamic-chat-integration}

En savoir plus sur l’intégration de Dynamic Chat à Sales Insight.

>[!PREREQUISITES]
>
>* Le package SFDC de Sales Insight doit être de la version [2.4.0 ou ultérieure](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"}
>
>* L&#39;intégration [Dynamic Chat doit être configurée](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"}
>
>* Assurez-vous que le champ « Clé secrète API » est renseigné dans l’Insight commerciale [Paramètres opérationnels](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.md#operational-settings){target="_blank"}. Dans le cas contraire, apprenez à le récupérer [ici](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md#configure-sales-insight-in-marketo){target="_blank"}.

## Onglet Configuration [!DNL Marketo Sales Insight] {#marketo-sales-insight-configuration-tab}

Suivez les étapes ci-dessous pour activer l’intégration [!DNL Dynamic Chat].

1. Connectez-vous à votre compte [!DNL Salesforce], cliquez sur le signe + à la fin de la barre d’onglets, puis cliquez sur **[!DNL Marketo Sales Insight Config]**.

1. Cliquez pour déployer le « [!UICONTROL Panneau Visualforce] ».

   ![](assets/dynamic-chat-integration-1.png)

1. Cochez la case **[!UICONTROL Activer les données Dynamic Chat]**.

   ![](assets/dynamic-chat-integration-2.png)

## Vue d’ensemble des fonctionnalités {#feature-overview}

Les activités [!DNL Dynamic Chat] suivantes peuvent être exploitées par les utilisateurs [!DNL Sales Insight]...

Boîte de dialogue engagée : connectée à Marketo et renseignée dans [!DNL Sales Insight] lorsqu’un visiteur clique sur un chatbot et engage la boîte de dialogue.

* Nom du dialogue
* Page URL (URL de la page)
* Statut (Initié / Abandonné / Terminé)

Rendez-vous planifié : connecté à Marketo et renseigné dans [!DNL Sales Insight] lorsqu’un visiteur planifie un rendez-vous avec succès via le chatbot.

* Nom du dialogue
* Agent ou agente
* Page URL (URL de la page)
* Planifié le (insérer la date et l’heure)
* Statut (Planifié, Replanifié, Annulé)

Objectif atteint : connecté à Marketo et renseigné en [!DNL Sales Insight] lorsqu’un visiteur atteint un objectif dans un flux de boîte de dialogue.

* Nom du dialogue
* Nom de l&#39;objectif
* Page URL (URL de la page)

Interagi avec le document : connecté à Marketo et renseigné dans [!DNL Sales Insight] lorsqu’un visiteur interagit avec un document partagé via le chatbot.

* Nom du dialogue
* Document
* Statut

Les activités de conversation sont disponibles dans le tableau de bord des insights.

![](assets/dynamic-chat-integration-3.png)

Un onglet Conversation est disponible dans les panneaux Lead et Contact. Il comprend les colonnes [!UICONTROL Type d’activité], [!UICONTROL Nom de la boîte de dialogue] et [!UICONTROL Date].

![](assets/dynamic-chat-integration-4.png)

Pour en savoir plus sur un type d’activité, cliquez dessus.

![](assets/dynamic-chat-integration-5.png)

De même, les panneaux Compte et Opportunité comprennent les colonnes [!UICONTROL Nom], [!UICONTROL Type d’activité], [!UICONTROL Nom de la boîte de dialogue] et [!UICONTROL Date].

![](assets/dynamic-chat-integration-6.png)

L’onglet Conversation est également inclus dans votre onglet Marketo global . Il comprend trois types d’activités ([!UICONTROL Boîte de dialogue engagée], [!UICONTROL Rendez-vous prévu], [!UICONTROL Objectif atteint]), ainsi que les colonnes suivantes :

* [!UICONTROL &#x200B; Personne &#x200B;]
* [!UICONTROL Compte]
* [!UICONTROL &#x200B; Type d’activité &#x200B;] ([!UICONTROL Boîte de dialogue engagée], [!UICONTROL Rendez-vous prévu], [!UICONTROL Objectif atteint])
* [!UICONTROL Nom de la boîte de dialogue]
* [!UICONTROL Date]

Là encore, vous pouvez en savoir plus sur un type d’activité en cliquant dessus.

![](assets/dynamic-chat-integration-7.png)

>[!NOTE]
>
>Si la case à cocher « [!UICONTROL Activer les données Dynamic Chat] » est désactivée, les fonctionnalités suivantes seront désactivées :
>
>* Ligne avec les activités de conversation dans le tableau de bord des informations (grille intelligente et vue de liste hebdomadaire)
>* Onglet Conversation dans les panneaux Lead, Contact, Compte et Opportunité
>* Onglet Conversation dans l’onglet Marketo globale
>
>Il n’est pas possible de désactiver une seule de ces fonctionnalités.
