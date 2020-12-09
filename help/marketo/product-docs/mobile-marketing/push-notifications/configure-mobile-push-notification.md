---
unique-page-id: 7512454
description: Configurer la notification Push mobile - Documents marketing - Documentation du produit
title: Configuration de la notification Push mobile
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Configuration de la notification Push mobile {#configure-mobile-push-notification}

1. Accédez à la zone Activités marketing.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Sélectionnez votre fichier Push et cliquez sur **Modifier le brouillon**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Accédez à **Configuration**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Sélectionnez l’application de votre choix. Les plateformes Android et Apple sont activées par défaut.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

   Si votre message Push s’applique à une seule plate-forme (par exemple, pour les iPhones), vous pouvez exclure l’autre en déplaçant son sélecteur sur Désactivé.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

   Cliquez sur SUIVANT.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Entrez le texte du message ou sélectionnez l’icône de jeton pour ajouter des jetons. Sélectionnez ensuite une action **** Appuyez sur.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Si une plate-forme est activée, elle s’affiche sur le côté gauche de l’écran de smartphone. Il s’affiche en couleur lorsqu’il est sélectionné.

   >[!NOTE]
   >
   >**Définition**
   >
   >
   >Il existe trois types d’actions d’appui** :**
   >
   >
   >**Lancer l&#39;application** : **cette application** ouvre la page d&#39;accueil de votre application lorsque la notification est activée. **Personnalisé** utilise un lien profond pour ouvrir d’autres zones de votre application ou de toute autre application à laquelle vous disposez du lien (voir les URI [de lien](#Deeplink) profond ci-dessous pour plus d’informations).
   >
   >
   >**landing page** : vous conduit à un landing page Marketo spécifié.
   >
   >
   >**URL** externe : vous conduit à un landing page non-marketing.

   Pour insérer un lien profond pour une action de contact personnalisée, cliquez sur Personnalisé et saisissez l’URI [de lien](#Deeplink) profond dans le champ.

   ![](assets/image2016-7-28-16-3a19-3a13.png)

   Pour insérer des jetons, sélectionnez un jeton, entrez une valeur par défaut, puis cliquez sur Insérer.

   >[!NOTE]
   >
   >Les jetons apparaissent à l’endroit où vous placez le curseur dans la zone de texte. Vous pouvez utiliser plusieurs jetons.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >Les messages et les actions de clic seront identiques sur les deux plates-formes.

   Pour iOS uniquement, cochez la case pour indiquer à l’application de lire un son lorsque le message arrive. Android lit automatiquement le son.

   ![](assets/ios-tap-and-notification-hand.png)

   Prévisualisation l’autre plateforme et cliquez sur FINISH.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Cliquez sur **APPROUVER ET FERMER**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Félicitations ! Désormais, la notification Push est prête à être envoyée.

## URI de lien profond {#deep-link-uris}

Lorsque les abonnés cliquent sur un bouton d’un message Push, ils peuvent être dirigés vers la page d&#39;accueil de votre application ou directement vers une page spécifique de l’application. Un lien profond est une référence unique à une page spécifique de votre application et ressemble beaucoup à un lien de site Web.

Un URI de lien profond est constitué de trois parties : nom, chemin et identifiant du schéma. Dans l’exemple ci-dessous, &quot;myappname&quot; est le schéma. &quot;products&quot; est le chemin d’accès et &quot;pourpre-shirt&quot; est l’identifiant. Lorsque le client touche, il est dirigé spécifiquement vers l’objet de chemise violette dans les pages de produit de votre application.

![](assets/image2016-7-29-12-3a49-3a1.png)

Cela dit, la structure des liens profonds de votre application peut être différente de l’exemple ci-dessus. Votre développeur dispose de nombreuses options pour définir les URI des liens profonds. Demandez donc à votre développeur de vous envoyer les URI (liens) pour les pages que vous souhaitez utiliser. Ceci garantit que les URI que vous saisissez dans les messages push pointent vers les bons emplacements. Votre développeur peut [trouver plus d&#39;informations ici](http://developers.marketo.com/mobile/enabling-deep-links-in-your-app/).

>[!MORELIKETHIS]
>
>* [Envoyer une notification Push mobile](send-a-mobile-push-notification.md)

>



