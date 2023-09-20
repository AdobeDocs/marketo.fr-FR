---
unique-page-id: 14352509
description: Glossaire des champs dynamiques - Documents Marketo - Documentation du produit
title: Glossaire des champs dynamiques
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: d6a3d95ed42d1c08d69014e1aa013e7436bd06c2
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 2%

---

# Glossaire des champs dynamiques {#dynamic-fields-glossary}

Lors de la création d’un modèle dans Sales Connect, il est toujours recommandé d’intégrer les champs dynamiques à l’aide de la variable **Champs dynamiques MSE** bouton .

Cet outil est utilisé pour `auto-personalize your email` et vous permettent de gagner du temps en `pulling information from the People page`.

| Champ dynamique | Exemple de ce qui apparaît dans votre email |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Si vous ne voulez plus entendre parler de moi, faites-le-moi savoir ici. |
| `{{my_name}}` | Keith Flynn |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Rédacteur technique senior |
| `{{work_website}}` | https://www.adobe.com |

**Remarques :**:

* Si les informations d’un contact sont incorrectement saisies ou sont manquantes dans la page Personnes, elles ne s’affichent pas correctement dans votre modèle.
* La différence entre `{{company}}` et `{{company_friendly}}` est que `{{company_friendly}}` Supprimera tout titre formel, tel que Inc., LLC, etc., du nom de la société de votre contact.
* Lorsque vous utilisez `{{company_friendly}}`, veillez à séparer Inc. ou Co. avec une virgule dans les détails du contact. C’est ainsi que Sales Connect sait quoi supprimer lors de l’extraction de la valeur.

>[!TIP]
>
>Vous pouvez créer les vôtres [champ dynamique personnalisé](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) pour tout ce que vous souhaitez que soit automatiquement extrait dans vos emails
