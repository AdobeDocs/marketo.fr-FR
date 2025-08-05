---
unique-page-id: 9437991
description: Triggers et filtres pour les campagnes intelligentes mobiles - Documents Marketo - Documentation du produit
title: Déclencheurs et filtres pour les campagnes intelligentes mobiles
exl-id: 76fc7a74-b27d-4898-a8ca-85c9c2828a28
feature: Smart Campaigns
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 1%

---

# Déclencheurs et filtres pour les campagnes intelligentes mobiles {#triggers-and-filters-for-mobile-smart-campaigns}

Vous pouvez configurer des déclencheurs et des filtres pour une campagne dynamique sur les applications mobiles.

Pour la plupart des activités, il existe un déclencheur, un filtre et un filtre d’inactivité. Utilisez les filtres d’inactivité pour suivre une action qui ne s’est _produite, comme appuyer sur une notification push_ par exemple.

* L’Application Mobile Est/A Été Installée
* L&#39;Application Mobile Est/A Été Ouverte
* A/A Eu Une Activité D’Application Mobile
* A/A Eu Une Session D’Application Mobile
* Appuyez/Appuyez sur Notification Push Mobile

Il n’existe que des filtres pour cette activité :

* Une notification push a été envoyée - filtre et filtre d’inactivité

Recherchez « application mobile » dans le panneau de droite pour répertorier tous les déclencheurs et filtres d’application mobile.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-1.png)

## Contraintes {#constraints}

Utilisez des contraintes avec des déclencheurs et des filtres pour trier davantage les données.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-2.png)

Tous les déclencheurs et filtres, à l’exception de la notification push A été envoyée, contiennent les deux contraintes standard suivantes :

* Type d’appareil : [!DNL iPod], iPhone, [!DNL iPhone 6 Plus], [!DNL iPad mini], iPad, smartphone Android, tablette Android, inconnu (il s’agit d’une liste prédéfinie).

* Platform - iPhone ou Android

Certains déclencheurs et filtres offrent des contraintes supplémentaires, telles que :

* Version de l’application - Un moyen de cibler les personnes qui ne disposent pas de la dernière version. Par exemple, si la dernière version de l’application est la version 2.0, vous pouvez l’utiliser pour rechercher des personnes qui ne figurent PAS dans la version 2.0 de l’application

* Installer Source - Actuellement, la seule option est l’API

* Paramètre régional - Paramètre sur l’appareil

* Application mobile : nom d’une application spécifique. Utile pour indiquer si vous en avez plusieurs

* Version de la plateforme : version du système d’exploitation.

* Durée de la session (secondes) - Durée de la session pendant laquelle l’application est au premier plan

* Est activé pour les notifications push : **True** signifie que les notifications push peuvent être envoyées. **False** signifie qu’elle ne peut pas ; par exemple, la personne peut avoir choisi de ne pas recevoir de notifications push

## Déclencheurs et filtres {#triggers-and-filters}

**A une application mobile**

Utilisez ce filtre pour identifier toutes les personnes qui ont déjà installé votre application. Cette option n’est disponible qu’en tant que filtre.

>[!NOTE]
>
>Le filtre trouvera les installations actuelles et antérieures, car Marketo ne suit pas les désinstallations de l’application.

**Constraints** - Type d’appareil, plateforme, application mobile, version de l’application mobile, type d’appareil, installation de Source, est activé pour les notifications push et paramètres régionaux

![](assets/triggers-and-filters-for-mobile-smart-campaigns-3.png)

>[!TIP]
>
>Il est recommandé de spécifier A une application mobile = true et Est activé pour les notifications push = true, ainsi que le nom de votre application mobile lors de la définition de la liste dynamique des personnes qui doivent recevoir une notification push.

L’Application Mobile Est/A Été Installée

* L’application mobile est installée - trigger

* L’application mobile a été installée - filtre

* L’application mobile n’a PAS été installée - filtre d’inactivité

**Constraints** - Type d’appareil, plateforme, version d’application, paramètre régional et installation de Source

![](assets/triggers-and-filters-for-mobile-smart-campaigns-4.png)

