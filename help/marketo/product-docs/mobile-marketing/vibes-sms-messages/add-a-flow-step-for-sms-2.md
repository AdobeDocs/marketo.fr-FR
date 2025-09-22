---
description: Ajouter une étape de flux pour SMS - Documents Marketo - Documentation du produit
title: Ajouter une étape de flux pour les SMS
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 3%

---

# Ajouter une étape de flux pour les SMS {#add-a-flow-step-for-sms}

Marketo Engage comporte trois étapes de flux que vous pouvez utiliser dans vos campagnes intelligentes SMS :

<table>
<tbody>
  <tr>
    <td style="width:25%">Envoyer un message SMS</td>
    <td>Cette action de flux envoie des messages aux personnes de la liste dynamique Marketo qui sont abonnées à une liste d’abonnements Vibes activée par l’utilisateur. Il ne lance pas le processus d’abonnement. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-a-vibes-sms-message.md">En savoir plus</a>.</td>
  </tr>

<tr>
    <td style="width:25%">S’abonner à la liste Vibes</td>
    <td>Cette action de flux lance le processus d’abonnement SMS par le biais d’une campagne d’acquisition Vibes sélectionnée par l’utilisateur. Vibes envoie alors un message de confirmation auquel le destinataire doit répondre par « Y » dans les 24 heures pour confirmer son opt-in. Une fois que l’utilisateur a choisi de s’inscrire, il devient membre de la liste d’abonnements Vibes associée.</td>
  </tr>
  <tr>
    <td style="width:25%">Se désabonner de la liste Vibes</td>
    <td>Cette action de flux désabonne chaque personne d’une liste d’abonnements Vibes activée par l’utilisateur. Lorsqu’un utilisateur envoie un SMS « STOP » à votre code, son enregistrement de personne est mis à jour pour refléter le fait qu’il n’est plus membre de la liste d’abonnements Vibes.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>Lors de l’envoi de SMS :
>
>* Marketo déduplique par numéro de téléphone. Ainsi, si plusieurs personnes ont le même numéro de téléphone, une seule personne recevra le message si elle est membre d&#39;une seule liste d&#39;abonnements Vibes. Le dédoublonnage est effectué au niveau de la liste d’abonnements Vibes, et non au niveau du programme Marketo.
>* Marketo placer sur la liste bloquée n’enverra pas de messages aux personnes qui sont bloquées ou dont le marketing est suspendu.

Pour obtenir des informations générales sur la configuration des étapes de flux, voir [Ajouter une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Voici les principes de base régissant l’utilisation des SMS.

1. Dans Mon Marketo, cliquez sur **Activités marketing**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Recherchez et sélectionnez la campagne intelligente à laquelle vous souhaitez ajouter le flux SMS.

   CAPTURE D’ÉCRAN

1. Dans l’onglet Liste dynamique , choisissez le ou les déclencheurs souhaités (par exemple, « Formulaire rempli »).

   CAPTURE D’ÉCRAN

1. Dans l’onglet **Flux**, faites glisser sur l’étape de flux (par exemple, **Envoyer un SMS**). Sélectionnez le SMS et la liste Vibes dans les listes déroulantes.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Le sélecteur de liste Vibes agit comme un filtre supplémentaire sur l’audience déjà identifiée dans la liste dynamique afin de cibler uniquement les prospects appartenant à cette liste Vibes.
   >
   >Les flux **S’abonner à la liste Vibes** et **Se désabonner de la liste Vibes** ont des exigences différentes. Pour **S&#39;abonner**, vous devez sélectionner la liste Vibes et la campagne d&#39;acquisition Vibes. Pour **Unsubscribe**, seule la liste Vibes est requise.
