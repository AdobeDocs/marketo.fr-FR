---
unique-page-id: 7505310
description: S’abonner à une liste dynamique - Documents Marketo - Documentation du produit
title: S’abonner à une liste intelligente
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 2%

---

# S’abonner à une liste intelligente {#subscribe-to-a-smart-list}

L’abonnement aux listes intelligentes est un excellent moyen de suivre les personnes, avec des rapports envoyés directement dans votre boîte de réception.

Vous pouvez créer un abonnement à une liste dynamique à deux endroits distincts :

* [!UICONTROL Activités marketing]
* [!UICONTROL &#x200B; Base de données &#x200B;]

Les abonnements utilisent la liste complète des personnes au moment où l’abonnement s’exécute.

Les abonnements se trouvent là où réside votre liste dynamique, dans [!UICONTROL Activités marketing] ou [!UICONTROL Base de données].

Vous pouvez créer plusieurs abonnements à partir de la même liste dynamique.

Les abonnements sont spécifiques à l’espace de travail. Par exemple, cette liste d’abonnements se trouve dans un espace de travail différent de ceux affichés dans le reste de cet article :

![](assets/one.png)

>[!NOTE]
>
>Vous êtes limité à 100 abonnements et à un maximum de 100 000 personnes par abonnement, sur les espaces de travail, par instance de Marketo. Si la liste dynamique contient plus de 100 000 noms, Marketo exécutera l’abonnement pour les 100 000 premiers.

## Créer un abonnement à une liste dynamique {#create-a-smart-list-subscription}

1. Accédez à la **[!UICONTROL Base de données]** ou **[!UICONTROL Activités marketing]**.

   ![](assets/db.png)

1. Sélectionnez la liste dynamique pour laquelle vous souhaitez créer un abonnement. Cliquez sur **[!UICONTROL Liste des actions]** et sélectionnez **[!UICONTROL Nouvel abonnement à la liste dynamique]**.

   ![](assets/three.png)

1. Attribuez un **[!UICONTROL Nom]** à votre abonnement, puis sélectionnez ou saisissez les adresses e-mail des **[!UICONTROL Destinataires]**.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. Cliquez sur la liste **[!UICONTROL Fréquence]** et sélectionnez une fréquence.

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. Définissez la date de **[!UICONTROL Fin de la diffusion]**. Vous pouvez sélectionner **[!UICONTROL Jamais]** ou une date de calendrier.

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. Cliquez sur **[!UICONTROL Format]** et effectuez votre choix dans la liste.

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. Cliquez sur **[!UICONTROL Créer]**.

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. Votre nouvel abonnement à la liste dynamique s’affiche en haut de la liste dans l’onglet Abonnements . Cliquez sur **[!UICONTROL Envoyer]** si vous souhaitez effectuer l’envoi maintenant, sans attendre la diffusion e-mail planifiée.

   ![](assets/eight.png)

1. Nous vous recommandons de décocher la case **[!UICONTROL Actif]** pour désactiver l’abonnement à une liste dynamique si personne n’y est abonné.

   ![](assets/nine.png)

   C&#39;était facile, non ?

## E-mail {#email-message}

Les destinataires recevront un e-mail contenant une option pour télécharger le rapport, ainsi qu’un lien direct vers la liste dans l’instance Marketo. Le lien de téléchargement expire dans quatre jours.

>[!NOTE]
>
>Si le paramètre [Secure Subscription Admin](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) est défini sur **[!UICONTROL Oui]**, seules les personnes ayant accès à l’instance Marketo pourront télécharger le rapport.

![](assets/image2015-4-17-15-3a46-3a47.png)

Si un rapport contient 0 personne, les destinataires recevront toujours un e-mail. Cependant, l’e-mail indique simplement qu’il n’y a personne à signaler.

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>Lorsque vous modifiez un filtre de liste dynamique sur lequel vous avez basé un abonnement, il met également à jour le rapport.

L’e-mail fournit également des informations supplémentaires sur les filtres utilisés pour créer la liste.

## Supprimer un abonnement {#delete-a-subscription}

Pour supprimer un abonnement, sélectionnez-le dans l’onglet abonnements et cliquez sur **[!UICONTROL Supprimer l’abonnement]**.

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [Modifier un abonnement à une liste dynamique](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [Sécuriser le paramètre d’administration des abonnements](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)
