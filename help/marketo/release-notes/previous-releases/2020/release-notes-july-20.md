---
unique-page-id: 45416698
description: Notes De Mise À Jour -20 Juillet - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Juillet 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 2%

---

# Notes de mise à jour : juillet 2020 {#release-notes-july}

Les fonctionnalités suivantes sont incluses dans la version du 20 juillet. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo.

>[!AVAILABILITY]
>
>Veuillez noter que, selon votre forfait actuel, les articles avec une étoile ( ![(étoile)](assets/yellow-star.png)) peuvent nécessiter l&#39;achat d&#39;un complément de valeur. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

**_Versions trimestrielles_** Les fonctionnalités suivantes seront publiées le **31 juillet 2020**.

## Administration {#administration}

* **[Exportation « Utilisé par » dans la gestion des champs](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)** : les administrateurs peuvent désormais exporter tous les liens de ressources « Utilisé par » pour un champ sélectionné dans un fichier CSV. Cette amélioration peut aider les administrateurs et les non-administrateurs à nettoyer les champs inutilisés. En outre, les ressources peuvent désormais être ouvertes dans un nouvel onglet ou une nouvelle fenêtre du navigateur.

## Account-Based Marketing {#account-based-marketing}

![(étoile)](assets/yellow-star.png)

* **Mise à jour de l’interface utilisateur pour le profilage de compte** : simplifiez la création de votre liste de comptes cibles dans le profilage de compte avec des étapes rationalisées, le tout sur un seul écran.

<br> 

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes font l’objet d’un cycle non trimestriel et seront publiées au cours des prochains mois.

* **Service Forms** : nous renforçons la validation de la syntaxe des champs de formulaire et la possibilité de bloquer les modèles de robots courants avec les nouvelles fonctionnalités de domaines sécurisés pour les pages de destination. Le blocage des modèles de robots peut réduire les envois de formulaires indésirables et améliorer la qualité de votre base de données.

>[!NOTE]
>
>Le déploiement complet de la validation de la syntaxe de champ de formulaire amélioré a été reporté après notre version de janvier 2021.

* **Limite de taille de l’URI de l’API de ressource augmentée** : la limite de taille de l’URI (Uniform Resource Identifier) est augmentée de 8 Ko à 65 Ko avant la suppression du paramètre « _method ». Lors de l’exécution de chaînes de requête longues, cette augmentation de la limite de taille permettra aux données de passer plus facilement. La suppression du paramètre « _method » fait partie d’une mise à niveau de sécurité à venir.

## [!DNL Sales Insight] {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Activé pour les clients disposant d’une intégration CRM  [!DNL Salesforce]  native](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)** : les clients Marketo Engage disposant d’intégrations CRM [!DNL Salesforce] non natives peuvent désormais utiliser [!DNL Sales Insight] pour aider leurs équipes commerciales à comprendre les prospects et les opportunités les plus engagés, à les classer par priorité et à interagir avec eux, afin de permettre des ventes intelligentes et des offres plus rapides.

## [!DNL Sales Connect] {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **[Consentement bipartite amélioré pour les appels de vente : les administrateurs](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** désormais un meilleur contrôle sur les configurations d’enregistrement des appels. [Activez les enregistrements d’appels](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) en vous assurant que vous vous conformez à la loi sur le consentement bipartite. Automatisez la notification de l&#39;appel en cours d&#39;enregistrement et activez les clips audio à lire avant l&#39;appel.

<br> 

## Annonces et obsolescence {#announcements-deprecations}

* **Suppression du paramètre « _method » de l’API de ressources** : après septembre 2020, les points d’entrée de l’API de ressources n’accepteront plus « _method » pour transmettre des paramètres de requête dans un corps POST afin de contourner les limites de longueur d’URI. Pour répondre aux requêtes qui nécessitaient ce paramètre, les limites d’URI pour les API de ressources passeront de 8 Ko à 65 Ko.
* **[[!DNL Munchkin] Associer le prospect](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** : avec cette version du client Munchkin JavaScript, version 159, nous allons commencer à abandonner la méthode [!DNL Munchkin] Associer le prospect. Si cette option est appelée, vous recevez un avertissement indiquant que la méthode sera supprimée dans une version ultérieure. Une fois supprimée, la méthode ne sera plus fonctionnelle et les tentatives pour l’utiliser échoueront. Les clients Marketo Engage qui ont récemment utilisé cette méthode seront avertis individuellement de leur utilisation.
* **Prise en charge d’Internet Explorer** : comme annoncé précédemment, la prise en charge de Marketo Engage pour Internet Explorer 11 prend fin le **31 juillet 2020**. Nous continuerons d&#39;appuyer [!DNL Google Chrome], [!DNL Mozilla Firefox], [!DNL &#x200B; Apple Safari] et [!DNL Microsoft Edge].
* **Expérience Sky par défaut** : l’option permettant aux administrateurs ou aux utilisateurs de définir [!DNL Marketo Sky] comme expérience par défaut sera supprimée dans cette version en vue d’une mise à jour de l’expérience utilisateur principale. Plus de détails sur la mise à jour de l’expérience principale, prévue pour plus tard dans l’année, seront disponibles en juillet. Les utilisateurs qui ont défini [!DNL Marketo Sky] comme expérience par défaut, ou à qui l’accès à [!DNL Marketo Sky] a été accordé, peuvent continuer à accéder aux [!DNL Marketo Sky] à partir d’une mosaïque de la page d’accueil Mon Marketo.
* **Prise en charge du [!DNL Microsoft Edge] EdgeHTML (autre que Chromium)** : Marketo Engage ne prendra plus en charge les versions EdgeHTML de Microsoft Edge fin 2020. À compter du 1er janvier 2021, nous ne prendrons en charge que la dernière version Chromium de Microsoft Edge.
