---
unique-page-id: 2950578
description: Gérer les données du Profil Social - Documents marketing - Documentation du produit
title: Gérer les données de Profil Social
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# Gérer les données du Profil social {#manage-social-profile-data}

Lorsqu’un utilisateur interagit avec une [application sociale](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) de Marketo ou autorise son réseau social à préremplir un formulaire Marketo avec [remplissage de formulaire social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo capture toutes les données disponibles à partir de son profil social. Vous pouvez vue ces informations sur la [page Détails sur la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) ou les ajouter sous forme de colonne dans une [vue personnalisée d&#39;une liste intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

Le remplissage de formulaires sociaux et les applications sociales capturent des ensembles de champs légèrement différents ; voir la section pour chacun des éléments ci-dessous.

>[!AVAILABILITY]
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

### Capturé via le remplissage du formulaire de réseau social {#captured-via-social-form-fill}

Selon les paramètres de confidentialité du réseau et de l’utilisateur, un ou plusieurs de ces champs sont récupérés :

>[!CAUTION]
>
>Les données capturées par le remplissage de formulaires sociaux remplacent les champs correspondants, sauf si vous [bloquez les mises à jour de ces champs au niveau du formulaire](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

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
>Le remplissage de formulaire Social capture l’adresse électronique _uniquement_ si la personne l’entre dans le formulaire. Si vous avez besoin de l’adresse électronique, vous devez [en faire un champ obligatoire dans votre formulaire](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Pour capturer ces informations à partir de formulaires, activez [remplissage de formulaire social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
