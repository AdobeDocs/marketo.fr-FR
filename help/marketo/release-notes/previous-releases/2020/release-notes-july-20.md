---
unique-page-id: 45416698
description: Notes de mise à jour - 20 juillet - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Juillet 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 1%

---

# Notes de mise à jour : 20 juillet {#release-notes-july}

Les fonctionnalités suivantes sont incluses dans la version du 20 juillet. Vérifiez la disponibilité de votre édition Marketo.

>[!AVAILABILITY]
>
>Notez que, selon votre package actuel, les éléments avec une étoile ( ![(étoile)](assets/yellow-star.png)) peut nécessiter l’achat d’un module complémentaire de valeur. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_** Les fonctionnalités suivantes seront publiées sur **31 juillet 2020**.

## Administration {#administration}

* **[Exportation &quot;utilisée par&quot; dans la gestion des champs](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: Les administrateurs peuvent désormais exporter tous les liens de ressources &quot;Utilisé par&quot; pour un champ sélectionné dans un fichier CSV. Cette amélioration peut aider les administrateurs et les non-administrateurs à nettoyer les champs inutilisés. En outre, les ressources peuvent désormais être ouvertes dans un nouvel onglet ou une nouvelle fenêtre du navigateur.

## Account-Based Marketing {#account-based-marketing}

![(étoile)](assets/yellow-star.png)

* **Mise à jour de l’interface utilisateur pour le profilage de compte**: Simplifiez la création de votre liste de comptes cible dans le Profilage de compte avec des étapes simplifiées, le tout sur un seul écran.

<br> 

**_Sortie pendant tout le trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

* **Forms Service**: Nous proposons une validation plus poussée de la syntaxe des champs de formulaire et la possibilité de bloquer les modèles de robots courants avec de nouvelles fonctionnalités Domaines sécurisés pour les landing pages. Le blocage des modèles de robots peut réduire les envois de formulaires indésirables et améliorer la qualité de votre base de données.

>[!NOTE]
>
>Le déploiement complet de la validation améliorée de la syntaxe des champs de formulaire a été reporté après notre version de janvier 2021.

* **Augmentation de la taille de l’URI de l’API de ressource**: La limite de taille de l’URI (Uniform Resource Identifier) est augmentée de 8 Ko à 65 Ko avant la suppression du paramètre &quot;_method&quot;. Lors de l’exécution de longues chaînes de requête, cette augmentation de taille limite permet aux données de passer plus facilement. La suppression du paramètre &quot;_method&quot; fait partie d’une mise à niveau de sécurité à venir.

## Sales Insight {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **[Sales Insight activé pour les clients avec une intégration CRM Salesforce non native](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Version bêta)**: Les clients Marketo Engage disposant d’intégrations CRM Salesforce non natives peuvent désormais utiliser Sales Insight pour aider leurs équipes commerciales à comprendre, à hiérarchiser et à interagir avec les prospects et opportunités les plus engagés afin de permettre des ventes intelligentes et des offres plus rapides.

## SalesConnect {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **[Amélioration du consentement bipartite pour les appels de vente :](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Les administrateurs disposent désormais d’un meilleur contrôle sur les configurations d’enregistrement des appels. [Activation des enregistrements d’appel](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) en toute confiance que vous vous conformez à la loi sur le consentement des deux parties. Automatisez la notification de l’appel en cours d’enregistrement et activez les clips audio à lire avant l’appel.

<br> 

## Annonces et obsolescences {#announcements-deprecations}

* **Suppression de paramètres de l’API de ressource &quot;_method&quot;**: Après septembre 2020, les points de terminaison de l’API Asset n’accepteront plus &quot;_method&quot; pour transmettre les paramètres de requête dans un corps de POST afin de contourner les limitations de longueur d’URI. Pour répondre aux demandes qui nécessitaient ce paramètre, les limites d’URI pour les API de ressources seront augmentées de 8 Ko à 65 Ko.
* **[Munchkin, plomb associé](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: Avec cette version du client JavaScript Munchkin, version 159, nous allons commencer à abandonner la méthode &quot;Munchkin Associate Lead&quot;. En cas d’appel, vous recevrez un avertissement indiquant que la méthode sera supprimée dans une version ultérieure. Une fois supprimée, la méthode ne sera plus fonctionnelle et les tentatives d’utilisation échoueront. Les clients Marketo Engage qui ont récemment utilisé cette méthode seront informés individuellement de leur utilisation.
* **Prise en charge d’Internet Explorer**: Comme annoncé précédemment, la prise en charge du Marketo Engage pour Internet Explorer 11 prend fin le **31 juillet 2020**. Nous continuerons à prendre en charge Google Chrome, Mozilla Firefox, Apple Safari et Microsoft Edge.
* **Expérience par défaut du ciel**: L’option permettant aux administrateurs ou aux utilisateurs de définir Marketo Sky comme expérience par défaut sera supprimée dans cette version en vue d’une mise à jour de la Principale expérience utilisateur. D’autres détails sur la mise à jour de la Principale expérience, prévue plus tard cette année, seront disponibles en juillet. Les utilisateurs qui ont défini Marketo Sky comme expérience par défaut, ou qui ont reçu l’accès à Marketo Sky, peuvent continuer à accéder à Marketo Sky à partir d’une mosaïque de la page d’accueil de My Marketo.
* **Prise en charge d’EdgeHTML (non Chromium) Microsoft Edge**: Marketo Engage ne prendra plus en charge les versions EdgeHTML de Microsoft Edge à la fin de 2020. À compter du 1er janvier 2021, nous ne prendrons en charge que la dernière version de Chromium de Microsoft Edge.
