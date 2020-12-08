---
unique-page-id: 45416698
description: Notes de mise à jour - Juillet 20 - Documentation sur le marketing - Documentation du produit
title: Notes de mise à jour - Juillet 20
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---


# Notes de mise à jour : Juillet 20 {#release-notes-july}

Les fonctionnalités suivantes sont incluses dans la version du 20 juillet. Vérifiez la disponibilité des fonctionnalités de votre édition Marketing.

>[!NOTE]
>
>**Disponibilité**
>
>Veuillez noter que, selon votre forfait actuel, les articles dotés d&#39;une étoile ( ![(étoile)](assets/star-yellow.svg)) peuvent nécessiter l&#39;achat d&#39;une valeur ajoutée. Veuillez contacter votre représentant Marketo Engage pour en savoir plus.

***Versions*** trimestrielles Les fonctionnalités suivantes seront publiées le 31 **juillet 2020**.

## Administration {#administration}

* ** [&quot;Utilisé par&quot; Exportation dans la gestion](https://docs.marketo.com/x/hAK1Ag)des champs** : Les administrateurs peuvent désormais exporter tous les liens de ressource &quot;Utilisé par&quot; pour un champ sélectionné dans un fichier CSV. Cette amélioration peut aider les administrateurs et les non-administrateurs à nettoyer les champs inutilisés. En outre, les fichiers peuvent désormais être ouverts dans un nouvel onglet ou une nouvelle fenêtre du navigateur.

**Marketing basé sur le compte ![(étoile)](assets/star-yellow.svg)

**

* **Mise à jour de l’interface utilisateur pour le profilage de compte : **Simplifiez la création de votre liste de compte de cible dans le profilage de compte avec des étapes simplifiées, le tout dans un seul écran.

<br> 

**

***Libération au cours du trimestre***

Les fonctionnalités suivantes sont présentées sur un cycle non trimestriel et seront publiées au cours des prochains mois.

* **Service Forms : **Nous introduisons une validation plus poussée de la syntaxe des champs de formulaire et la possibilité de bloquer les modèles de robots courants avec les nouvelles fonctionnalités de domaines sécurisés pour les Landings page. Le blocage des modèles de robots peut réduire les envois de formulaires de spam et améliorer la qualité de votre base de données.
* **Augmentation de la taille de l’URI de l’API de ressources**: La limite de taille de l&#39;URI (Uniforme Resource Identifier) est augmentée de 8 Ko à 65 Ko avant la suppression du paramètre &quot;_method&quot;. Lorsque vous effectuez de longues chaînes de requête, cette augmentation de taille limite permet aux données de passer plus facilement. La suppression du paramètre &quot;_method&quot; fait partie d&#39;une mise à niveau de sécurité à venir.

**Sales Insight ![(star)](assets/star-yellow.svg)

**

* ** [Sales Insight activé pour les clients avec une intégration](https://docs.marketo.com/x/pQK1Ag)CRM Salesforce non native (bêta)** : Les clients Marketo Engage disposant d&#39;intégrations CRM Salesforce non natives peuvent désormais utiliser Sales Insight pour aider leurs équipes commerciales à comprendre, classer par priorité et interagir avec les pistes et opportunités les plus impliquées afin de permettre des ventes intelligentes et des offres plus rapides.

**Connexion commerciale ![(étoile)](assets/star-yellow.svg)

**

* ** Consentement [amélioré à deux parties pour les appels de vente :](https://docs.marketo.com/x/dgC1Ag)** Les administrateurs ont désormais un meilleur contrôle sur les configurations d&#39;enregistrement des appels. [Activez les enregistrements](https://docs.marketo.com/x/dAC1Ag) d’appels en toute confiance, en vous conformant à la loi sur le consentement des deux parties. Automatisez la notification de l&#39;appel enregistré et activez les clips audio à lire avant l&#39;appel.

<br> 

## Annonces et dépréciations {#announcements-deprecations}

* **Retrait** de paramètre de l&#39;API de ressource &quot;_method&quot; : Après septembre 2020, les points de terminaison de l’API Asset n’accepteront plus &quot;_method&quot; pour transmettre des paramètres de Requête dans un corps de POST afin de contourner les limites de longueur d’URI. Pour répondre aux demandes nécessitant ce paramètre, les limites d’URI pour les API d’actifs seront augmentées de 8 Ko à 65 Ko.
* ** [Munchkin Responsable](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)associé** : Avec cette version du client JavaScript Munchkin, version 159, nous commencerons à déprécier la méthode de piste associée Munchkin. En cas d’appel, vous recevrez un avertissement indiquant que la méthode sera supprimée dans une prochaine version. Une fois supprimée, la méthode ne sera plus fonctionnelle et les tentatives d’utilisation échoueront. Les clients Marketo Engage qui ont récemment utilisé cette méthode seront informés individuellement de leur utilisation.
* **Prise en charge d’Internet Explorer**: Comme annoncé précédemment, la prise en charge par les Marketo Engage d’Internet Explorer 11 prend fin le 31 **juillet 2020**. Nous continuerons à prendre en charge Google Chrome, Mozilla Firefox, Apple Safari et Microsoft Edge.

* **Expérience** par défaut Sky : L’option permettant aux administrateurs ou aux utilisateurs de définir le Marketo Sky comme expérience par défaut sera supprimée dans cette version en vue d’une mise à jour de l’expérience utilisateur Principale. D&#39;autres détails sur la mise à jour de la Principale expérience, prévue pour la fin de l&#39;année, seront disponibles en juillet. Les utilisateurs qui ont défini le Marketo Sky comme expérience par défaut, ou qui ont obtenu l’accès au Marketo Sky, peuvent continuer à accéder au Marketo Sky à partir d’une mosaïque sur la page d&#39;accueil Mon marché.
* **Prise en charge** de Microsoft EdgeHTML (non chrome) : Fin 2020, le Marketo Engage ne prendra plus en charge les versions EdgeHTML de Microsoft Edge. À compter du 1er janvier 2021, nous ne prendrons en charge que la dernière version de Chromium de Microsoft Edge.

