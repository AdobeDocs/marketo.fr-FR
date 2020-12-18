---
unique-page-id: 14352509
description: Glossaire des champs dynamiques - Documents marketing - Documentation du produit
title: Glossaire des champs dynamiques
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '173'
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
| `{{personal_email}}` | [[courriel protégé]](http://docs.marketo.com/cdn-cgi/l/email-protection) |
| `{{title}}` | Rédacteur technique principal |
| `{{work_website}}` | https://www.marketo.com |

**A noter** :

* Si un contact est `information is entered incorrectly` ou est absent de la page Personnes, il est `will not pull over correctly` dans votre modèle.

* La différence entre `{{company}}` et `{{company_friendly}}` est que `{{company_friendly}}` `remove any formal title`, tel que Inc., LLC., etc., sera &lt;a2/> du nom de la société de votre contact.
* Lorsque vous utilisez `{{company_friendly}}`, veillez à séparer Inc. ou Co. par une virgule dans les coordonnées. C&#39;est ainsi que Sales Connect sait ce qu&#39;il faut supprimer lorsqu&#39;il tire la valeur.

>[!TIP]
>
>Vous pouvez créer votre propre [champ dynamique personnalisé](http://docs.marketo.com/x/fADb) pour tout ce que vous souhaitez extraire automatiquement dans vos courriers électroniques.

