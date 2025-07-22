---
description: Expiration Des Ressources Locales - Documents Marketo - Documentation Du Produit
title: Expiration des ressources locales
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
feature: Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Expiration des ressources locales {#local-asset-expiration}

Définissez une date/heure d’expiration pour dépublier des pages de destination, désactiver les campagnes de déclenchement ou arrêter les campagnes par lots récurrentes.

## Octroyer l’autorisation d’expiration des ressources de planification {#grant-schedule-asset-expiration-permission}

Avant de pouvoir planifier l’expiration d’une ressource, votre rôle Marketo doit disposer de l’autorisation appropriée activée.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Dans la zone [!UICONTROL Admin], cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/local-asset-expiration-1.png)

1. Cliquez sur l’onglet **[!UICONTROL Rôles]**, sélectionnez l’utilisateur auquel vous souhaitez accorder l’accès, puis cliquez sur **[!UICONTROL Modifier le rôle]**.

   ![](assets/local-asset-expiration-2.png)

1. Sous [!UICONTROL Accéder aux activités marketing], sélectionnez **[!UICONTROL Planifier l’expiration locale des ressources]** et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/local-asset-expiration-3.png)

## Définir une date d’expiration {#set-an-expiration-date}

1. Faites un clic droit sur le programme souhaité et sélectionnez **[!UICONTROL Définir l’expiration de la ressource locale]**.

   ![](assets/local-asset-expiration-4.png)

1. Vérifiez la ou les ressources pour lesquelles vous souhaitez définir une date d’expiration, puis cliquez sur **[!UICONTROL Définir l’expiration]**.

   ![](assets/local-asset-expiration-5.png)

1. Choisissez une date d’expiration.

   ![](assets/local-asset-expiration-6.png)

1. Définissez une heure. Vous devez planifier une heure au moins 15 minutes à l&#39;avenir (n&#39;oubliez pas d&#39;entrer AM/PM). Cliquez sur **[!UICONTROL Confirmer]** lorsque vous avez terminé.

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
