---
description: Ajout d’une étape de flux pour SMS - Documents Marketo - Documentation du produit
title: Ajout d’une étape de flux pour un SMS
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: fee2d692acd8d54f2e308e2d5edc9876d13d5a4d
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 2%

---

# Ajout d’une étape de flux pour un SMS {#add-a-flow-step-for-sms}

Marketo Engage comprend trois étapes de flux que vous pouvez utiliser dans vos campagnes dynamiques SMS :

<table>
<tbody>
  <tr>
    <td style="width:25%">Envoyer un message SMS</td>
    <td>Cette action de flux envoie des messages aux personnes de la liste dynamique Marketo qui sont abonnées à une liste d’abonnements Vibes de souscription de l’utilisateur. Il ne lance pas le processus d’abonnement. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-a-vibes-sms-message.md">En savoir plus</a>.</td>
  </tr>

<tr>
    <td style="width:25%">S’abonner à la liste Vibes</td>
    <td>Cette action de flux lance le processus d'inscription SMS via une campagne d'acquisition Vibes sélectionnée par l'utilisateur. Vibes envoie alors un message de confirmation, auquel le destinataire doit répondre avec "Y" dans les 24 heures pour confirmer l'opt-in. Une fois que l’utilisateur s’est inscrit, il deviendra membre de la liste d’abonnements Vibes associée.</td>
  </tr>
  <tr>
    <td style="width:25%">Se désabonner de la liste Vibes</td>
    <td>Cette action de flux désabonne chaque personne de la liste d’abonnement Vibes de l’utilisateur. Lorsqu’un utilisateur envoie un SMS "STOP" à votre code, son enregistrement de personne est mis à jour pour indiquer qu’il n’est plus membre de la liste d’abonnement Vibes.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>Lors de l&#39;envoi de SMS :
>
>* Marketo déduplique par numéro de téléphone. Ainsi, si plusieurs personnes ont le même numéro de téléphone, une seule personne recevra le message s’ils ne sont membres que d’une seule liste d’inscription Vibes. Le dédoublonnage est effectué au niveau de la liste d’abonnements Vibes, et non au niveau du programme Marketo.
>* Marketo n’enverra pas aux personnes placées sur la liste bloquée ou Marketing suspendu.

Pour des informations générales sur la configuration des étapes de flux, voir [Ajout d’une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Voici les principes de base de l’utilisation des SMS.

1. Dans Mon Marketo, cliquez sur **Activités marketing**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Recherchez et sélectionnez la campagne dynamique à laquelle vous souhaitez ajouter le flux SMS.

   CAPTURE D’ÉCRAN

1. Dans l’onglet Liste dynamique , sélectionnez le ou les déclencheurs souhaités (par exemple, &quot;Formulaire rempli&quot;).

   CAPTURE D’ÉCRAN

1. Dans l’onglet **Flux**, faites glisser l’étape de flux (par exemple, **Envoyer un message SMS**). Sélectionnez le SMS et la liste Vibes dans les listes déroulantes.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Le sélecteur de liste de vidéos sert de filtre supplémentaire pour l’audience déjà identifiée dans la liste dynamique afin de cibler uniquement les pistes qui appartiennent à cette liste.
   >
   >Les flux **S’abonner à la liste des vidéos** et **Se désabonner de la liste des vidéos** ont des exigences différentes. Pour **S’abonner**, vous devez sélectionner la liste Vibes et la campagne d’acquisition Vibes. Pour **Se désabonner**, seule la liste Vibes est requise.
