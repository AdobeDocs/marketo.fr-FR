---
description: Créer un message SMS Vibes - Documents Marketo - Documentation du produit
title: Création d’un message SMS Vibes
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 3%

---

# Création d’un message SMS Vibes {#create-a-vibes-sms-message}

Voici comment créer un SMS Vibes.

>[!AVAILABILITY]
>
>Cette fonctionnalité est disponible en tant que module complémentaire pour votre compte Adobe Marketo Engage. Pour qu’il soit correctement configuré, il doit être acheté par Adobe. Pour plus d’informations, contactez l’équipe de compte d’Adobe (votre gestionnaire de compte).

1. Accédez à **Activités marketing**.

   ![](assets/mobile-right-click-hand.jpg)

1. Cliquez avec le bouton droit de la souris sur un programme et sélectionnez **Nouvelle ressource locale**.

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
   >La limite de caractères d&#39;un SMS est de 160 caractères à l&#39;aide du jeu de caractères ASCII standard. Si vous dépassez 160 caractères, votre message sera fractionné en fonction du nombre total de caractères.

1. Cliquez sur **Jeton** dans le menu Insérer pour ajouter un jeton à votre message.

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >L’ajout d’un jeton peut provoquer le dépassement de la limite de caractères du message. Le message se divise alors, ce qui entraîne la création de messages supplémentaires.

   >[!IMPORTANT]
   >
   >Conformité SMS : tous les SMS sortants doivent inclure le nom de la marque ou la description du programme. Les instructions HELP et STOP doivent être fournies au moins une fois par mois et par abonné pour les programmes de messages récurrents.

   ?????? L’utilisation du réducteur d’URL Marketo entraîne l’utilisation de X caractères dans votre message ??????

1. Cliquez sur **Lien** dans le menu Insérer pour ajouter un lien vers votre message.

   ![](assets/full-message-link-hand.jpg)

1. Sélectionnez un type de lien. La page d’entrée Marketo est la page par défaut. Si vous procédez de la sorte, vous devez sélectionner la landing page dans la liste déroulante, puis cliquer sur **Insérer**.

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >* Les deux liens de tracking sont sélectionnés par défaut.
   >* L’utilisation du réducteur d’URL Marketo entraîne l’utilisation de X caractères dans votre message.??????????????????

1. Si vous souhaitez utiliser une URL externe à la place, cliquez sur le bouton **URL externe** et saisissez l’URL dans le champ URL . Cliquez sur **Insérer**.

   ![](assets/insert-link-url-hands.jpg)

   >[!CAUTION]
   >
   >Il est recommandé de _not_ utilisez des réducteurs d’URL (par exemple, Bisément), car les opérateurs peuvent signaler votre message comme indésirable.

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

LIMIT AMÉRICAIN????????
