---
description: Découvrez l’expiration des ressources locales dans les programmes. Défini lorsque les ressources locales d’un programme expirent et sont supprimées.
title: Expiration des ressources locales
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
feature: Programs
TQID: https://experienceleague.adobe.com/3mXajdQYczhGSxbqPw8UdoavzeHL1ABekMZSiAdaNyQ
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 277
ht-degree: 3%

---

# Expiration des ressources locales {#local-asset-expiration}

Définissez une date/heure d’expiration pour dépublier des pages de destination, désactiver les campagnes de déclenchement ou arrêter les campagnes par lots récurrentes.

## Octroyer l’autorisation d’expiration des ressources de planification {#grant-schedule-asset-expiration-permission}

Avant de pouvoir planifier l’expiration d’une ressource, votre rôle Marketo doit disposer de l’autorisation appropriée activée.

>[!NOTE]
>
>**Autorisations d’administration requises**

1. Dans la zone [!UICONTROL Admin], cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/local-asset-expiration-1.png)

1. Cliquez sur l’onglet **[!UICONTROL Rôles]**, sélectionnez l’utilisateur auquel vous souhaitez accorder l’accès, puis cliquez sur **[!UICONTROL Modifier le rôle]**.

   ![](assets/local-asset-expiration-2.png)

1. Sous [!UICONTROL Accéder aux activités marketing], sélectionnez **[!UICONTROL Planifier l’expiration locale des ressources]** et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/local-asset-expiration-3.png)

## Définir une date d’expiration {#set-an-expiration-date}

1. Faites un clic droit sur le programme souhaité et sélectionnez **[!UICONTROL Définir l’expiration de la ressource locale]**.

   ![](assets/local-asset-expiration-4.png)

1. Cochez la ressource pour laquelle vous souhaitez définir une date d’expiration, puis cliquez sur **[!UICONTROL Définir l’expiration]**.

   ![](assets/local-asset-expiration-5.png)

1. Choisissez une date d’expiration.

   ![](assets/local-asset-expiration-6.png)

1. Définissez une heure. Vous devez planifier une heure au moins 15 minutes à l’avenir (pensez à entrer matin/après-midi). Cliquez sur **[!UICONTROL Confirmer]** lorsque vous avez terminé.

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* Pour modifier une date d’expiration existante, vérifiez simplement la ou les ressources, puis cliquez sur **[!UICONTROL Définir l’expiration]**.
>* Une fois qu’une ressource a expiré, elle ne s’affiche plus dans la grille d’expiration. La grille affiche uniquement les pages de destination publiées, les campagnes de déclenchement actives et les campagnes par lots récurrentes.
>* Les expirations planifiées seront supprimées si la ressource est déplacée vers un autre programme.

## Supprimer une date d’expiration {#remove-an-expiration-date}

1. Pour supprimer une date d’expiration, vérifiez la ou les ressources, puis cliquez sur **[!UICONTROL Supprimer l’expiration]**.

   ![](assets/local-asset-expiration-8.png)

1. Vérifiez les ressources affectées, puis cliquez sur **[!UICONTROL Confirmer]**.

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>Les dates d’expiration postérieures à 15 minutes ne peuvent pas être supprimées. Pour « supprimer » l’expiration, vous devez attendre qu’elle arrive à expiration, puis la réapprouver ou la réactiver.
