---
description: Champs dynamiques - Documents Marketo - Documentation du produit
title: Champs dynamiques
hide: true
hidefromtoc: true
source-git-commit: 1db88a95777df43c3cef7ee5cabada2464329661
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 1%

---

# Champs dynamiques {#dynamic-fields}

Vous pouvez personnaliser vos modèles d’email avec des attributs prédéfinis tels que `{{first_name}}` ou `{{company}}`. Ces champs vous permettent d’envoyer un email à plusieurs contacts et de les renseigner automatiquement sans avoir à les entrer séparément pour chaque contact.

>[!TIP]
>
>Les champs &quot;first_name&quot; et &quot;company&quot; sont les seuls champs qui se pencheront à la fois sur les actions Sales Insight et sur Salesforce. Cela signifie que si un contact n’existe pas dans la variable [application web](https://toutapp.com/login), nous recherchons dans Salesforce si nous pouvons trouver un enregistrement de contact/piste avec une adresse électronique correspondante. Nous utilisons ensuite les informations de cet enregistrement pour remplir le champ.

## Insertion d’un champ dynamique dans un modèle {#insert-a-dynamic-field-into-a-template}

1. Dans **Modèles et campagnes**, recherchez le modèle à modifier, puis cliquez sur **Modifier le modèle**.

1. Cliquez sur **Insérer un champ dynamique**.

   >[!NOTE]
   >
   >Lors de l’envoi par courrier électronique de contacts figurant dans les actions Sales Insight , vous pouvez utiliser les champs dynamiques de base. Elles proviennent directement du contact.

Si vous envoyez un courrier électronique à des contacts qui se trouvent dans Salesforce, vous pouvez tirer parti des champs dynamiques Salesforce. Tous commencent par &quot;sfdc&quot;. Tant que vous avez une connexion à Salesforce, ces champs appellent directement le prospect/contact dans Salesforce pour renseigner les informations dans le modèle.

## Insertion de champs dynamiques dans un objet {#insert-dynamic-fields-in-a-subject-line}

Il vous suffit de les copier et de les coller manuellement dans le champ d’objet d’un email, en veillant à disposer du formatage approprié.

## Glossaire des champs dynamiques {#dynamic-fields-glossary}

Lors de la création d’un modèle dans les actions Sales Insight, il est toujours recommandé d’intégrer des champs dynamiques à l’aide de la variable **Insérer un champ dynamique** bouton .

Cet outil est utilisé pour `auto-personalize your email` et vous permettent de gagner du temps en `pulling information from the People page`.

| Champ dynamique | Exemple de ce qui apparaît dans votre email |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Si vous ne voulez plus entendre parler de moi, faites-le-moi savoir ici. |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Rédacteur technique senior |
| `{{work_website}}` | https://www.marketo.com |

**Remarques :**:

* Si les informations d’un contact sont incorrectement saisies ou sont manquantes dans la page Personnes, elles ne s’affichent pas correctement dans votre modèle.
* La différence entre `{{company}}` et `{{company_friendly}}` est que `{{company_friendly}}` Supprimera tout titre formel, tel que Inc., LLC, etc., du nom de la société de votre contact.
* Lors de l’utilisation de `{{company_friendly}}`, veillez à séparer Inc. ou Co. avec une virgule dans les coordonnées. C’est ainsi que les actions Sales Insight savent quoi supprimer lors de l’extraction de la valeur.
* Vous pouvez personnaliser vos modèles d’email avec des attributs prédéfinis tels que `{{my_name}}` ou `{{my_title}}`. Ces champs vous permettent de vous référencer rapidement dans vos modèles d’email.

>[!TIP]
>
>Si vos champs dynamiques ne sont pas renseignés, extrayez [cet article](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out).
