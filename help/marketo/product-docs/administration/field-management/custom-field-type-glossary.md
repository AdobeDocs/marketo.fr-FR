---
unique-page-id: 2951259
description: Glossaire du type de champ personnalisé - Documents Marketo - Documentation du produit
title: Glossaire du type de champ personnalisé
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 2%

---

# Glossaire du type de champ personnalisé {#custom-field-type-glossary}

Lorsque vous créez un champ personnalisé dans Marketo, vous avez le choix entre une liste de types.

>[!PREREQUISITES]
>
>[Création d’un champ personnalisé dans Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Selon le type de champ, filtrer/déclencher [opérateurs](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) sera différent.

>[!NOTE]
>
>La plupart des champs ne peuvent pas dépasser le nombre de caractères, mais plutôt le nombre d’octets. Pour cette raison, nous ne pouvons pas fournir de limite de caractères définitive pour chaque champ. L’exception est **Chaîne**, qui peut contenir jusqu’à 255 caractères.

## Booléenne {#boolean}

**Exemple de nom :** Est client : marquez vos clients comme des clients

**Exemples de valeurs :** True (coché) / False (non coché)

**Opérateurs**: Aucun

## Devise {#currency}

**Exemple de nom :** Budget : stocke une valeur numérique pour le budget d’une entreprise.

**Exemples de valeurs :** 100

**Opérateurs**: est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Date {#date}

**Exemple de nom :** Date de renouvellement - Stocker les dates de renouvellement de vos clients

**Exemples de valeurs :** 8/19/14

**Opérateurs**: est, n’est pas, entre, dans le passé, dans le passé avant, dans le futur après, dans la période, après, avant, après, après ou après, sur ou avant, est vide, n’est pas vide

## Datetime {#datetime}

**Exemple de nom :** Date de création : stocke la date et l’heure de création d’une personne.

**Exemples de valeurs :** 8/19/14 02:00

**Opérateurs**: est, n’est pas, entre, dans le passé, dans le passé avant, dans le futur après, dans la période, après, avant, après, après ou après, sur ou avant, est vide, n’est pas vide

## Adresse e-mail {#email}

**Exemple de nom :** Autre adresse électronique : conservez une autre adresse électronique pour vos personnes (ne peut pas envoyer de courriers électroniques à ce champ comme le champ d’adresse électronique par défaut, celui-ci est spécial).

**Exemples de valeurs :** name@company.com

**Opérateurs**: est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## Flottante {#float}

**Exemple de nom :** Moyenne par point d’évaluation : permet de conserver la moyenne par point d’évaluation d’une personne ou toute autre valeur numérique ayant des décimales.

**Exemples de valeurs :** 2,47

**Opérateurs**: entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Formule {#formula}

**Exemple de nom :** Salutations : utilisez ce champ spécial dans une [solution pour obtenir la formule de salutation appropriée](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) selon le genre

**Exemples de valeurs :** vérifier la solution liée

## Entier {#integer}

**Exemple de nom :** Nombre d’employés : stocke une valeur numérique qui ne nécessite pas de décimales.

**Exemples de valeurs :** 600

**Opérateurs**: est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Pourcentage {#percent}

**Exemple de nom :** Probablement à acheter : stockez une valeur en pourcentage (peut-être calculée côté CRM).

**Exemples de valeurs :** 85 %

**Opérateurs**: est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Téléphone {#phone}

**Exemple de nom :** Autre téléphone : stockez un numéro de téléphone supplémentaire pour vos utilisateurs.

**Exemple de valeur :** 650-555-5555

**Opérateurs**: est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## Évaluation {#score}

**Exemple de nom :** Score comportemental/Score démographique : créez plusieurs champs de score pour effectuer le suivi des différents attributs.

**Exemple de valeur :** 14

**Opérateurs**: est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Chaîne {#string}

**Exemple de nom :** Middle Name - stocker un attribut de texte supplémentaire

**Exemple de valeur :** Rose

**Opérateurs**: est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## Zone de texte {#text-area}

**Exemple de nom :** Commentaires : ajoutez un champ de commentaires à vos formulaires pour autoriser la saisie de texte multiligne.

**Exemple de valeur :** Cet article est fantastique !

**Opérateurs**: est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## URL {#url}

**Exemple de nom :** Blog : créez un champ pour stocker les URL de blog d’une personne.

**Exemple de valeur :** www.myblog.com

**Opérateurs**: est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide
