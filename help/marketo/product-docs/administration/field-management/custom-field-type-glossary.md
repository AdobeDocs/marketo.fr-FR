---
unique-page-id: 2951259
description: Glossaire du type de champ personnalisé - Documents marketing - Documentation du produit
title: Glossaire du type de champ personnalisé
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---


# Glossaire du type de champ personnalisé {#custom-field-type-glossary}

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Lorsque vous créez un champ personnalisé dans Marketing, vous disposez d’une liste de types parmi lesquels choisir.

>[!PREREQUISITES]
>
>* [Créer un champ personnalisé dans Marketo](create-a-custom-field-in-marketo.md)

>



>[!TIP]
>
>Selon le type de champ, les [opérateurs](https://docs.marketo.com/display/public/DOCS/Smart+List+Filter+Operators+Glossary) de filtre/déclencheur seront différents.

>[!NOTE]
>
>La plupart des champs n’excèdent pas le nombre de caractères, mais le nombre d’octets. Pour cette raison, nous ne pouvons pas fournir une limite de caractères définitive pour chaque champ. L’exception est **String**, qui peut contenir jusqu’à 255 caractères.

## Boolean {#boolean}

**Exemple de nom :** Est-il client - Identifiez vos clients comme clients

**Exemples de valeurs :** True (coché) / False (non coché)

**Opérateurs**: Aucun

## Devise {#currency}

**Exemple de nom :** Budget - Stocker une valeur numérique pour un budget de société

**Exemples de valeurs :** 100

**Opérateurs**: est, n&#39;est pas, entre, plus grand que, inférieur, au moins, est vide, n&#39;est pas vide, n&#39;est pas vide

## Date {#date}

**Exemple de nom :** Date de renouvellement - Stocker les dates de renouvellement de vos clients

**Exemples de valeurs :** 19/08/14

**Opérateurs**: est, n&#39;est pas, entre, dans le passé, dans le passé avant, dans le futur après, dans le cadre de la période, après, avant, avant, le ou après, le ou avant, est vide, n&#39;est pas vide

## Date/Heure {#datetime}

**Exemple de nom :** Date de création - Stocker la date et l&#39;heure de création d&#39;une personne

**Exemples de valeurs :** 19/08/14 2:00

**Opérateurs**: est, n&#39;est pas, entre, dans le passé, dans le passé avant, dans le futur après, dans le cadre de la période, après, avant, avant, le ou après, le ou avant, est vide, n&#39;est pas vide

## Courriel {#email}

**Exemple de nom :** Autre adresse électronique : conservez une autre adresse électronique pour vos utilisateurs (il n&#39;est pas possible d&#39;envoyer des courriers électroniques à ce champ comme le champ d&#39;adresse électronique par défaut, celui-ci étant spécial).

**Exemples de valeurs :** [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#335d525e5673505c5e43525d4a1d505c5e)

**Opérateurs**: est, n’est pas, les débuts avec, et non les débuts avec, contient, ne contient pas, est vide, n’est pas vide

## Flottant {#float}

**Exemple de nom :** Moyenne des points de note - Conserver la moyenne des points de note d&#39;une personne ou toute autre valeur numérique ayant des décimales.

**Exemples de valeurs :** 2,47

**Opérateurs**: entre, supérieur à, inférieur, au moins, est vide, n&#39;est pas vide

## Formule {#formula}

**Exemple de nom :** Salutations : utilisez ce champ spécial dans une [solution pour obtenir la formule](create-and-use-a-concatenated-string-formula-field.md) de salutations appropriée en fonction du sexe

**Exemples de valeurs :** vérifier la solution liée

## Entier {#integer}

**Exemple de nom :** Nombre d&#39;employés : stockez une valeur numérique qui ne nécessite pas de décimales.

**Exemples de valeurs :** 600

**Opérateurs**: est, n&#39;est pas, entre, plus grand que, inférieur, au moins, est vide, n&#39;est pas vide, n&#39;est pas vide

## Pourcentage {#percent}

**Exemple de nom :** Achats possibles - stockez un pourcentage (calculé peut-être du côté CRM).

**Exemples de valeurs :** 85 %

**Opérateurs**: est, n&#39;est pas, entre, plus grand que, inférieur, au moins, est vide, n&#39;est pas vide, n&#39;est pas vide

## Téléphone {#phone}

**Exemple de nom :** Autre téléphone : stockez un numéro de téléphone supplémentaire pour votre personnel.

**Exemple de valeur :** 650-555-5555

**Opérateurs**: est, n’est pas, les débuts avec, et non les débuts avec, contient, ne contient pas, est vide, n’est pas vide

## Score {#score}

**Exemple de nom :** Score comportemental / Score démographique : créez plusieurs champs de score pour suivre les différents attributs.

**Exemple de valeur :** 14

**Opérateurs**: est, n&#39;est pas, entre, plus grand que, inférieur, au moins, est vide, n&#39;est pas vide, n&#39;est pas vide

## Chaîne {#string}

**Exemple de nom :** Milieu : stocke un attribut de texte supplémentaire.

**Exemple de valeur :** Rose

**Opérateurs**: est, n’est pas, les débuts avec, et non les débuts avec, contient, ne contient pas, est vide, n’est pas vide

## Zone de texte {#text-area}

**Exemple de nom :** Commentaires : ajoutez un champ de commentaires à vos formulaires pour autoriser la saisie de texte multiligne.

**Exemple de valeur :** Cet article est fantastique !

**Opérateurs**: est, n’est pas, les débuts avec, et non les débuts avec, contient, ne contient pas, est vide, n’est pas vide

## URL {#url}

**Exemple de nom :** Blog : créez un champ pour stocker les URL de blog d&#39;une personne

**Exemple de valeur :** www.myblog.com

**Opérateurs**: est, n’est pas, les débuts avec, et non les débuts avec, contient, ne contient pas, est vide, n’est pas vide
