---
unique-page-id: 11379045
description: Ajout d’une étape de flux pour SMS - Documents Marketo - Documentation du produit
title: Ajout d’une étape de flux pour un SMS
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Ajout d’une étape de flux pour un SMS {#add-a-flow-step-for-sms}

Marketo comprend trois étapes de flux que vous pouvez utiliser dans vos campagnes SMS intelligentes :

* **Envoyer un message SMS** - Cette action de flux envoie des messages aux personnes de la liste intelligente Marketo qui sont inscrites à une liste d’abonnements Vibes sélectionnée par l’utilisateur. Il ne lance pas le processus d’abonnement.
* **Abonnement à la liste des vidéos** - Cette action de flux lance le processus d&#39;inscription SMS via une campagne d&#39;acquisition de vidéos sélectionnée par l&#39;utilisateur. Vibes envoie alors un message de confirmation, auquel le destinataire doit répondre pour terminer le processus d&#39;inscription.
* **Se désabonner de la liste Vibes** - Cette action de flux désabonne chaque personne d’une liste d’abonnements Vibes sélectionnée par l’utilisateur.

>[!NOTE]
>
>Lors de l&#39;envoi de SMS :
>
>* Marketo déduplique par numéro de téléphone. Ainsi, si plusieurs personnes ont le même numéro de téléphone, une seule personne recevra le message.
>* Marketo n’enverra pas aux personnes placées sur la liste bloquée ou Marketing suspendu.

Pour obtenir des informations générales sur la configuration des étapes de flux, voir [Ajout d’une étape de flux à une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Voici les principes de base de l’utilisation des SMS.

1. Dans Mon Marketo, cliquez sur **Activités marketing**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Recherchez la campagne dynamique à laquelle vous souhaitez ajouter le flux SMS. Cliquez sur le bouton **Flux** .

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Faites glisser le curseur sur le flux, par exemple : **Envoyer un message SMS**. Sélectionnez le SMS et la liste Vibes dans les listes déroulantes.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Le sélecteur de liste de vidéos sert de filtre supplémentaire pour l’audience déjà identifiée dans la liste dynamique afin de cibler uniquement les pistes qui appartiennent à cette liste.
   >
   >La variable **Abonnement à la liste des vidéos** et **Se désabonner de la liste Vibes** les flux ont des exigences différentes. Pour **Abonner**, vous devez sélectionner la liste Vibes et la campagne d&#39;acquisition Vibes . Pour **Désabonner**, seule la liste Vibes est requise.
