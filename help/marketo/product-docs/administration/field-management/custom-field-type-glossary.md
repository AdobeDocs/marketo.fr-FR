---
unique-page-id: 2951259
description: Référence pour les types de champs personnalisés dans Marketo, notamment Booléen, Devise, Date, E-mail, Formule, etc.
title: Glossaire de type de champ personnalisé
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
TQID: https://experienceleague.adobe.com/Dh25WBFjkhrFODNcn6DpWNC9F2F-3D7C24Nwkv8fbOM
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 601
ht-degree: 3%

---

# Glossaire de type de champ personnalisé {#custom-field-type-glossary}

Lorsque vous créez un champ personnalisé dans Marketo, vous disposez d’une liste de types.

>[!PREREQUISITES]
>
>[Créer un champ personnalisé dans Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Selon le type de champ, le filtre/déclencheur [opérateurs](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) sera différent.

>[!NOTE]
>
>La plupart des champs ne sont pas limités par le nombre de caractères, mais par le nombre d’octets. Pour cette raison, Marketo n’est pas en mesure de fournir une limite de caractères définitive pour chaque champ. L’exception est **String**, qui atteint sa limite de 255 caractères.

## Booléen {#boolean}

**Exemple de nom :** Est client - Identifiez les personnes comme des clients

**Exemples de valeurs :** True (coché) / False (non coché)

**Opérateurs** : aucun

## Devise {#currency}

**Exemple de nom :** Budget - Stocker une valeur numérique pour le budget d’une entreprise

**Exemples de valeurs :** 100

**Opérateurs** : est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Date {#date}

**Exemple de nom :** Date de renouvellement - Stockez les dates de renouvellement de vos clients

**Exemples de valeurs :** 8/19/14

**Opérateurs** : est, n’est pas, entre, dans le passé, dans le passé avant, dans le futur, dans le futur après, dans le délai, après, avant, on ou après, on ou avant, est vide, n’est pas vide

## Datetime {#datetime}

**Exemple de nom :** Date de création - Stockez la date et l’heure de création d’une personne

**Exemples de valeurs :** 8/19/14 2:00

**Opérateurs** : est, n’est pas, entre, dans le passé, dans le passé avant, dans le futur, dans le futur après, dans le délai, après, avant, on ou après, on ou avant, est vide, n’est pas vide

## E-mail {#email}

**Exemple de nom :** Autre adresse e-mail - Conservez une autre adresse e-mail pour les personnes (impossible d’envoyer réellement des e-mails à ce champ comme le champ Adresse e-mail par défaut)

**Exemples de valeurs :** <name@company.com>

**Opérateurs** : est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## Flottante {#float}

**Exemple de nom :** Moyenne par point de note - Conservez la moyenne par point de note d’une personne ou toute autre valeur numérique comportant des décimales

**Exemples de valeurs :** 2,47

**Opérateurs** : entre, supérieur à, inférieur à, au moins, au plus, est vide, n’est pas vide.

## Formule {#formula}

**Exemple de nom : Salutations** - Utilisez ce champ spécial dans une [solution pour obtenir la salutation appropriée](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) en fonction du sexe

**Exemples de valeurs :** Vérifier la solution liée

## Nombre entier {#integer}

**Exemple de nom :** Nombre d’employés - Stockez une valeur numérique qui ne nécessite pas de décimales

**Exemples de valeurs :** 600

**Opérateurs** : est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Pourcentage {#percent}

**Exemple de nom :** susceptible d’acheter - Stocker une valeur en pourcentage (calculée dans le CRM)

**Exemples de valeurs :** 85 %

**Opérateurs** : est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Téléphone {#phone}

**Exemple de nom :** autre téléphone - Stocker un numéro de téléphone supplémentaire pour les personnes

**Exemple de valeur :** 650-555-5555

**Opérateurs** : est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## Score {#score}

**Exemple de nom :** score comportemental/score démographique - Créez plusieurs champs de score pour effectuer le suivi de différents attributs

**Exemple de valeur :** 14

**Opérateurs** : est, n’est pas, entre, supérieur à, inférieur à, au moins, est vide, n’est pas vide

## Chaîne {#string}

**Exemple de nom : Deuxième prénom** - Stockez un attribut de texte supplémentaire

**Exemple de valeur :** Rose

**Opérateurs** : est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## Zone de texte {#text-area}

**Exemple de nom :** Commentaires - Ajoutez un champ de commentaires à vos formulaires pour autoriser la saisie de texte multiligne

**Exemple de valeur :** cet article est fantastique !

**Opérateurs** : est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide

## URL {#url}

**Exemple de nom :** Blog - Créez un champ pour stocker les URL de blog d’une personne

**Exemple de valeur :** &lt;www.myblog.com>

**Opérateurs** : est, n’est pas, commence par, ne commence pas par, contient, ne contient pas, est vide, n’est pas vide
