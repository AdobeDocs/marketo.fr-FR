---
unique-page-id: 2951259
description: Glossaire du type de champ personnalisé - Documents Marketo - Documentation du produit
title: Glossaire du type de champ personnalisé
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 2%

---

# Glossaire du type de champ personnalisé {#custom-field-type-glossary}

Lorsque vous créez un champ personnalisé dans Marketo, vous avez le choix entre une liste de types.

>[!PREREQUISITES]
>
>[Créer un champ personnalisé dans Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Selon le type de champ, filter/trigger [opérateurs](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) sera différent.

>[!NOTE]
>
>La plupart des champs ne peuvent pas dépasser le nombre de caractères, mais plutôt le nombre d’octets. Pour cette raison, nous ne sommes pas en mesure de fournir une limite de caractères définitive pour chaque champ. L’exception est **String**, qui peut contenir jusqu’à 255 caractères.

## Booléenne {#boolean}

**Exemple de nom :** Is Customer - Tag your people as customers (Baliser vos clients)

**Exemple de valeurs :** True (coché) / False (non coché)

**Opérateurs** : aucune

## Devise {#currency}

**Exemple de nom :** Budget - Stocker une valeur numérique pour le budget d’une entreprise

**Exemple de valeurs :** 100

**Opérateurs** : est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Date {#date}

**Exemple de nom :** Date de renouvellement - Stocker les dates de renouvellement de vos clients

**Exemple de valeurs :** 8/19/14

**Opérateurs** : est, n’est pas, entre, dans le passé, dans le passé avant, dans le futur après, dans le futur après, dans la période après, avant, avant, après, le ou après, le ou avant est vide, n’est pas vide

## Datetime {#datetime}

**Exemple de nom :** Date de création - Permet de stocker la date et l’heure de création d’une personne.

**Exemple de valeurs :** 8/19/14 2:00

**Opérateurs** : est, n’est pas, entre, dans le passé, dans le passé avant, dans le futur après, dans le futur après, dans la période après, avant, avant, après, le ou après, le ou avant est vide, n’est pas vide

## E-mail {#email}

**Exemple de nom :** Autre adresse électronique : conservez une autre adresse électronique pour vos personnes (ne peut pas envoyer de courriers électroniques dans ce champ comme le champ d’adresse électronique par défaut, celui-ci est spécial)

**Exemples de valeurs :** name@company.com

**Opérateurs** : est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## Flottante {#float}

**Exemple de nom :** Note moyenne - Conserver la moyenne du point d’évaluation d’une personne ou toute autre valeur numérique ayant des décimales

**Exemple de valeurs :** 2.47

**Opérateurs** : entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Formule {#formula}

**Exemple de nom :** Salutations : utilisez ce champ spécial dans une [solution pour obtenir la salutation appropriée](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) en fonction du sexe

**Exemples de valeurs :** vérifiez la solution liée

## Entier {#integer}

**Exemple de nom :** Nombre d’employés - stocke une valeur de nombre qui ne nécessite pas de décimales

**Exemple de valeurs :** 600

**Opérateurs** : est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Pourcentage {#percent}

**Exemple de nom :** Probable d’achat - stockez une valeur en pourcentage (peut-être calculée côté CRM)

**Exemples de valeurs :** 85 %

**Opérateurs** : est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Téléphone {#phone}

**Exemple de nom :** Autre téléphone - stockage d’un numéro de téléphone supplémentaire pour vos personnes

**Exemple de valeur :** 650-555-5555

**Opérateurs** : est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## Évaluation {#score}

**Exemple de nom :** score comportemental / score démographique - créez plusieurs champs de score pour effectuer le suivi des différents attributs.

**Exemple de valeur :** 14

**Opérateurs** : est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Chaîne {#string}

**Exemple de nom :** Middle Name - stocker un attribut de texte supplémentaire

**Exemple de valeur :** Rose

**Opérateurs** : est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## Zone de texte {#text-area}

**Exemple de nom :** Commentaires : ajoutez un champ de commentaires à vos formulaires pour autoriser la saisie de texte multiligne

**Exemple de valeur :** Cet article est fantastique !

**Opérateurs** : est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## URL {#url}

**Exemple de nom :** Blog - créez un champ pour stocker les URL de blog d’une personne

**Exemple de valeur :** www.myblog.com

**Opérateurs** : est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide
