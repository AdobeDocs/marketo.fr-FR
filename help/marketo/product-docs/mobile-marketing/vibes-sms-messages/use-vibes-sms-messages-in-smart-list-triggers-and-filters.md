---
unique-page-id: 11378871
description: Utiliser des messages SMS de vidéos dans la liste dynamique Triggers et filtres - Documents Marketo - Documentation du produit
title: Utiliser des messages SMS de vidéos dans des déclencheurs et des filtres de liste dynamique
exl-id: 9a629a39-fddc-4ec5-b1c5-d5053d676594
feature: Mobile Marketing
source-git-commit: 444a184e48bf7034c6e0ef277c9a4dd1fb33bd86
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Utiliser des messages SMS de vidéos dans des déclencheurs et des filtres de liste dynamique {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Après vous [créer un SMS Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md), vous souhaitez utiliser des déclencheurs de liste dynamique et des filtres dans une campagne dynamique pour en tirer parti. Voici comment.

1. Dans Mon Marketo, cliquez sur **Activités marketing**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Sélectionnez une campagne dynamique dans laquelle vous souhaitez utiliser votre ressource SMS. Faites glisser le curseur sur un déclencheur, tel que le **Remplir le formulaire**.

   ![](assets/fills-out-form-pull-over.jpg)

## Triggers SMS {#sms-triggers}

D&#39;autres déclencheurs de SMS sont disponibles. Les déclencheurs SMS s’affichent uniquement si le service Vibes est activé.

![](assets/new-sms-search2.png)

Voici quelques exemples :

Le déclencheur Rebonds de message SMS lance un flux, tel que l’envoi d’un email, lorsqu’un message SMS rebondit.

![](assets/sms-message-bounces-real.jpg)

La variable **S’abonne à la liste des vidéos** déclenche un flux lorsqu’une personne s’abonne.

![](assets/subscribes-to-vibes-list-real.jpg)

La variable **Clics sur le lien dans un message SMS** déclenche un flux lorsqu’une personne clique sur un lien dans le SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtres SMS {#sms-filters}

Vous pouvez également utiliser des filtres Vibes dans les listes dynamiques. La variable **Abonné à la liste des vidéos** filtre recherche quiconque possède *ever* abonné à Vibes. Cela inclut les personnes désabonnées et supprimées, même si les personnes supprimées sont omises du flux. Ce filtre est mieux adapté à la création de rapports.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

En revanche, la variable **Membre de la liste des vidéos** filter find _any_ actuellement abonné à Vibes et convient le mieux à une utilisation dans des campagnes ou des listes dynamiques.

![](assets/image001.png)

>[!NOTE]
>
>Tous les filtres SMS incluent la variable **Date de l’activité** contrainte par défaut.

Après avoir configuré les déclencheurs et filtres Vibes dans votre liste dynamique, vous pouvez [définir le flux ;](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Définition d’une liste dynamique pour Smart Campaign | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Recherche et ajout de filtres à une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
