---
description: Envoi d’un message SMS Vibes - Documents Marketo - Documentation du produit
title: Envoi d’un SMS de vidéos
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: d4bd94b22b4f9da993150a94d2757014cbf87d80
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Envoi d’un SMS de vidéos {#send-a-vibes-sms-message}

Vous avez [création de votre SMS Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md), il est maintenant temps de l&#39;envoyer. Vous pouvez l&#39;envoyer par lot ou par campagne de déclenchement.

>[!NOTE]
>
>Lors de l&#39;envoi de SMS :
>
>* déduplication Marketo Engage par numéro de téléphone. Ainsi, si plusieurs personnes ont le même numéro de téléphone, une seule personne recevra le message s’ils ne sont membres que d’une seule liste d’inscription Vibes. Le dédoublonnage est effectué au niveau de la liste d’abonnements Vibes, et non au niveau du programme Marketo.
>* Marketo n’enverra pas aux personnes placées sur la liste bloquée ou Marketing suspendu.

## Envoyer un SMS par lots {#send-a-batch-sms}

1. Dans Mon Marketo, cliquez sur **Activités marketing**.

   ![](assets/send-a-vibes-sms-message-1.png)

1. Recherchez et sélectionnez une campagne dynamique.

   ![](assets/send-a-vibes-sms-message-2.png)

1. Cliquez sur le bouton **Liste dynamique** et définissez l&#39;audience du SMS. Dans cet exemple, nous envoyons à toutes les personnes de notre base de données dont &quot;Adobe&quot; est répertorié comme leur société.

   ![](assets/send-a-vibes-sms-message-3.png)

1. Dans le **Flux** onglet, glisser dessus **Envoyer un message SMS**. Sélectionnez la liste SMS et vidéos souhaitée dans les listes déroulantes.

   ![](assets/send-a-vibes-sms-message-4.png)

   >[!NOTE]
   >
   >Le sélecteur de liste de vidéos sert de filtre supplémentaire pour l’audience déjà identifiée dans la liste dynamique afin de cibler uniquement les personnes qui appartiennent à cette liste.

1. Cliquez sur le bouton **Planification** et planifiez votre SMS.

   ![](assets/send-a-vibes-sms-message-5.png)

## Envoyer un SMS de déclenchement {#send-a-trigger-sms}

1. Dans Mon Marketo, cliquez sur **Activités marketing**.

   ![](assets/send-a-vibes-sms-message-6.png)

1. Recherchez et sélectionnez une campagne dynamique.

   ![](assets/send-a-vibes-sms-message-7.png)

1. Cliquez sur le bouton **Liste dynamique** , sélectionnez le déclencheur désiré et définissez sa valeur. Dans cet exemple, nous utilisons **Remplir le formulaire**.

   ![](assets/send-a-vibes-sms-message-8.png)

1. Dans le **Flux** onglet, glisser dessus **Envoyer un message SMS**. Sélectionnez la liste SMS et vidéos souhaitée dans les listes déroulantes.

   ![](assets/send-a-vibes-sms-message-9.png)

   >[!NOTE]
   >
   >Le sélecteur de liste de vidéos sert de filtre supplémentaire pour l’audience déjà identifiée dans la liste dynamique afin de cibler uniquement les personnes qui appartiennent à cette liste.

1. Cliquez sur le bouton **Planification** , puis **Activer**.

   ![](assets/send-a-vibes-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Création d’un message vidéo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)
>* Étapes de flux de vidéos

