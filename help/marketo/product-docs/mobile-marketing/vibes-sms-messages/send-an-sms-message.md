---
description: Envoyer un message SMS - Documents Marketo - Documentation du produit
title: Envoyer un SMS
feature: Mobile Marketing
exl-id: 2c863ded-f441-4217-9541-6dcc442d9831
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Envoyer un SMS {#send-a-vibes-sms-message}

Vous avez [créé votre SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, il est maintenant temps de l&#39;envoyer. Vous pouvez l&#39;envoyer par lot ou par campagne de déclenchement.

>[!NOTE]
>
>Lors de l&#39;envoi de SMS :
>
>* déduplication Marketo Engage par numéro de téléphone. Ainsi, si plusieurs personnes ont le même numéro de téléphone, une seule personne recevra le message s’ils ne sont membres que d’une seule liste d’inscription Vibes. Le dédoublonnage est effectué au niveau de la liste d’abonnements Vibes, et non au niveau du programme Marketo.
>* Marketo n’enverra pas aux personnes placées sur la liste bloquée ou Marketing suspendu.
>* Un SMS ne sera envoyé à personne désabonné s’il ne figure pas dans la liste de la base de données mobile de Vibes.

## Envoyer un SMS par lots {#send-a-batch-sms}

1. Dans Mon Marketo, cliquez sur **Activités marketing**.

   ![](assets/send-an-sms-message-1.png)

1. Recherchez et sélectionnez une campagne dynamique.

   ![](assets/send-an-sms-message-2.png)

1. Cliquez sur l&#39;onglet **Liste dynamique** et définissez l&#39;audience du SMS. Dans cet exemple, nous envoyons à toutes les personnes de notre base de données dont &quot;Adobe&quot; est répertorié comme leur société.

   ![](assets/send-an-sms-message-3.png)

1. Dans l’onglet **Flux**, placez le curseur sur **Envoyer un message SMS**. Sélectionnez la liste SMS et vidéos souhaitée dans les listes déroulantes.

   ![](assets/send-an-sms-message-4.png)

   >[!NOTE]
   >
   >Le sélecteur de liste de vidéos sert de filtre supplémentaire pour l’audience déjà identifiée dans la liste dynamique afin de cibler uniquement les personnes qui appartiennent à cette liste.

1. Cliquez sur l&#39;onglet **Planning** et planifiez votre SMS.

   ![](assets/send-an-sms-message-5.png)

## Envoyer un SMS de déclenchement {#send-a-trigger-sms}

1. Dans Mon Marketo, cliquez sur **Activités marketing**.

   ![](assets/send-an-sms-message-6.png)

1. Recherchez et sélectionnez une campagne dynamique.

   ![](assets/send-an-sms-message-7.png)

1. Cliquez sur l’onglet **Liste dynamique** , sélectionnez le déclencheur désiré et définissez sa valeur. Dans cet exemple, nous utilisons **Remplit le formulaire**.

   ![](assets/send-an-sms-message-8.png)

1. Dans l’onglet **Flux**, placez le curseur sur **Envoyer un message SMS**. Sélectionnez la liste SMS et vidéos souhaitée dans les listes déroulantes.

   ![](assets/send-an-sms-message-9.png)

   >[!NOTE]
   >
   >Le sélecteur de liste de vidéos sert de filtre supplémentaire pour l’audience déjà identifiée dans la liste dynamique afin de cibler uniquement les personnes qui appartiennent à cette liste.

1. Cliquez sur l’onglet **Planning** , puis **Activer**.

   ![](assets/send-an-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Créer un message vidéo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}
>* [Utilisation des options SMS dans une campagne dynamique](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/using-sms-options-in-a-smart-campaign.md){target="_blank"}
