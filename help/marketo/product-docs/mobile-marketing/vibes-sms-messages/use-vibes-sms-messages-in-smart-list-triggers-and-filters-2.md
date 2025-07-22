---
description: Utiliser des messages SMS Vibes dans les déclencheurs et filtres de liste dynamique - Documents Marketo - Documentation du produit
title: Utiliser les messages SMS Vibes dans les déclencheurs et filtres de liste dynamique
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 1%

---

# Utiliser les messages SMS Vibes dans les déclencheurs et filtres de liste dynamique {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Après avoir [créé un SMS Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"}, vous souhaiterez utiliser les déclencheurs et filtres de liste dynamique dans une campagne dynamique pour en tirer les avantages. Voici comment procéder.

1. Dans Mon Marketo, cliquez sur **[!UICONTROL Activités marketing]**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Choisissez une campagne intelligente dans laquelle vous souhaitez utiliser vos ressources SMS. Faites glisser sur un déclencheur. Dans cet exemple, nous utilisons **remplit le formulaire**.

   ![](assets/fills-out-form-pull-over.jpg)

## Déclencheurs SMS {#sms-triggers}

D’autres déclencheurs SMS sont disponibles. Les déclencheurs SMS s’affichent uniquement si le service Vibes est activé.

ENVOYER UN SMS :

* Activités marketing > choisir une nouvelle campagne intelligente
   * Liste dynamique > Choisir la liste Vibes Filtrer et logique correcte > Liste Vibes : liste déroulante Choisir la liste (liste de base de données mobile qui se synchronise à partir de la plateforme Vibes)
      * Peut affiner la segmentation et utiliser des filtres et triggers SMS et e-mail dans une campagne
      * Filtres Vibes : Abonné à la liste Vibes par rapport au membre de la liste Vibes - la logique est cohérente avec l’e-mail
         * Abonnés à la liste Vibes : participants qui ne se sont jamais abonnés à cette liste Vibes, même s’ils sont maintenant désabonnés.  : principalement utilisé pour les efforts marketing cross-canal
            * Remarque : aucun SMS ne sera envoyé à une personne désabonnée si elle ne figure pas dans la liste Base de données mobile Vibes
         * Membre de la liste Vibes - abonné actif et confirmé
         * Ajouté à la liste : les listes Vibes ne seront pas renseignées avec ce filtre, il s’agit des listes Marketo

![](assets/new-sms-search2.png)

Voici quelques exemples :

Le déclencheur **Bounces de messages SMS** lance un flux, tel que l’envoi d’un e-mail, lorsqu’un message SMS fait l’objet de bounces.

![](assets/sms-message-bounces-real.jpg)

Le déclencheur **[!UICONTROL S’abonne à la liste Vibes]** lance un flux lorsqu’une personne s’abonne.

![](assets/subscribes-to-vibes-list-real.jpg)

Le déclencheur **[!UICONTROL Clics sur le lien dans un SMS]** lance un flux lorsqu’une personne clique sur un lien dans le SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtres SMS {#sms-filters}

Vous pouvez également utiliser les filtres Vibes dans les listes dynamiques. Le filtre **[!UICONTROL Liste des abonnés à Vibes]** recherche toute personne qui s’est *jamais* abonnée à Vibes. Cela inclut les personnes désabonnées et supprimées, même si les personnes supprimées sont omises du flux. Ce filtre est le mieux adapté aux rapports.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

En revanche, le filtre **Membre de la liste Vibes** trouve _toute personne_ actuellement abonnée à Vibes et est plus adapté à une utilisation dans des campagnes ou des listes intelligentes.

![](assets/image001.png)

>[!NOTE]
>
>Tous les filtres SMS incluent par défaut la contrainte **[!UICONTROL Date de l’activité]**.

Après avoir configuré les déclencheurs et filtres Vibes dans votre liste dynamique, vous pouvez [définir le flux](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Définir une liste dynamique pour une campagne dynamique | Déclencheur ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Rechercher et ajouter des filtres à une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
