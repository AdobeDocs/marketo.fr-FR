---
unique-page-id: 7512454
description: Configuration de la notification push mobile - Documents Marketo - Documentation du produit
title: Configuration de la notification push mobile
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Configuration de la notification push mobile {#configure-mobile-push-notification}

1. Accédez au **Activités marketing** zone.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Sélectionnez votre ressource push et cliquez sur **Modifier le brouillon**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Accédez à **Configuration**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Sélectionnez l’application souhaitée. Les plateformes Android et Apple sont activées par défaut.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

1. Si votre message push s’applique à une seule plateforme (par exemple, pour les iPhones), vous pouvez exclure l’autre plateforme en glissant son sélecteur sur Désactivé.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

1. Cliquez sur **Suivant**.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Saisissez le texte du message ou sélectionnez l’icône de jeton à ajouter. Sélectionnez ensuite une **Appuyez sur Action**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Si une plateforme est activée, elle s’affiche sur le côté gauche de l’écran du téléphone. Il s’affiche en couleur lorsqu’il est sélectionné.

   >[!NOTE]
   >
   >Il existe trois types d’actions Appuyez sur :
   >
   >**Lancer l’application** - **Cette application** ouvre la page d’accueil de votre application lorsque la notification est activée. **Personnalisé** utilise un lien profond pour ouvrir d’autres zones de l’application ou de toute autre application à laquelle vous avez le lien (voir [URI de lien profond](#Deeplink) ci-dessous pour plus de détails).
   >
   >**Page d’entrée** - vous conduit à une page d’entrée Marketo spécifiée.
   >
   >**URL externe** - vous conduit à une page d’entrée non Marketo.

1. Pour insérer un lien profond pour une action d’appui personnalisée, cliquez sur Personnalisé et saisissez la variable [URI de lien profond](#Deeplink) dans le champ .

   ![](assets/image2016-7-28-16-3a19-3a13.png)

1. Pour insérer des jetons, sélectionnez un jeton, saisissez une valeur par défaut, puis cliquez sur Insérer.

   >[!NOTE]
   >
   >Les jetons apparaissent à l’endroit où vous placez le curseur dans la zone de texte. Vous pouvez utiliser plusieurs jetons.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >Les messages et les actions de Appuyez se présentent de la même manière sur les deux plateformes.

1. Pour iOS uniquement, cochez la case pour indiquer à l’application de lire un son à l’arrivée du message. Android lit le son automatiquement.

   ![](assets/ios-tap-and-notification-hand.png)

1. Prévisualisez l’autre plateforme et cliquez sur **Terminer**.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Cliquez sur **Approuver et fermer**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Félicitations ! La notification push est maintenant prête à être envoyée.

## URI de lien profond {#deep-link-uris}

Lorsque les abonnés cliquent sur un bouton dans un message push, ils peuvent être amenés à la page d’accueil de l’application ou directement à une page spécifique de l’application. Un lien profond est une référence unique à une page spécifique de votre application qui ressemble beaucoup à un lien de site web.

Un URI de lien profond se compose de trois parties : nom du schéma, chemin et identifiant. Dans l’exemple ci-dessous, &quot;myappname&quot; est le schéma. &quot;products&quot; est le chemin d’accès, et &quot;violet-chemise&quot; est l’identifiant. Lorsque le client clique, il est dirigé spécifiquement vers l’article &quot;T-shirt violet&quot; dans les pages de produits de votre application.

![](assets/image2016-7-29-12-3a49-3a1.png)

Cela dit, la structure des liens profonds de votre application peut être différente de l’exemple ci-dessus. Votre développeur dispose de nombreuses options pour définir les URI de lien profond. Demandez donc à votre développeur de vous envoyer les URI (liens) pour les pages que vous souhaitez utiliser. Cela permet de s’assurer que les URI que vous saisissez dans les messages push pointent vers les bons emplacements. Votre développeur peut [trouver plus d’informations ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Envoi d’une notification push mobile](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
