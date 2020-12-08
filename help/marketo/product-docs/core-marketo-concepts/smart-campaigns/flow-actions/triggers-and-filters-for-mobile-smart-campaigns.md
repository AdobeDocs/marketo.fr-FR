---
unique-page-id: 9437991
description: Déclencheurs et Filtres pour les campagnes dynamiques mobiles - Documents marketing - Documentation sur les produits
title: Déclencheurs et Filtres pour les campagnes dynamiques mobiles
translation-type: tm+mt
source-git-commit: 1c4c4c62215550a09125f76fb76017348aba2bdf
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---


# Déclencheurs et Filtres pour les campagnes dynamiques mobiles {#triggers-and-filters-for-mobile-smart-campaigns}

Vous pouvez configurer des déclencheurs et des filtres pour une campagne dynamique d’application mobile.

Pour la plupart des activités, il existe un déclencheur, un filtre et un filtre d’inactivité. Utilisez des filtres d’inactivité pour effectuer le suivi d’une action, telle que le fait d’appuyer sur une notification Push, qui *n’a pas* eu lieu.

* Application mobile installée/installée
* Application mobile ouverte/ouverte
* Avec/avec Activité d&#39;application mobile
* A/possédait une session d’application mobile
* Notification Push mobile sur une pression/pression

Il n&#39;y a que des filtres pour cette activité :

* Notification Push envoyée - filtre et filtre d’inactivité

Recherchez une application **** mobile dans le panneau de droite pour liste de tous les déclencheurs et filtres d’application mobile.

![](assets/image2015-8-12-17-3a25-3a18.png)

## Contraintes {#constraints}

Utilisez des contraintes avec des déclencheurs et des filtres pour trier davantage les données.

![](assets/image2015-8-17-12-3a6-3a33.png)

Tous les déclencheurs et filtres, à l’exception de Notification Push envoyée, contiennent les deux contraintes standard suivantes :

* Type de périphérique : iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, smartphone Android, tablette Android, Inconnu (il s’agit d’une liste prédéfinie)

* Plate-forme - iPhone ou Android

Certains déclencheurs et filtres d’offre imposent des contraintes supplémentaires, telles que :

* Version de l’application - Un moyen de cible aux personnes qui ne disposent pas de la dernière version. Par exemple, si la dernière version de l’application est 2.0, vous pouvez l’utiliser pour rechercher les personnes qui ne le sont pas dans la version 2.0 de l’application.

* Source d&#39;installation - Actuellement, la seule option est l&#39;API.

* Paramètres régionaux : paramètre défini sur le périphérique

* Application mobile : nom de l&#39;application spécifique. Utile pour spécifier si vous en avez plusieurs

* Version de la plate-forme - Version du système d&#39;exploitation

* Durée de session (secondes) - Durée de session lorsque l’application est en premier plan

* Push est activé - **True** signifie que les notifications Push peuvent être envoyées. **Faux** signifie qu&#39;ils ne peuvent pas ; par exemple, la personne peut avoir choisi de ne pas recevoir de notifications Push

## Déclencheurs et Filtres {#triggers-and-filters}

**Avec application mobile**

Utilisez ce filtre pour identifier toutes les personnes qui ont déjà installé votre application. Cette option est disponible uniquement sous la forme d’un filtre.

>[!NOTE]
>
>Le filtre trouvera les installations en cours et les anciennes, car Marketo ne suit pas les désinstallations de l’application.

**Contraintes**: Type de périphérique, plate-forme, application mobile, version de l’application mobile, type de périphérique, source d’installation, Activé pour la diffusion Push et Paramètre régional

![](assets/image2015-8-21-13-3a33-3a54.png)

>[!TIP]
>
>Il est recommandé de spécifier Has Mobile App = true et Is Push Enabled = true, ainsi que le nom de votre application mobile lors de la définition de la liste intelligente de l’expéditeur d’une notification Push.

Application mobile installée/installée

* Application mobile installée - trigger

* Application mobile installée - filtre

* PAS d’application mobile installée - filtre d’inactivité

