---
unique-page-id: 11378869
description: Créer un message SMS Vibes - Documents Marketo - Documentation du produit
title: Création d’un message SMS Vibes
exl-id: 9ec0da97-7a80-4c40-be79-be08d7d1d9c1
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 3%

---

# Création d’un message SMS Vibes {#create-a-vibes-sms-message}

Voici comment créer un SMS Vibes.

>[!AVAILABILITY]
>
>Cette fonctionnalité est disponible en tant que module complémentaire pour votre compte Adobe Marketo Engage. Pour qu’il soit correctement configuré, il doit être acheté par Adobe. Pour plus d’informations, contactez l’équipe de compte d’Adobe (votre gestionnaire de compte).

>[!NOTE]
>
>Les SMS ne sont pas conformes à la loi HIPAA.

1. Accédez à **Activités marketing** et cliquez avec le bouton droit de la souris sur un programme.

   ![](assets/mobile-right-click-hand.jpg)

1. Cliquez sur **Nouvelle ressource locale**.

   ![](assets/new-local-asset-hand.jpg)

   >[!TIP]
   >
   >Vous pouvez également cliquer sur le bouton **Nouveau** menu déroulant.

1. Cliquez sur **SMS Message**.

   ![](assets/new-local-asset-selection-hand.jpg)

1. Saisissez un nom et une description facultative pour le nouveau SMS, puis cliquez sur **Créer**.

   ![](assets/new-sms-message-offer-ends-soon-hands.jpg)

1. Cliquez sur **Modifier le brouillon**.

   ![](assets/edit-draft-hand.jpg)

1. Dans l’éditeur de messages, cliquez à l’intérieur de la bulle bleue et commencez à saisir du texte.

   ![](assets/message-text-pencil.jpg)

   >[!NOTE]
   >
   >Les limites des États-Unis et du Canada sont différentes, à 160 et 130 caractères respectivement. Si vous dépassez ces limites de caractères, votre message peut être fractionné. Bien que nous l’indiquions lorsque vous dépassez la limite canadienne, l’éditeur est optimisé pour les États-Unis et divise le message en fonction de la limite américaine.

1. Cliquez sur **Jeton** dans le menu Insérer pour ajouter un jeton à votre message.

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >L’ajout d’un jeton peut provoquer le dépassement de la limite de caractères du message. Le message sera alors divisé, ce qui entraînera des frais supplémentaires.

1. Cliquez sur **Lien** dans le menu Insérer pour ajouter un lien vers votre message.

   ![](assets/full-message-link-hand.jpg)

1. Sélectionnez un type de lien. La page d’entrée Marketo est la page par défaut. Si vous procédez de la sorte, vous devez sélectionner la landing page dans la liste déroulante, puis cliquer sur **Insérer**.

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >Les deux liens de tracking sont sélectionnés par défaut.

1. Si vous souhaitez utiliser une URL externe à la place, cliquez sur le bouton **URL externe** et saisissez l’URL dans le champ URL . Cliquez sur **Insérer**.

   ![](assets/insert-link-url-hands.jpg)

1. Le lien s’affiche dans le message.

   ![](assets/link-added.jpg)

   >[!NOTE]
   >
   >Marketo affiche un aperçu des liens du domaine de suivi de marque. Si vous décochez la case du lien mkt_tok, le lien est modifié. Décochez également la case Lien de suivi et l’URL sera raccourcie à sa longueur de base (par exemple, www.mygooglepage.com).

   ![](assets/image2016-7-27-16-3a20-3a16.png)

   >[!NOTE]
   >
   >Le nombre de caractères ne reflète que les caractères contenus dans le message le plus bas.

Si vous insérez plus que la limite E.U., l&#39;éditeur divise votre message en sections. La limite totale absolue est de 900 caractères. Une fois cette limite atteinte, le message sera automatiquement tronqué lorsqu’il sera envoyé à son audience.