L&#39;Application Mobile Est/A Été Ouverte

* L’application mobile est ouverte - déclencheur

* L’application mobile a été ouverte - filtre

* L’application mobile n’a PAS été ouverte - filtre d’inactivité

**Contraintes** - Type d’appareil et plateforme

![](assets/triggers-and-filters-for-mobile-smart-campaigns-5.png)

A/A Eu Une Activité D’Application Mobile

Ils offrent un moyen puissant de suivre l’activité mobile personnalisée. Vous devrez travailler avec votre développeur pour configurer le suivi [pour Android](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android){target="_blank"} et [pour iOS](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios){target="_blank"}.

* A une activité d’application mobile - déclencheur

* Avait une activité d’application mobile - filtre

* N’avait PAS d’activité d’application mobile - filtre d’inactivité

**Constraints** - Type d’appareil, plateforme, version de l’application mobile, paramètre régional, version de la plateforme, ainsi que cinq autres contraintes :

* Action - Activité mobile personnalisée

* Type d’action - (facultatif) Champ de texte utilisé pour classer plusieurs actions

* Détails de l’action - (facultatif) Champ de texte qui fournit des informations supplémentaires sur une action

* Mesure d’action - (facultatif) Champ numérique qui fournit des informations supplémentaires sur une action (par exemple, le prix)

* Durée de l’action (secondes) - (facultatif) champ numérique qui peut être utilisé pour capturer la durée nécessaire à un utilisateur ou une utilisatrice pour exécuter une action

Les contraintes d’action vous permettent d’utiliser le déclencheur et les filtres pour suivre de très près l’activité mobile.

>[!NOTE]
>
>**Exemple**
>
>Sous le type d’action _Shopping_, voici une action très spécifique, définie par les autres contraintes :
>
>* J&#39;ai acheté une chemise
>   * C&#39;était rouge
>   * Ça a coûté 30 $
>   * 20 secondes pour acheter

Voici à quoi ressemble le filtre dans Marketo :

![](assets/triggers-and-filters-for-mobile-smart-campaigns-6.png)

>[!NOTE]
>
>**Exemple**
>
>Plusieurs actions peuvent être associées au même type d’action. En fait, votre expérience d’achat normale peut comporter plusieurs colonnes sous Achats ! Que diriez-vous de chaussettes avec ça ?
>
>| Type d’action | Shopping | Shopping |
>|---|---|---|
>| Action | Chemise achetée | Pantalon acheté |
>| Détails de l’action | Couleur | Couleur |
>| Mesure de l’action | Prix | Prix |

**A/A Eu Une Session D’Application Mobile**

* A une session d’application mobile - déclencheur

* Session d’application mobile terminée - filtre

* N’a PAS eu de session d’application mobile - filtre d’inactivité

**Contraintes** - Type d’appareil, plateforme et durée de session (secondes)

![](assets/triggers-and-filters-for-mobile-smart-campaigns-7.png)

Appuyez/Appuyez sur Notification Push

* Appuyez sur Notification push - déclencheur

* Notification push avec bouton - filtre

* Notification push non activée - filtre d’inactivité

**Constraints** - Type d’appareil, plateforme, version d’application mobile, notification push et version de plateforme

![](assets/triggers-and-filters-for-mobile-smart-campaigns-8.png)

>[!TIP]
>
>Utilisez le filtre d&#39;inactivité Notification push non activée pour rechercher les personnes qui n&#39;ont pas appuyé sur une notification push qui leur a été récemment envoyée, afin que vous puissiez effectuer un suivi par e-mail.

**Notification push envoyée** Cette activité est disponible uniquement en tant que filtre.

* Une notification push a été envoyée - filtre

* Aucune notification push n’a été envoyée - filtre d’inactivité

**Constraints** - Notification push et application mobile

![](assets/triggers-and-filters-for-mobile-smart-campaigns-9.png)

>[!MORELIKETHIS]
>
>* [Ajouter une contrainte à un filtre de liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}
>* [Utilisation des filtres d’inactivité dans une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
