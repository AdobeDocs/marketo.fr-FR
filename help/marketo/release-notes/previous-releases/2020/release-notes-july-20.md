---
unique-page-id: 45416698
description: Notes de mise à jour - 20 juillet - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Juillet 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 1%

---

# Notes de mise à jour : 20 juillet {#release-notes-july}

Les fonctionnalités suivantes sont incluses dans la version du 20 juillet. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Marketo.

>[!AVAILABILITY]
>
>Notez que, selon votre package actuel, les éléments avec une étoile ( ![(étoile)](assets/yellow-star.png)) peuvent nécessiter l’achat d’un module complémentaire de valeur. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_** Les fonctionnalités suivantes seront publiées le **31 juillet 2020**.

## Administration {#administration}

* **[&quot;Used By&quot; Export dans Field Management](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)** : les administrateurs peuvent désormais exporter tous les liens de ressources &quot;Used by&quot; pour un champ sélectionné dans un fichier CSV. Cette amélioration peut aider les administrateurs et les non-administrateurs à nettoyer les champs inutilisés. En outre, les ressources peuvent désormais être ouvertes dans un nouvel onglet ou une nouvelle fenêtre du navigateur.

## Account-Based Marketing {#account-based-marketing}

![(star)](assets/yellow-star.png)

* **Interface utilisateur mise à jour pour le profilage de compte** : simplifiez la création de votre liste de comptes cible dans le profilage de compte avec des étapes simplifiées toutes en un seul écran.

<br> 

**_Mise à jour tout au long du trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

* **Service Forms** : nous introduisons une validation de la syntaxe des champs de formulaire plus forte et la possibilité de bloquer les modèles de robots courants avec de nouveaux domaines sécurisés pour les pages d’entrée. Le blocage des modèles de robots peut réduire les envois de formulaires indésirables et améliorer la qualité de votre base de données.

>[!NOTE]
>
>Le déploiement complet de la validation améliorée de la syntaxe des champs de formulaire a été reporté après notre version de janvier 2021.

* **Augmentation de la taille de l’URI de l’API de ressource** : la limite de taille de l’URI (Uniform Resource Identifier) est augmentée de 8 Ko à 65 Ko avant la suppression du paramètre &quot;_method&quot;. Lors de l’exécution de longues chaînes de requête, cette augmentation de taille limite permet aux données de passer plus facilement. La suppression du paramètre &quot;_method&quot; fait partie d’une mise à niveau de sécurité à venir.

## Sales Insight {#sales-insight}

![(star)](assets/yellow-star.png)

* **[Sales Insight activé pour les clients avec une intégration CRM Salesforce non native](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)** : les clients Marketo Engage avec des intégrations CRM Salesforce non natives peuvent désormais utiliser Sales Insight pour aider leurs équipes commerciales à comprendre, hiérarchiser et interagir avec les prospects et opportunités les plus engagés afin d’activer des ventes intelligentes et des offres plus rapides.

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **[Consentement bipartite amélioré pour les appels de vente :](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Les administrateurs disposent désormais d’un meilleur contrôle sur les configurations d’enregistrement des appels. [ Activez les enregistrements d’appel ](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) en toute confiance, conformément à la loi sur le consentement bipartite. Automatisez la notification de l’appel en cours d’enregistrement et activez les clips audio à lire avant l’appel.

<br> 

## Annonces et obsolescences {#announcements-deprecations}

* **Retrait de paramètre de l’API de ressource &quot;_method&quot;** : après septembre 2020, les points de terminaison de l’API de ressource n’accepteront plus &quot;_method&quot; pour transmettre les paramètres de requête dans un corps de POST afin de contourner les limitations de longueur d’URI. Pour répondre aux demandes qui nécessitaient ce paramètre, les limites d’URI pour les API de ressources seront augmentées de 8 Ko à 65 Ko.
* **[Plomb associé Munchkin](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** : avec cette version du client Munchkin JavaScript, version 159, nous allons commencer à abandonner la méthode &quot;plomb associé Munchkin&quot;. En cas d’appel, vous recevrez un avertissement indiquant que la méthode sera supprimée dans une version ultérieure. Une fois supprimée, la méthode ne sera plus fonctionnelle et les tentatives d’utilisation échoueront. Les clients Marketo Engage qui ont récemment utilisé cette méthode seront informés individuellement de leur utilisation.
* **Prise en charge d’Internet Explorer** : comme annoncé précédemment, la prise en charge du Marketo Engage pour Internet Explorer 11 se termine le **31 juillet 2020**. Nous continuerons à prendre en charge Google Chrome, Mozilla Firefox, Apple Safari et Microsoft Edge.
* **Expérience par défaut du ciel** : l’option permettant aux administrateurs ou aux utilisateurs de définir Marketo Sky comme expérience par défaut sera supprimée dans cette version en vue d’une mise à jour de l’expérience utilisateur principale. D’autres détails sur la mise à jour de l’expérience principale, prévue plus tard cette année, seront disponibles en juillet. Les utilisateurs qui ont défini Marketo Sky comme expérience par défaut, ou qui ont reçu l’accès à Marketo Sky, peuvent continuer à accéder à Marketo Sky à partir d’une mosaïque de la page d’accueil de My Marketo.
* **Prise en charge de Microsoft Edge EdgeHTML (non Chromium)** : Marketo Engage ne prendra plus en charge les versions EdgeHTML de Microsoft Edge à la fin de 2020. À compter du 1er janvier 2021, nous ne prendrons en charge que la dernière version de Chromium de Microsoft Edge.