**Contraintes**: Type de périphérique, plate-forme, version de l’application, langue et source d’installation

![](assets/image2015-8-17-13-3a11-3a3.png)

Application mobile ouverte/ouverte

* Application mobile ouverte - trigger

* Application mobile ouverte - filtre

* PAS d’application mobile ouverte - filtre d’inactivité

**Contraintes**: Type de périphérique et plate-forme

![](assets/image2015-8-17-13-3a13-3a55.png)

Avec/avec Activité d&#39;application mobile

Elles offrent un moyen puissant de suivre l&#39;activité mobile personnalisée. Vous devrez travailler avec votre développeur pour configurer le suivi [pour Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android) et [pour iOS](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios).

* Avec Activité d’application mobile - trigger

* Activité d’application mobile - filtre

* ACTIVITÉ d’application mobile NON présente - filtre d’inactivité

**Contraintes**: Type de périphérique et plate-forme, plus cinq autres :

* Action - activité mobile personnalisée

* Type d’action - Champ de texte (facultatif) utilisé pour classer plusieurs actions par catégorie

* Détails de l’action - Champ de texte (facultatif) qui fournit des informations supplémentaires sur une action

* Mesure d’action - (facultatif) champ numérique qui fournit des informations supplémentaires sur une action (par exemple, le prix)

* Longueur d’action (secondes) - (facultatif) champ numérique pouvant être utilisé pour capturer le temps nécessaire à un utilisateur pour terminer une action

Les contraintes Action vous permettent d’utiliser le déclencheur et les filtres pour suivre l’activité mobile de très près.

>[!NOTE]
>
>**Exemple**
>
>Sous le type d&#39;action *Shopping*, voici une action très spécifique, avec les autres contraintes qui la définissent :
>
>* Achat d&#39;une chemise
>  * C&#39;était rouge.
>  * Ça a coûté 30 dollars.
>  * Il a fallu 20 secondes pour acheter


Voici à quoi ressemble le filtre dans Marketo :   ![](assets/image2015-8-17-13-3a16-3a12.png)

>[!NOTE]
>
>**Exemple**
>
>Vous pouvez avoir plusieurs actions sous le même type d’action. En fait, votre expérience d&#39;achat normale peut impliquer plusieurs colonnes sous Shopping ! Et des chaussettes pour ça ?
>
>| Type d&#39;action | Shopping | Shopping |
>|---|---|---|
>| Action | Chemise achetée | Pantalon acheté |
>| Détails de l&#39;action | Couleur | Couleur |
>| Mesure d’action | Prix | Prix |


**A/possédait une session d’application mobile**

* Comporte une session d’application mobile - trigger

* Session d’application mobile - filtre

* Session d’application mobile NON présente - filtre d’inactivité

**Contraintes**: Type de périphérique, plate-forme et durée de session (secondes)

![](assets/image2015-8-17-13-3a18-3a34.png)

Notification Push avec appui/appui sur une touche

* Notification Push sur pression - trigger

* Notification Push avec activation - filtre

* Notification Push NON activée - filtre d’inactivité

**Contraintes**: Type de périphérique, plate-forme, version de l’application mobile, notification Push et version de la plate-forme

![](assets/image2015-8-21-14-3a2-3a24.png)

>[!TIP]
>
>Utilisez le filtre d’inactivité Notification Push non activée pour rechercher les personnes qui n’ont pas appuyé sur une notification Push récemment envoyée, afin que vous puissiez effectuer un suivi par courrier électronique.

**Notification** Push envoyée Cette activité n&#39;est disponible qu&#39;en tant que filtre.

* Notification Push envoyée - filtre

* Notification Push NON envoyée - filtre d&#39;inactivité

**Contraintes**: Notification Push et application mobile

![](assets/image2015-8-21-14-3a3-3a50.png)

>[!NOTE]
>
>**Articles connexes**
>
>* [Ajouter une contrainte à un filtre de Liste dynamique](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)
>* [Utiliser les Filtres d&#39;inactivité dans une Liste dynamique](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

