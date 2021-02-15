---
unique-page-id: 14352509
description: Glossaire des champs dynamiques - Documents marketing - Documentation du produit
title: Glossaire des champs dynamiques
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Glossaire des champs dynamiques {#dynamic-fields-glossary}

Lors de la création d&#39;un modèle dans Sales Connect, il est toujours recommandé d&#39;intégrer des champs dynamiques à l&#39;aide du bouton **Champs dynamiques MSE**.

Cet outil est utilisé pour `auto-personalize your email` et vous permet de gagner du temps par `pulling information from the People page`.

| Champ dynamique | Exemple de ce qui apparaît dans votre courrier électronique |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Si vous ne voulez plus entendre parler de moi, veuillez me le faire savoir ici. |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Rédacteur technique principal |
| `{{work_website}}` | https://www.marketo.com |

**A noter** :

* Si les informations d’un contact sont saisies incorrectement ou sont manquantes dans la page Personnes, elles ne sont pas correctement récupérées dans votre modèle.
* La différence entre `{{company}}` et `{{company_friendly}}` est que `{{company_friendly}}` supprimera tout titre officiel, tel que Inc., LLC., etc., du nom de la société de votre contact.
* Lorsque vous utilisez `{{company_friendly}}`, veillez à séparer Inc. ou Co. par une virgule dans les coordonnées. C&#39;est ainsi que Sales Connect sait ce qu&#39;il faut supprimer lorsqu&#39;il tire la valeur.

>[!TIP]
>
>Vous pouvez créer votre propre [champ dynamique personnalisé](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) pour tout ce que vous souhaitez extraire automatiquement dans vos courriers électroniques.
