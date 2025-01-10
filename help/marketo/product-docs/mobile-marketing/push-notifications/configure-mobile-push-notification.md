---
unique-page-id: 7512454
description: Configuration Des Notifications Push Mobiles - Documents Marketo - Documentation Du Produit
title: Configurer les notifications push mobiles
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 736e21d45d8a62e50f449e0ee6d0fc4df5963dfb
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Configurer les notifications push mobiles {#configure-mobile-push-notification}

1. Accédez à la zone **Activités marketing**.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Sélectionnez votre ressource push et cliquez sur **Modifier le brouillon**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Accédez à **Configuration**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Sélectionnez l’application de votre choix. Les plateformes Android et Apple sont activées par défaut.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

1. Si votre message push s&#39;applique à une seule plateforme (par exemple, les cas pour iPhone), vous pouvez exclure l&#39;autre plateforme en faisant glisser son sélecteur sur Désactivé.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

1. Cliquez sur **Suivant**.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Saisissez le texte du message ou sélectionnez l’icône de jeton pour ajouter des jetons. Sélectionnez ensuite une **Action de clic**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Si une plateforme est activée, elle s’affiche sur le côté gauche de l’écran du téléphone. Il s’affiche en couleur lorsqu’il est sélectionné.

   >[!NOTE]
   >
   >Il existe trois types d’actions de clic :
   >
   >**Lancer l’application** - **Cette application** ouvre la page d’accueil de votre application lorsque vous appuyez sur la notification. **Personnalisé** utilise un lien profond pour ouvrir d’autres zones de votre application ou de toute autre application vers laquelle vous disposez du lien (voir [URI de lien profond](#deep-link-uris) ci-dessous pour plus de détails).
   >
   >**Page de destination** - vous dirige vers une page de destination Marketo spécifiée.
   >
   >**URL externe** - vous dirige vers une page de destination autre que Marketo.

1. Pour insérer un lien profond pour une action d’appui personnalisée, cliquez sur Personnalisé et saisissez l’[URI du lien profond](#deep-link-uris) dans le champ.

   ![](assets/image2016-7-28-16-3a19-3a13.png)

1. Pour insérer des jetons, sélectionnez un jeton, saisissez une valeur par défaut, puis cliquez sur Insérer.

   >[!NOTE]
   >
   >Des jetons apparaissent à l’endroit où vous placez le curseur dans la zone de texte. Vous pouvez utiliser plusieurs jetons.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >Les messages et les actions de clic auront le même aspect sur les deux plateformes.

1. Pour iOS uniquement, cochez la case pour indiquer à l’application de lire un son à l’arrivée du message. Android lit le son automatiquement.

   ![](assets/ios-tap-and-notification-hand.png)

1. Prévisualisez l’autre plateforme et cliquez sur **Terminer**.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Cliquez sur **Approuver et fermer**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Félicitations ! Désormais, la notification push est prête à être envoyée.

## URI de lien profond {#deep-link-uris}

Lorsque les abonnés cliquent sur un bouton dans un message push, ils peuvent être redirigés vers la page d&#39;accueil de votre application ou directement vers une page spécifique de l&#39;application. Un lien profond est une référence unique à une page spécifique de votre application et ressemble beaucoup à un lien de site web.

Un URI de lien profond est constitué de trois parties : nom du schéma, chemin et identifiant. Dans l’exemple ci-dessous, « myappname » est le schéma. « products » est le chemin d’accès, et « purple-shirt » est l’identifiant. Lorsque le client appuie sur, il est dirigé spécifiquement vers l’élément de chemise violet dans les pages de produits de votre application.

![](assets/image2016-7-29-12-3a49-3a1.png)

Cela dit, la structure de lien profond de votre application peut être différente de l’exemple ci-dessus. Comme votre développeur dispose de nombreuses options pour définir des URI de lien profond, demandez-lui de vous envoyer les URI (liens) des pages que vous souhaitez utiliser. Cela permet de s’assurer que les URI que vous saisissez dans les messages push pointent vers les bons endroits. Votre développeur peut [trouver plus d’informations ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Envoyer une notification push mobile](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
