---
title: Connecter Experience Manager doc
description: Découvrez comment connecter AEM Cloud Services à Marketo Engage. Utilisez vos ressources AEM lors de la création d’e-mails dans le concepteur.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: 'yes'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: f8f7d99a-f455-45bb-8028-428a55a7130b
    internal-label: Email Designer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 8%
---
# Connexion aux services cloud Adobe Experience Manager {#connect-adobe-experience-manager-cloud-services}

Découvrez comment connecter votre compte AEM Assets Cloud Services à votre instance Adobe Marketo Engage afin de pouvoir exploiter votre référentiel de ressources AEM dans Marketo Engage Email Designer.

>[!NOTE]
>
>**Autorisations d’administration requises**

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

1. Le référentiel configuré est affiché ci-dessous, ainsi que le statut et l’expiration. Cliquez sur le bouton représentant des points de suspension (**...**) pour afficher le certificat. Sinon, vous avez terminé.

CAPTURE D’ÉCRAN

Désormais, toutes les images de la bibliothèque de gestion des ressources numériques de ce référentiel sont accessibles à partir du Designer de messagerie Marketo Engage.

>[!MORELIKETHIS]
>
>[Utilisation des ressources Experience Manager](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
