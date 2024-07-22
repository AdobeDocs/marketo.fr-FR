---
description: Utiliser des messages SMS de vidéos dans la liste dynamique Triggers et filtres - Documents Marketo - Documentation du produit
title: Utiliser des messages SMS de vidéos dans des déclencheurs et des filtres de liste dynamique
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: fee2d692acd8d54f2e308e2d5edc9876d13d5a4d
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Utiliser des messages SMS de vidéos dans des déclencheurs et des filtres de liste dynamique {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Après avoir [ créé un SMS Vibes ](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"}, vous souhaiterez utiliser des triggers et filtres de liste dynamique dans une campagne dynamique pour en tirer les avantages. Voici comment.

1. Dans Mon Marketo, cliquez sur **Activités marketing**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Sélectionnez une campagne dynamique dans laquelle vous souhaitez utiliser vos ressources SMS. Faites glisser le curseur sur un déclencheur. Dans cet exemple, nous utilisons **Remplit le formulaire**.

   ![](assets/fills-out-form-pull-over.jpg)

## Triggers SMS {#sms-triggers}

D&#39;autres déclencheurs de SMS sont disponibles. Les déclencheurs SMS s’affichent uniquement si le service Vibes est activé.

ENVOYER UN SMS :

* Activités marketing > choisissez Nouvelle campagne dynamique
   * Liste dynamique > Choisir la liste des vidéos : filtrer et corriger la logique > Liste des vidéos : choisissez la liste dans la liste déroulante (liste des bases de données mobiles qui se synchronise à partir de la plateforme Vibes)
      * Peuvent affiner la segmentation et utiliser les filtres et déclencheurs de SMS et d&#39;email dans une seule campagne
      * Filtres de vidéos : Abonné à la liste des vidéos par rapport à Membre de la liste des vidéos - la logique est cohérente avec les emails.
         * S’abonner à la liste des vidéos : les participants qui se sont jamais inscrits à cette liste même s’ils se sont désabonnés.  - principalement utilisés pour les efforts marketing cross-canal
            * Remarque : Un SMS ne sera envoyé à personne désabonné s’il ne figure pas dans la liste de la base de données mobile Vibes.
         * Membre de la liste des vidéos : abonné actif et confirmé
         * Ajouté à la liste - Les listes Vibes ne seront pas renseignées avec ce filtre ; il s’agit des listes Marketo

![](assets/new-sms-search2.png)

Voici quelques exemples :

Le déclencheur **SMS Message Bounces** initie un flux, comme l&#39;envoi d&#39;un email, lorsqu&#39;un message SMS rebondit.

![](assets/sms-message-bounces-real.jpg)

Le déclencheur **S’abonne à la liste des vidéos** lance un flux lorsqu’une personne s’abonne.

![](assets/subscribes-to-vibes-list-real.jpg)

Le déclencheur **Clics sur le lien dans le message SMS** initie un flux lorsqu’une personne clique sur un lien dans le message SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtres SMS {#sms-filters}

Vous pouvez également utiliser des filtres Vibes dans les listes dynamiques. Le filtre **Abonné à la liste des vidéos** trouve quiconque a *ever* abonné à Vibes. Cela inclut les personnes désabonnées et supprimées, même si les personnes supprimées sont omises du flux. Ce filtre est mieux adapté à la création de rapports.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

En revanche, le filtre **Member of Vibes List** trouve _n’importe qui_ actuellement abonné à Vibes et est le mieux adapté aux campagnes ou listes dynamiques.

![](assets/image001.png)

>[!NOTE]
>
>Tous les filtres SMS incluent par défaut la contrainte **Date of Activity** .

Après avoir configuré les déclencheurs et filtres Vibes dans votre liste dynamique, vous pouvez [définir le flux](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [ Définition d’une liste dynamique pour une campagne dynamique | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Rechercher et ajouter des filtres à une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
