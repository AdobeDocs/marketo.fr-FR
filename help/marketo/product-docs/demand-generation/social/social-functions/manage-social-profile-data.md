---
unique-page-id: 2950578
description: Gérer les données du Profil Social - Documents marketing - Documentation du produit
title: Gérer les données de Profil Social
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---


# Gérer les données de Profil Social {#manage-social-profile-data}

Lorsqu’une personne interagit avec une application [](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)sociale Marketo ou autorise son réseau social à préremplir un formulaire Marketo avec un formulaire [social à remplir](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo capture toutes les données disponibles à partir de son profil social. Vous pouvez vue ces informations sur la page [Détails de la](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)personne ou les ajouter sous la forme d’une colonne dans une vue [personnalisée d’une liste](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List)intelligente.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Le remplissage de formulaires sociaux et les applications sociales capturent des ensembles de champs légèrement différents ; voir la section pour chacun des éléments ci-dessous.

>[!NOTE]
>
>**Disponibilité**
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus de détails.

## Capturée via l’application Social {#captured-via-social-app}

Selon les paramètres de confidentialité du réseau et de l’utilisateur, un ou plusieurs de ces champs sont récupérés :

>[!NOTE]
>
>Les informations supplémentaires provenant des réseaux sociaux s’affichent sur la page Détails sur la personne environ cinq minutes après l’autorisation de la personne.

## Sur Twitter : {#from-twitter}

* Prénom (analysé à partir du nom d’affichage)
* Nom (analysé à partir du nom d’affichage)
* URL de la photo du profil
* URL de la page de profil
* Portée sociale (nombre d&#39;abonnés)

>[!NOTE]
>
>Les applications sociales ne récupèrent pas l’adresse électronique de la personne.

## Sur Facebook : {#from-facebook}

* Prénom
* Nom
* URL du profil
* URL de la photo du profil
* Sexe
* Portée sociale (nombre d’amis)

### Capturé via le remplissage de formulaires sur les réseaux sociaux {#captured-via-social-form-fill}

Selon les paramètres de confidentialité du réseau et de l’utilisateur, un ou plusieurs de ces champs sont récupérés :

>[!CAUTION]
>
>Les données capturées par le remplissage de formulaires sur les réseaux sociaux remplacent les champs correspondants, sauf si vous [bloquez les mises à jour de ces champs au niveau](../../../../product-docs/administration/field-management/block-updates-to-a-field.md)du formulaire.

## Sur Twitter : {#from-twitter-1}

* Prénom (analysé à partir du nom d’affichage)
* Nom (analysé à partir du nom d’affichage)
* Courriel

## Sur Facebook : {#from-facebook-1}

* Prénom
* Nom
* Courriel
* Date de naissance
* Titre de la tâche
* Société

>[!NOTE]
>
>Le remplissage de formulaire Social capture l’adresse électronique *uniquement* si la personne l’entre dans le formulaire. Si vous avez besoin de l’adresse électronique, vous devez [en faire un champ obligatoire dans votre formulaire](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!NOTE]
>
>**Articles connexes**
>
>Pour capturer ces informations à partir de formulaires, activez le remplissage [de formulaires](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)sociaux.

>[!NOTE]
>
>**Plongée profonde**
>
>En savoir plus sur l&#39;utilisation des formulaires dans la plongée en profondeur [Forms](http://docs.marketo.com/display/docs/forms) .

