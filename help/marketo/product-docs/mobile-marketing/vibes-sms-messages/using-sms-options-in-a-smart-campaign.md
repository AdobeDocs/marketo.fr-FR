---
description: Utilisation des options SMS dans une campagne intelligente - Documents Marketo - Documentation du produit
title: Utilisation des options SMS dans une campagne intelligente
feature: Mobile Marketing
exl-id: 199b7cae-86d2-42fe-8934-10aa780f4454
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 7%

---

# Utilisation des options SMS dans une campagne intelligente {#using-sms-options-in-a-smart-campaign}

Après avoir [créé un SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, vous souhaiterez utiliser les déclencheurs et filtres de liste dynamique dans une campagne dynamique pour en tirer les avantages.

>[!NOTE]
>
>Si vous souhaitez envoyer un SMS, nous disposons d’un [article spécifique](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"} à cet effet.

>[!PREREQUISITES]
>
>Les déclencheurs/filtres SMS ne s’affichent que si le service [Vibes a été activé](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}.

## Déclencheurs SMS {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

Voici quelques exemples :

Le déclencheur **Bounces de messages SMS** lance un flux, tel que l’envoi d’un e-mail, lorsqu’un message SMS fait l’objet de bounces.

Le déclencheur **S’abonne à la liste Vibes** lance un flux lorsqu’une personne s’abonne.

Le déclencheur **Clics sur le lien dans un SMS** lance un flux lorsqu’une personne clique sur un lien dans le SMS.

## Filtres SMS {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

Le filtre **Liste des abonnés à Vibes** recherche toute personne qui s’est *jamais* abonnée à Vibes. Cela inclut les personnes désabonnées et supprimées, même si les personnes supprimées sont omises du flux. Ce filtre est le mieux adapté aux rapports.

En revanche, le filtre **Membre de la liste Vibes** trouve *toute personne* actuellement abonnée à Vibes et est plus adapté à une utilisation dans des campagnes ou des listes intelligentes.

>[!NOTE]
>
>Tous les filtres SMS incluent par défaut la contrainte **Date de l’activité**.

## Étapes du flux SMS {#sms-flow-steps}

Vous avez le choix entre trois étapes de flux de SMS.

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>Envoyer un message SMS</b></td>
    <td>Cette action de flux envoie des messages aux personnes de la liste dynamique Marketo qui sont abonnées à une liste d’abonnements Vibes activée par l’utilisateur. Il ne lance pas le processus d’abonnement. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">En savoir plus</a>.</td>
  </tr>

<tr>
    <td style="width:20%"><b>S’abonner à la liste Vibes</b></td>
    <td>Cette action de flux lance le processus d’abonnement SMS par le biais d’une campagne d’acquisition Vibes sélectionnée par l’utilisateur. Vibes envoie alors un message de confirmation auquel le destinataire doit répondre par « Y » dans les 24 heures pour confirmer son opt-in. Une fois que l’utilisateur a choisi de s’inscrire, il devient membre de la liste d’abonnements Vibes associée.</td>
  </tr>
  <tr>
    <td style="width:20%"><b>Se désabonner de la liste Vibes</b></td>
    <td>Cette action de flux désabonne chaque personne d’une liste d’abonnements Vibes activée par l’utilisateur. Lorsqu’un utilisateur envoie un SMS « STOP » à votre code, son enregistrement de personne est mis à jour pour refléter le fait qu’il n’est plus membre de la liste d’abonnements Vibes.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>Les flux **S’abonner à la liste Vibes** et **Se désabonner de la liste Vibes** ont des exigences différentes. Pour **S&#39;abonner**, vous devez sélectionner la liste Vibes et la campagne d&#39;acquisition Vibes. Pour **Unsubscribe**, seule la liste Vibes est requise.

>[!MORELIKETHIS]
>
>* [Envoyer un SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [Définir une liste dynamique pour une campagne dynamique | Déclencheur ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [Définir une liste dynamique pour une campagne dynamique | Lot ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
