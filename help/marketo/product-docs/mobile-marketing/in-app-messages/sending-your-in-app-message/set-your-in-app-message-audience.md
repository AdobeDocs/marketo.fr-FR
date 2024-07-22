---
unique-page-id: 10617431
description: Définition de l’audience du message in-app - Documents Marketo - Documentation du produit
title: Définition de l’audience du message in-app
exl-id: 696ae5b6-7063-41bc-bcef-27879182ff1e
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Définition de l’audience du message in-app {#set-your-in-app-message-audience}

La première étape consiste à décider qui doit recevoir votre message in-app. Vous devez configurer votre liste dynamique.

1. Cliquez sur **Modifier la liste dynamique**.

   ![](assets/image2016-5-9-15-3a15-3a7.png)

1. Dans la liste dynamique, le déclencheur Avec activité d’application mobile est automatiquement renseigné. Cliquez sur la liste déroulante et sélectionnez l’application dans laquelle vous souhaitez placer le message.

   ![](assets/image2016-5-9-15-3a18-3a10.png)

   >[!NOTE]
   >
   >Plusieurs valeurs pour le champ Application mobile ne sont actuellement pas prises en charge pour les programmes de messages in-app.

1. **App Open** est le paramètre d’action par défaut, mais vous pouvez sélectionner n’importe quel événement personnalisé que vous avez déjà configuré.

   ![](assets/image2016-5-9-15-3a20-3a23.png)

   >[!NOTE]
   >
   >Le déclencheur par défaut (ouverture de l’application) et les déclencheurs personnalisés ajoutés au code par votre développeur s’affichent automatiquement dans le sélecteur Action. Si un événement personnalisé est manquant, contactez votre développeur pour vous assurer qu’il a ajouté les événements personnalisés à l’application. Gardez à l’esprit que le processus d’approbation et de codage des événements personnalisés peut prendre du temps. Voir [cet article](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md) pour plus d’informations.

1. Des contraintes sont disponibles pour le déclencheur **Avec activité d’application mobile** si vous en avez besoin.

   ![](assets/image2016-5-9-15-3a22-3a27.png)

1. Vous pouvez ajouter des filtres à votre liste dynamique pour limiter la réception de votre message in-app. Dans cet exemple, en utilisant le filtre **Date d’acquisition**, seules les personnes acquises le 9 juin 2016 recevront le message in-app.

   ![](assets/image2016-5-9-15-3a26-3a2.png)

1. Revenez à votre Panneau de Contrôle de messages in-app. Définissez la limite d’affichage dans la liste déroulante.

   ![](assets/image2016-5-9-15-3a30-3a35.png)

   >[!NOTE]
   >
   >La limite d’affichage par défaut est **Une fois par session**. Si vous souhaitez que le message cesse de s’afficher après la réponse du destinataire, sélectionnez **A chaque fois que l’utilisateur n’a pas appuyé sur**. S&#39;il doit s&#39;afficher à chaque fois, quel que soit le destinataire, choisissez **Chaque fois**.

   ![](assets/image2016-5-9-15-3a32-3a6.png)

Beau travail ! Vous avez votre audience définie. Vous avez gagné la barre bleue et la coche verte.

Temps jusqu’à [sélectionner votre message in-app](/help/marketo/product-docs/mobile-marketing/in-app-messages/sending-your-in-app-message/select-your-in-app-message.md) !
