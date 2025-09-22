---
unique-page-id: 11382593
description: Définition du Personalization Web sur Ne pas suivre - Documents Marketo - Documentation du produit
title: Définition de Web Personalization sur Ne pas suivre
exl-id: 9c60cd6b-4244-4472-90fa-4ba9fa9a4f34
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 3%

---

# Définition de [!UICONTROL Web Personalization] sur Ne pas suivre {#setting-web-personalization-to-do-not-track}

Les visiteurs du Web peuvent paramétrer leur navigateur pour empêcher le tracking par n&#39;importe quel site Web, en choisissant « Do Not Track » (DNT). Cela empêche le suivi de ce navigateur et de cet appareil en particulier.

Dans [!UICONTROL Web Personalization] et [!UICONTROL Contenu prédictif], un spécialiste marketing peut définir un bouton pour indiquer s’il faut prendre en charge ou ignorer le paramètre Ne pas suivre (DNT) du navigateur. Le bouton (bascule) des comptes est désactivé par défaut, ce qui signifie que le DNT n’est pas honoré par l’application.

## Activer ou désactiver le bouton (bascule) {#enable-or-disable-the-toggle}

1. Accédez à **[!UICONTROL Paramètres du compte]**.

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. Dans [!UICONTROL Domain] et [!UICONTROL Domain Configuration], sélectionnez **[!UICONTROL On]** pour activer le bouton (bascule) [!UICONTROL Honour DNT].

   ![](assets/two-1.png)

   Lorsque le bouton (bascule) est défini sur [!UICONTROL Activé], Web Personalization respecte et prend en charge le paramètre Ne pas suivre (DNT) du navigateur. Il ne suit aucune activité web et n’exécute aucune campagne ni recommandation de contenu sur votre site web.

   >[!NOTE]
   >
   >Définir le bouton (bascule) sur [!UICONTROL Activé] peut avoir une incidence sur la valeur et les fonctionnalités de Marketo dans des zones spécifiques.

1. Pour désactiver le bouton (bascule) [!UICONTROL Honorer DNT] et ignorer le paramètre Ne pas suivre (DNT) du navigateur, sélectionnez **[!UICONTROL Désactivé]** sous [!UICONTROL Honorer DNT].
