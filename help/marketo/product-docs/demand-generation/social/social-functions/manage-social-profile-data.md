---
unique-page-id: 2950578
description: Gérer les données de profil social - Documents Marketo - Documentation du produit
title: Gestion des données de profil Social
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 8%

---

# Gestion des données de profil Social {#manage-social-profile-data}

Lorsqu’une personne interagit avec un Marketo [application sociale](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)ou autorise leur réseau social à préremplir un formulaire Marketo avec [remplissage de formulaire social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo capture toutes les données disponibles à partir de leur profil social. Vous pouvez afficher ces informations sur la variable [Page Détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)ou l’ajouter en tant que colonne dans une [vue personnalisée d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

le remplissage de formulaires sociaux et les applications sociales capturent des ensembles de champs légèrement différents ; consultez la section pour chacun des éléments ci-dessous.

>[!AVAILABILITY]
>
>Tous les clients n’ont pas acheté cette fonctionnalité. Contactez votre représentant commercial pour plus d&#39;informations.

## Capturé via l’application sociale {#captured-via-social-app}

Selon les paramètres de confidentialité du réseau et de l’utilisateur, un ou plusieurs de ces champs sont récupérés :

>[!NOTE]
>
>Les informations supplémentaires provenant des réseaux sociaux apparaissent sur la page Détails de la personne environ cinq minutes après l’autorisation de la personne.

## Depuis Twitter : {#from-twitter}

* Prénom (analysé à partir du nom d’affichage)
* Nom (analysé à partir du nom d’affichage)
* URL de la photo de profil
* URL de la page de profil
* Portée sociale (nombre d’abonnés)

>[!NOTE]
>
>Les applications sociales ne récupèrent pas l’adresse électronique de la personne.

## Depuis Facebook : {#from-facebook}

* Prénom
* Nom
* URL du profil
* URL de la photo de profil
* Sexe
* Portée sociale (nombre d’amis)

### Capturé via le remplissage de formulaire Social {#captured-via-social-form-fill}

Selon les paramètres de confidentialité du réseau et de l’utilisateur, un ou plusieurs de ces champs sont récupérés :

>[!CAUTION]
>
>Les données capturées par le remplissage de formulaires sur les réseaux sociaux remplacent les champs correspondants, sauf si vous [bloquer les mises à jour de ces champs au niveau du formulaire ;](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Depuis Twitter : {#from-twitter-1}

* Prénom (analysé à partir du nom d’affichage)
* Nom (analysé à partir du nom d’affichage)
* Adresse e-mail

## De Facebook: {#from-facebook-1}

* Prénom
* Nom
* Adresse e-mail
* Date de naissance
* Intitulé du poste
* Société

>[!NOTE]
>
>Le remplissage de formulaire Social capture l’adresse électronique. _only_ si la personne la saisit dans le formulaire. Si vous avez besoin de l’adresse électronique, vous devez [en faire un champ obligatoire dans votre formulaire](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Pour capturer ces informations à partir de formulaires, activez l’option [remplissage de formulaire social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
