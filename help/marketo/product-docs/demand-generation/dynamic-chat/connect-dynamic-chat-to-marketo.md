---
description: Connexion de Dynamic Chat à Marketo - Documents Marketo - Documentation du produit
title: Connexion de la messagerie dynamique à Marketo
exl-id: bad6c2dc-d4e7-4f98-bf6d-743043f96e4e
source-git-commit: bb2620ab72987cf857a7144aca21e94a11f29d90
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Connexion de la messagerie dynamique à Marketo {#connect-dynamic-chat-to-marketo}

Une fois que vous avez terminé la [configuration initiale](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md), il est temps d’effectuer une synchronisation unique en connectant Dynamic Chat à votre abonnement Marketo.

1. Dans Mon Marketo, cliquez sur le bouton **Chat dynamique** mosaïque.

   ![](assets/connect-dynamic-chat-to-marketo-1.png)

   >[!NOTE]
   >
   >Si la mosaïque ne s’affiche pas, contactez votre administrateur Marketo.

1. Si vous avez déjà accédé à une application avec une Adobe ID, vous accédez directement à Dynamic Chat. Si ce n’est pas le cas, [Configuration de votre Adobe ID](https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html).

1. Pour connecter votre instance Marketo, sélectionnez **Intégrations**.

   ![](assets/connect-dynamic-chat-to-marketo-2.png)

1. Sur la carte Marketo, cliquez sur **Lancer la synchronisation**.

   ![](assets/connect-dynamic-chat-to-marketo-3.png)

1. Sélectionnez jusqu’à 50 champs standard ou personnalisés à synchroniser avec la messagerie instantanée. Cliquez sur **Suivant** une fois terminé.

   ![](assets/connect-dynamic-chat-to-marketo-4.png)

   >[!CAUTION]
   >
   >À l’heure actuelle, sélections d’attributs **cannot** être modifié après la synchronisation initiale. Une fois la synchronisation terminée, vous pouvez revenir en arrière et en ajouter davantage (si vous avez choisi moins de 50).

1. Assurez-vous de disposer des sélections correctes (rappel : vous ne pouvez pas supprimer les attributs post-synchronisation. cliquez sur **Modifier les sélections** si vous devez en modifier une au cours de cette étape). Cliquez sur **Confirmer** lorsque vous avez terminé pour lancer la synchronisation.

   ![](assets/connect-dynamic-chat-to-marketo-5.png)

>[!NOTE]
>
>Selon la taille de votre base de données, la synchronisation peut prendre entre 2 et 24 heures.

## Lier votre organisation d’Adobe et Marketo {#link-your-adobe-org-and-marketo}

Ensuite, il est temps de lier Adobe et Marketo.

1. Connectez-vous à [experience.adobe.com](https://experience.adobe.com).

1. Copiez l’ID d’organisation dans le coin inférieur droit de la page d’accueil, _moins_ le &quot;@AdobeOrg.&quot;

   ![](assets/connect-dynamic-chat-to-marketo-6.png)

1. Dans Marketo, accédez au **Administration** et sélectionnez **Mappage de l’organisation Adobe**.

   ![](assets/connect-dynamic-chat-to-marketo-7.png)

1. Cliquez sur **Modifier**.

   ![](assets/connect-dynamic-chat-to-marketo-8.png)

1. Collez l’ID d’organisation que vous avez copié à l’étape 2, puis cliquez sur **OK**.

   ![](assets/connect-dynamic-chat-to-marketo-9.png)

>[!MORELIKETHIS]
>
>[Configuration initiale](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md)
