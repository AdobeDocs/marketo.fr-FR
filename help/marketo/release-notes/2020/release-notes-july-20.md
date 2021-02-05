---
unique-page-id: 45416698
description: Notes de mise à jour - Juillet 20 - Documentation sur le marketing - Documentation du produit
title: Notes de mise à jour - Juillet 20
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---


# Notes de mise à jour : 20 juillet {#release-notes-july}

Les fonctionnalités suivantes sont incluses dans la version du 20 juillet. Vérifiez la disponibilité des fonctionnalités de votre édition Marketing.

>[!AVAILABILITY]
>
>
>Veuillez noter que, selon votre paquet actuel, les articles avec une étoile ( ![(star)](assets/star-yellow.svg)) peuvent nécessiter l&#39;achat d&#39;un module complémentaire de valeur. Veuillez contacter votre représentant Marketo Engage pour en savoir plus.

****** Versions trimestriellesLes fonctionnalités suivantes seront publiées le 31  **juillet 2020**.

## Administration {#administration}

* ** [&quot;Utilisé par&quot; Export in Field Management](https://docs.marketo.com/x/hAK1Ag)** : Les administrateurs peuvent désormais exporter tous les liens de ressource &quot;Utilisé par&quot; pour un champ sélectionné dans un fichier CSV. Cette amélioration peut aider les administrateurs et les non-administrateurs à nettoyer les champs inutilisés. En outre, les fichiers peuvent désormais être ouverts dans un nouvel onglet ou une nouvelle fenêtre du navigateur.

**Marketing basé sur le compte ![(star)](assets/star-yellow.svg)

**

* **Mise à jour de l’interface utilisateur pour le profilage de compte : **Simplifiez la création de votre liste de compte de cible dans le profilage de compte avec des étapes simplifiées, le tout dans un seul écran.

<br> 

**

***Libération au cours du trimestre***

Les fonctionnalités suivantes sont présentées sur un cycle non trimestriel et seront publiées au cours des prochains mois.

* **Service Forms : **Nous introduisons une validation plus poussée de la syntaxe des champs de formulaire et la possibilité de bloquer les modèles de robots courants avec les nouvelles fonctionnalités de domaines sécurisés pour les Landings page. Le blocage des modèles de robots peut réduire les envois de formulaires de spam et améliorer la qualité de votre base de données.
* **Augmentation de la taille de l’URI de l’API de ressources** : La limite de taille de l&#39;URI (Uniforme Resource Identifier) est augmentée de 8 Ko à 65 Ko avant la suppression du paramètre &quot;_method&quot;. Lorsque vous effectuez de longues chaînes de requête, cette augmentation de taille limite permet aux données de passer plus facilement. La suppression du paramètre &quot;_method&quot; fait partie d&#39;une mise à niveau de sécurité à venir.

**Sales Insight ![(star)](assets/star-yellow.svg)

**

* ** [Sales Insight activé pour les clients avec une intégration CRM Salesforce non native](https://docs.marketo.com/x/pQK1Ag)(bêta)** : Les clients Marketo Engage disposant d&#39;intégrations CRM Salesforce non natives peuvent désormais utiliser Sales Insight pour aider leurs équipes commerciales à comprendre, classer par priorité et interagir avec les pistes et opportunités les plus impliquées afin de permettre des ventes intelligentes et des offres plus rapides.

**Connexion commerciale ![(star)](assets/star-yellow.svg)

**

* ** [Consentement bipartite amélioré pour les appels de vente : ](https://docs.marketo.com/x/dgC1Ag)** Les administrateurs ont désormais un meilleur contrôle sur les configurations d&#39;enregistrement des appels. [Activez les ](https://docs.marketo.com/x/dAC1Ag) enregistrements d’appels en veillant à respecter la loi sur le consentement des deux parties. Automatisez la notification de l&#39;appel enregistré et activez les clips audio à lire avant l&#39;appel.

<br> 

## Annonces et obsolescences {#announcements-deprecations}

* **Retrait** de paramètre de l&#39;API de ressource &quot;_method&quot; : Après septembre 2020, les points de terminaison de l’API Asset n’accepteront plus &quot;_method&quot; pour transmettre des paramètres de Requête dans un corps de POST afin de contourner les limites de longueur d’URI. Pour répondre aux demandes nécessitant ce paramètre, les limites d’URI pour les API d’actifs seront augmentées de 8 Ko à 65 Ko.
* ** [Munchkin Associé Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** : Avec cette version du client JavaScript Munchkin, version 159, nous commencerons à déprécier la méthode de piste associée Munchkin. En cas d’appel, vous recevrez un avertissement indiquant que la méthode sera supprimée dans une prochaine version. Une fois supprimée, la méthode ne sera plus fonctionnelle et les tentatives d’utilisation échoueront. Les clients Marketo Engage qui ont récemment utilisé cette méthode seront informés individuellement de leur utilisation.
* **Prise en charge d’Internet Explorer** : Comme annoncé précédemment, la prise en charge par les Marketo Engage d’Internet Explorer 11 prend fin le 31  **juillet 2020**. Nous continuerons à prendre en charge Google Chrome, Mozilla Firefox, Apple Safari et Microsoft Edge.

* **Expérience** par défaut Sky : L’option permettant aux administrateurs ou aux utilisateurs de définir le Marketo Sky comme expérience par défaut sera supprimée dans cette version en vue d’une mise à jour de l’expérience utilisateur Principale. D&#39;autres détails sur la mise à jour de la Principale expérience, prévue pour la fin de l&#39;année, seront disponibles en juillet. Les utilisateurs qui ont défini le Marketo Sky comme expérience par défaut, ou qui ont obtenu l’accès au Marketo Sky, peuvent continuer à accéder au Marketo Sky à partir d’une mosaïque sur la page d&#39;accueil Mon marché.
* **Prise en charge** de Microsoft EdgeHTML (non chrome) : Fin 2020, le Marketo Engage ne prendra plus en charge les versions EdgeHTML de Microsoft Edge. À compter du 1er janvier 2021, nous ne prendrons en charge que la dernière version de Chromium de Microsoft Edge.

