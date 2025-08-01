---
title: Connecter Experience Manager doc
description: Découvrez comment connecter les services cloud Adobe Experience Manager à Adobe Marketo Engage afin de pouvoir exploiter vos ressources AEM.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Connexion aux services cloud Adobe Experience Manager {#connect-adobe-experience-manager-cloud-services}

Découvrez comment connecter votre compte AEM Assets Cloud Services à votre instance Adobe Marketo Engage afin de pouvoir exploiter votre référentiel de ressources AEM dans Marketo Engage Email Designer.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Dans Marketo Engage, accédez à la zone **Admin** et sélectionnez **Adobe Experience Manager** dans l’arborescence de navigation de gauche.

CAPTURE D’ÉCRAN

1. Cliquez sur **Modifier** en regard de _Services cloud Adobe Experience Manager_.

CAPTURE D’ÉCRAN

1. Sélectionnez un ou plusieurs référentiels.

CAPTURE D’ÉCRAN

>[!NOTE]
>
>Seuls les référentiels qui ont été associés dans la même organisation IMS que votre abonnement Marketo Engage sont répertoriés.

1. Vous devez ajouter un [certificat d’identification de service](https://experienceleague.adobe.com/fr/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) pour configurer le référentiel. Cliquez sur le bouton **+ Ajouter un certificat**.

CAPTURE D’ÉCRAN

1. Effectuez un glisser-déposer de votre certificat (fichier JSON uniquement) ou sélectionnez-le depuis votre ordinateur. Cliquez sur **Ajouter** lorsque vous avez terminé.

CAPTURE D’ÉCRAN

1. Le référentiel configuré est affiché ci-dessous, ainsi que le statut et l’expiration. Cliquez sur le bouton représentant des points de suspension (**...**) pour afficher le certificat. Sinon, c&#39;est fini.

CAPTURE D’ÉCRAN

Désormais, toutes les images de la bibliothèque de gestion des ressources numériques de ce référentiel sont accessibles à partir du Designer de messagerie Marketo Engage.

>[!MORELIKETHIS]
>
>[Utilisation des ressources Experience Manager](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
