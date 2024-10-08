---
unique-page-id: 2950578
description: Gérer les données de profil social - Documents Marketo - Documentation du produit
title: Gestion des données de profil Social
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 5%

---

# Gestion des données de profil Social {#manage-social-profile-data}

Lorsqu’une personne interagit avec une [application sociale](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) de Marketo ou autorise son réseau social à préremplir un formulaire Marketo avec le [remplissage de formulaire social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo capture toutes les données disponibles à partir de son profil social. Vous pouvez afficher ces informations sur la [page Détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) ou les ajouter en tant que colonne dans une [ vue personnalisée d’une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

>[!IMPORTANT]
>
>Le 31 juillet 2024, nous avons commencé à abandonner cette fonctionnalité. Il n’est plus possible de créer de nouvelles ressources. Les ressources existantes continueront à fonctionner jusqu’au 31 janvier 2025. [En savoir plus](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Le remplissage de formulaires sociaux et les applications sociales capturent des ensembles de champs légèrement différents ; reportez-vous à la section pour chacun des champs ci-dessous.

>[!AVAILABILITY]
>
>Tous les utilisateurs de Marketo Engage n’ont pas acheté cette fonctionnalité. Pour plus d’informations, contactez l’équipe du compte d’Adobe (votre gestionnaire de compte).

## Capturé via l’application sociale {#captured-via-social-app}

Selon les paramètres de confidentialité du réseau et de l’utilisateur, un ou plusieurs de ces champs sont récupérés :

>[!NOTE]
>
>Les informations supplémentaires provenant des réseaux sociaux apparaissent sur la page Détails de la personne environ cinq minutes après l’autorisation de la personne.

## Par Twitter : {#from-twitter}

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
* Genre
* Portée sociale (nombre d’amis)

### Capturé via le remplissage de formulaire Social {#captured-via-social-form-fill}

Selon les paramètres de confidentialité du réseau et de l’utilisateur, un ou plusieurs de ces champs sont récupérés :

>[!CAUTION]
>
>Les données capturées par le remplissage de formulaire social remplacent les champs correspondants, sauf si vous [bloquez les mises à jour de ces champs au niveau du formulaire](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Par Twitter : {#from-twitter-1}

* Prénom (analysé à partir du nom d’affichage)
* Nom (analysé à partir du nom d’affichage)
* E-mail

## Depuis Facebook : {#from-facebook-1}

* Prénom
* Nom
* E-mail
* Date de naissance
* Intitulé du poste
* Société

>[!NOTE]
>
>Le remplissage de formulaire Social capture l’adresse électronique _uniquement_ si la personne la saisit dans le formulaire. Si vous avez besoin de l’adresse électronique, [ faites-en un champ obligatoire dans votre formulaire ](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Pour capturer ces informations à partir de formulaires, activez le [remplissage de formulaire social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
