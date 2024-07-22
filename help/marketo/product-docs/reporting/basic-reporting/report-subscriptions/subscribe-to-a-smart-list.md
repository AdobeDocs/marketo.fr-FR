---
unique-page-id: 7505310
description: Abonnement à une liste dynamique - Documents Marketo - Documentation du produit
title: Abonnement à une liste dynamique
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 1%

---

# Abonnement à une liste dynamique {#subscribe-to-a-smart-list}

L’abonnement à des listes dynamiques est un excellent moyen de suivre les personnes, avec des rapports envoyés directement à votre boîte de réception.

Vous pouvez créer un abonnement à une liste dynamique à deux endroits distincts :

* Activités marketing
* Base de données

Les abonnements utilisent la liste complète des personnes au moment de l’exécution de l’abonnement.

Les abonnements résident là où se trouve votre liste dynamique, dans les activités marketing ou la base de données.

Vous pouvez créer plusieurs abonnements à partir de la même liste dynamique.

Les abonnements sont spécifiques à l&#39;espace de travail. Par exemple, cette liste d’abonnements se trouve dans un espace de travail différent de ceux affichés dans le reste de cet article :

![](assets/one.png)

>[!NOTE]
>
>Vous êtes limité à 100 abonnements et un maximum de 100 000 personnes par abonnement, sur l’ensemble des espaces de travail, par instance Marketo. Si la liste dynamique contient plus de 100 000 noms, Marketo exécute l’abonnement pour les 100 000 premiers noms.

## Création d’un abonnement à une liste dynamique {#create-a-smart-list-subscription}

1. Accédez à la **base de données** ou **Activités marketing**.

   ![](assets/db.png)

1. Sélectionnez la liste dynamique pour laquelle vous souhaitez créer un abonnement. Cliquez sur **Actions de liste** et sélectionnez **Nouvel abonnement à une liste dynamique**.

   ![](assets/three.png)

1. Donnez un **Nom** à votre abonnement, puis sélectionnez ou saisissez les adresses électroniques des **destinataires**.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. Cliquez sur la liste **Fréquence** et sélectionnez une fréquence.

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. Définissez la date **Fin de diffusion**. Vous pouvez sélectionner **Jamais** ou une date de calendrier.

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. Cliquez sur **Format** et faites votre choix dans la liste.

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. Cliquez sur **Créer**.

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. Votre nouvel abonnement à une liste dynamique s’affiche en haut de la liste dans l’onglet Abonnements . Cliquez sur **Envoyer** si vous souhaitez envoyer maintenant, et n’attendez pas la diffusion de l’email planifiée.

   ![](assets/eight.png)

1. Nous vous recommandons de décocher la case Actif pour désactiver un abonnement à une liste dynamique si personne ne s’y abonne.

   ![](assets/nine.png)

   C&#39;était facile, non ?

## Message électronique {#email-message}

Les destinataires recevront un email avec la possibilité de télécharger le rapport, ainsi qu&#39;un lien directement vers la liste au sein de l&#39;instance Marketo. Le lien de téléchargement expire dans quatre jours.

>[!NOTE]
>
>Si le paramètre [Admin d’abonnement sécurisé](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) est défini sur **Oui**, seules les personnes ayant accès à l’instance Marketo pourront télécharger le rapport.

![](assets/image2015-4-17-15-3a46-3a47.png)

Si un rapport contient 0 personne, les destinataires recevront toujours un email. Cependant, l&#39;email indique simplement qu&#39;il n&#39;y a personne à signaler.

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>Lorsque vous modifiez un filtre de liste dynamique sur lequel vous avez basé un abonnement, il met également à jour le rapport.

L&#39;email fournit également des informations supplémentaires sur les filtres utilisés pour créer la liste.

## Suppression d’un abonnement {#delete-a-subscription}

Pour supprimer un abonnement, sélectionnez-le dans l’onglet abonnements, puis cliquez sur Supprimer l’abonnement.

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [Modifier un abonnement à une liste dynamique](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [ Définition du paramètre d’administration des abonnements ](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)
