---
description: Utiliser les options SMS dans la liste dynamique Triggers et filtres - Documents Marketo - Documentation du produit
title: Utilisation des options SMS dans les triggers et filtres de liste dynamique
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 8e56b571a34451d6b0436dc041efaf0fd575db36
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Utilisation des options SMS dans les triggers et filtres de liste dynamique {#use-sms-options-in-smart-list-triggers-and-filters}

NEW DOC

Après vous [créer un SMS ;](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, vous souhaitez utiliser des déclencheurs et des filtres de liste dynamique dans une campagne dynamique pour en tirer parti.

>[!PREREQUISITES]
>
>Les déclencheurs/filtres SMS n’apparaissent que si la variable [Le service Vibes a été activé](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md).

## Triggers SMS {#sms-triggers}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-1.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-2.png"></td>
  </tr>
</table>

Voici quelques exemples :

La variable **SMS Message Bounces** déclenche un flux, tel que l’envoi d’un email, lorsqu’un SMS rebondit.

La variable **S’abonne à la liste des vidéos** déclenche un flux lorsqu’une personne s’abonne.

La variable **Clics sur le lien dans un message SMS** déclenche un flux lorsqu’une personne clique sur un lien dans le SMS.

## Filtres SMS {#sms-filters}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-3.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-4.png"></td>
  </tr>
</table>

Vous pouvez également utiliser des filtres Vibes dans les listes dynamiques. La variable **Abonné à la liste des vidéos** filtre recherche quiconque possède *ever* abonné à Vibes. Cela inclut les personnes désabonnées et supprimées, même si les personnes supprimées sont omises du flux. Ce filtre est mieux adapté à la création de rapports.

En revanche, la variable **Membre de la liste des vidéos** filter find _any_ actuellement abonné à Vibes et convient le mieux aux campagnes ou listes dynamiques.

>[!NOTE]
>
>Tous les filtres SMS incluent la variable **Date de l’activité** contrainte par défaut.

Après avoir configuré les déclencheurs et filtres de vidéos dans votre liste dynamique, vous pouvez [définir le flux ;](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Envoyer un SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md)
>* [Définition d’une liste dynamique pour Smart Campaign | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Recherche et ajout de filtres à une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
