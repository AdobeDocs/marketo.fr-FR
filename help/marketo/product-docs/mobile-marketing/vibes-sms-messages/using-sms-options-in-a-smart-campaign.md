---
description: Utilisation des options SMS dans une campagne dynamique - Documents Marketo - Documentation du produit
title: Utilisation des options SMS dans une campagne dynamique
feature: Mobile Marketing
exl-id: 199b7cae-86d2-42fe-8934-10aa780f4454
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 2%

---

# Utilisation des options SMS dans une campagne dynamique {#using-sms-options-in-a-smart-campaign}

Après avoir [créé un SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, vous souhaiterez utiliser des triggers et filtres de liste dynamique dans une campagne dynamique pour en tirer les avantages.

>[!NOTE]
>
>Si vous souhaitez envoyer un SMS, nous avons un [article spécifique](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"} pour cela.

>[!PREREQUISITES]
>
>Les déclencheurs/filtres SMS n’apparaissent que si le service [Vibes a été activé](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}.

## Triggers SMS {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

Voici quelques exemples :

Le déclencheur **SMS Message Bounces** initie un flux, comme l&#39;envoi d&#39;un email, lorsqu&#39;un message SMS rebondit.

Le déclencheur **S’abonne à la liste des vidéos** lance un flux lorsqu’une personne s’abonne.

Le déclencheur **Clics sur le lien dans le message SMS** initie un flux lorsqu’une personne clique sur un lien dans le message SMS.

## Filtres SMS {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

Le filtre **Abonné à la liste des vidéos** trouve quiconque a *ever* abonné à Vibes. Cela inclut les personnes désabonnées et supprimées, même si les personnes supprimées sont omises du flux. Ce filtre est mieux adapté à la création de rapports.

En revanche, le filtre **Member of Vibes List** trouve _n’importe qui_ actuellement abonné à Vibes et est le mieux adapté aux campagnes ou listes dynamiques.

>[!NOTE]
>
>Tous les filtres SMS incluent par défaut la contrainte **Date of Activity** .

## Étapes de flux de SMS {#sms-flow-steps}

Il existe trois étapes de flux SMS parmi lesquelles choisir.

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>Envoyer un message SMS</b></td>
    <td>Cette action de flux envoie des messages aux personnes de la liste dynamique Marketo qui sont abonnées à une liste d’abonnements Vibes de souscription de l’utilisateur. Il ne lance pas le processus d’abonnement. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">En savoir plus</a>.</td>
  </tr>

<tr>
    <td style="width:20%"><b>S’abonner à la liste Vibes</b></td>
    <td>Cette action de flux lance le processus d'inscription SMS via une campagne d'acquisition Vibes sélectionnée par l'utilisateur. Vibes envoie alors un message de confirmation, auquel le destinataire doit répondre avec "Y" dans les 24 heures pour confirmer l'opt-in. Une fois que l’utilisateur s’est inscrit, il deviendra membre de la liste d’abonnements Vibes associée.</td>
  </tr>
  <tr>
    <td style="width:20%"><b>Se désabonner de la liste Vibes</b></td>
    <td>Cette action de flux désabonne chaque personne de la liste d’abonnement Vibes de l’utilisateur. Lorsqu’un utilisateur envoie un SMS "STOP" à votre code, son enregistrement de personne est mis à jour pour indiquer qu’il n’est plus membre de la liste d’abonnement Vibes.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>Les flux **S’abonner à la liste des vidéos** et **Se désabonner de la liste des vidéos** ont des exigences différentes. Pour **S’abonner**, vous devez sélectionner la liste Vibes et la campagne d’acquisition Vibes. Pour **Se désabonner**, seule la liste Vibes est requise.

>[!MORELIKETHIS]
>
>* [Envoyer un SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [ Définition d’une liste dynamique pour une campagne dynamique | Déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [ Définition d’une liste dynamique pour une campagne dynamique | Lot](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
