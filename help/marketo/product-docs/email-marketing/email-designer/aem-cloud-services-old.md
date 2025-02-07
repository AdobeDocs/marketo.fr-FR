---
title: Connecter un document Experience Manager
description: Découvrez comment connecter les Cloud Service Adobe Experience Manager à Adobe Marketo Engage afin de pouvoir exploiter vos ressources AEM.
hide: true
hidefromtoc: true
source-git-commit: 3a3c3dae689760b720c4823bc1d11bf39da998fe
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Connexion aux Cloud Service Adobe Experience Manager {#connect-adobe-experience-manager-cloud-services}

Découvrez comment connecter votre compte AEM Assets Cloud Service à votre instance Adobe Marketo Engage afin de pouvoir exploiter votre référentiel de ressources AEM dans Marketo Engage Email Designer.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Dans Marketo Engage, accédez à la zone **Admin** et sélectionnez **Adobe Experience Manager** dans l’arborescence de navigation de gauche.

CAPTURE D’ÉCRAN

1. Cliquez sur **Modifier** en regard de _Cloud Service Adobe Experience Manager_.

CAPTURE D’ÉCRAN

1. Sélectionnez un ou plusieurs référentiels.

CAPTURE D’ÉCRAN

>[!NOTE]
>
>Seuls les référentiels qui ont été associés à la même organisation IMS que votre abonnement de Marketo Engage sont répertoriés.

1. Vous devez ajouter un [certificat d’identification de service](https://experienceleague.adobe.com/fr/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) pour configurer le référentiel. Cliquez sur le bouton **+ Ajouter un certificat**.

CAPTURE D’ÉCRAN

1. Effectuez un glisser-déposer de votre certificat (fichier JSON uniquement) ou sélectionnez-le depuis votre ordinateur. Cliquez sur **Ajouter** lorsque vous avez terminé.

CAPTURE D’ÉCRAN

1. Le référentiel configuré est affiché ci-dessous, ainsi que le statut et l’expiration. Cliquez sur le bouton représentant des points de suspension (**...**) pour afficher le certificat. Sinon, c&#39;est fini.

CAPTURE D’ÉCRAN

Désormais, toutes les images de la bibliothèque de gestion des ressources numériques de ce référentiel sont accessibles à partir du Designer d’e-mail du Marketo Engage.

>[!MORELIKETHIS]
>
>[Utilisation de ressources Experience Manager ](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
