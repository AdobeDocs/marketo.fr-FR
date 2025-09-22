---
unique-page-id: 7512454
description: Configuration Des Notifications Push Mobiles - Documents Marketo - Documentation Du Produit
title: Configurer la notification push pour mobile
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 3%

---

# Configurer la notification push pour mobile {#configure-mobile-push-notification}

1. Accédez à la zone **[!UICONTROL Activités marketing]**.

   ![](assets/configure-mobile-push-notification-1.png)

1. Sélectionnez votre ressource push et cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/configure-mobile-push-notification-2.png)

1. Dans **Configuration**, sélectionnez l’application de votre choix. Les plateformes Android et Apple sont activées par défaut.

   ![](assets/configure-mobile-push-notification-3.png)

   >[!NOTE]
   >
   >Si votre message push s&#39;applique à une seule plateforme (par exemple, iOS), vous pouvez exclure l&#39;autre plateforme en faisant glisser manuellement son sélecteur sur **Désactivé**.

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/configure-mobile-push-notification-4.png)

1. Saisissez le texte du message ou sélectionnez l’icône de jeton pour ajouter des jetons (dans cet éditeur, les jetons sont formatés [comme d’habitude](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) vous pouvez utiliser plusieurs jetons). Sélectionnez une **Action d’appui**.

   ![](assets/configure-mobile-push-notification-5.png)

   >[!NOTE]
   >
   >Si une plateforme est activée, elle s’affiche sur le côté gauche de l’écran du téléphone. Il s’affiche en couleur lorsqu’il est sélectionné.

   >[!NOTE]
   >
   >Il existe trois types d’actions [!UICONTROL Appuyer] :
   >
   >**Lancer l’application** - **Cette application** ouvre la page d’accueil de votre application lorsque vous appuyez sur la notification. **Personnalisé** utilise un lien profond pour ouvrir d’autres zones de votre application ou de toute autre application vers laquelle vous disposez du lien (voir [URI de lien profond](#deep-link-uris) ci-dessous pour plus de détails).
   >
   >**[!UICONTROL Page de destination]** - vous dirige vers une page de destination Marketo spécifiée.
   >
   >**[!UICONTROL URL externe]** - vous dirige vers une page de destination autre que Marketo.

1. Pour insérer un lien profond pour une action d’appui personnalisée, sélectionnez **Personnalisé** et saisissez l’[URI de lien profond](#deep-link-uris) dans le champ.

   ![](assets/configure-mobile-push-notification-6.png)

   >[!NOTE]
   >
   >Les messages et les actions de clic auront le même aspect sur les deux plateformes.

1. Pour iOS uniquement, cochez la case pour indiquer à l’application de lire un son à l’arrivée du message. Android lit le son automatiquement.

   ![](assets/configure-mobile-push-notification-7.png)

1. Prévisualisez l’autre plateforme et cliquez sur **[!UICONTROL Terminer]**.

   ![](assets/configure-mobile-push-notification-8.png)

1. Cliquez sur **[!UICONTROL Approuver et fermer]**.

   ![](assets/configure-mobile-push-notification-9.png)

Félicitations ! Désormais, la notification push est prête à être envoyée.

## URI de lien profond {#deep-link-uris}

Lorsque les abonnés cliquent sur un bouton dans un message push, ils peuvent être redirigés vers la page d&#39;accueil de votre application ou directement vers une page spécifique de l&#39;application. Un lien profond est une référence unique à une page spécifique de votre application et ressemble beaucoup à un lien de site web.

Un URI de lien profond est constitué de trois parties : nom du schéma, chemin et identifiant. Dans l’exemple ci-dessous, « myappname » est le schéma. « products » est le chemin d’accès, et « purple-shirt » est l’identifiant. Lorsque le client appuie sur, il est dirigé spécifiquement vers l’élément de chemise violet dans les pages de produits de votre application.

![](assets/configure-mobile-push-notification-10.png)

Cela dit, la structure de lien profond de votre application peut être différente de l’exemple ci-dessus. Comme votre développeur dispose de nombreuses options pour définir des URI de lien profond, demandez-lui de vous envoyer les URI (liens) des pages que vous souhaitez utiliser. Cela permet de s’assurer que les URI que vous saisissez dans les messages push pointent vers les bons endroits. Votre développeur peut [trouver plus d’informations ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Envoyer une notification push mobile](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
