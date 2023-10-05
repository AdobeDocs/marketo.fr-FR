---
unique-page-id: 14352509
description: Glossaire des champs dynamiques - Documents Marketo - Documentation du produit
title: Glossaire des champs dynamiques
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: cffe7a8734f79f887f3aad017a16fad4f04cda74
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%

---

# Glossaire des champs dynamiques {#dynamic-fields-glossary}

Lors de la création d’un modèle dans Sales Connect, il est toujours recommandé d’intégrer les champs dynamiques à l’aide de la variable **Champs dynamiques MSE** bouton .

Cet outil est utilisé pour `auto-personalize your email` et vous permettent de gagner du temps en `pulling information from the People page`.

| Champ dynamique | Exemple de ce qui apparaît dans votre email |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Si vous ne souhaitez plus recevoir d&#39;emails de notre part, cliquez ici |
| `{{friendly_unsubscribe}}` | Fatigué de tous les emails ? Veuillez me le faire savoir ici |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, rédacteur technique senior - Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Rédacteur technique senior |
| `{{work_website}}` | https://www.adobe.com |

**Remarques :**:

* Si les informations d’un contact sont incorrectement saisies ou sont manquantes dans la page Personnes, elles ne s’affichent pas correctement dans votre modèle.
* La différence entre `{{company}}` et `{{company_friendly}}` est que `{{company_friendly}}` Supprimera tout titre formel, tel que Inc., LLC, etc., du nom de la société de votre contact.
* Lorsque vous utilisez `{{company_friendly}}`, veillez à séparer Inc. ou Co. avec une virgule dans les détails du contact. C’est ainsi que Sales Connect sait quoi supprimer lors de l’extraction de la valeur.
* Le système ajoute automatiquement la signature de l’utilisateur à chaque e-mail envoyé. Si l’utilisateur utilise un modèle avec la variable `{{my_signature}}` dynamique, le système renseigne la signature dans laquelle la propriété `{{my_signature}}` champ dynamique a été placé. Il n&#39;est ajouté que pour éviter la duplication. Le système va gérer `{{team_unsubscribe}}` de la même manière que lorsque le paramètre de désabonnement global d’append est activé.

>[!TIP]
>
>Vous pouvez créer les vôtres [champ dynamique personnalisé](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) pour tout ce que vous souhaitez que soit automatiquement extrait dans vos emails
