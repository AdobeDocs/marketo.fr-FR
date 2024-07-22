---
description: Champs dynamiques - Documents Marketo - Documentation du produit
title: Champs dynamiques
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: cffe7a8734f79f887f3aad017a16fad4f04cda74
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Champs dynamiques {#dynamic-fields}

Nous vous permettons de personnaliser vos modèles d&#39;email avec des attributs prédéfinis tels que `{{first_name}}` ou `{{company}}`. Ces champs vous permettent d’envoyer un email à plusieurs contacts et de les renseigner automatiquement sans avoir à les entrer séparément pour chaque contact.

>[!TIP]
>
>Les champs &quot;first_name&quot; et &quot;company&quot; sont les seuls champs qui se pencheront à la fois sur les actions Sales Insight et sur Salesforce. Cela signifie que si un contact n’existe pas dans l’ [application web](https://toutapp.com/login), nous recherchons dans Salesforce si nous pouvons trouver un enregistrement de contact/piste avec une adresse électronique correspondante. Nous utilisons ensuite les informations de cet enregistrement pour remplir le champ.

## Insertion d’un champ dynamique dans un modèle {#insert-a-dynamic-field-into-a-template}

1. Dans **Modèles et campagnes**, recherchez le modèle à modifier, puis cliquez sur **Modifier le modèle**.

1. Cliquez sur **Insérer un champ dynamique**.

   >[!NOTE]
   >
   >Lors de l’envoi par courrier électronique de contacts figurant dans les actions Sales Insight , vous pouvez utiliser les champs dynamiques de base. Elles proviennent directement du contact.

Si vous envoyez un courrier électronique à des contacts qui se trouvent dans Salesforce, vous pouvez tirer parti des champs dynamiques Salesforce. Tous commencent par &quot;sfdc&quot;. Tant que vous avez une connexion à Salesforce, ces champs appellent directement le prospect/contact dans Salesforce pour renseigner les informations dans le modèle.

## Insertion de champs dynamiques dans un objet {#insert-dynamic-fields-in-a-subject-line}

Il vous suffit de les copier et de les coller manuellement dans le champ d’objet d’un email, en veillant à disposer du formatage approprié.

## Valeurs par défaut des champs dynamiques {#dynamic-field-default-values}

Lors de l’ajout de champs dynamiques à vos modèles d’email, vous pouvez ajouter une valeur par défaut à laquelle le champ dynamique se résout si aucune autre valeur n’est disponible.

Pour ce faire, ajoutez &quot;|&quot; après le libellé du champ dynamique, puis ajoutez &quot;default:&quot; (les deux sans guillemets). Ajoutez ensuite la valeur à laquelle le champ doit se résoudre (entre guillemets) si aucune autre valeur n’est trouvée.

**Exemple :**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## Glossaire des champs dynamiques {#dynamic-fields-glossary}

Lors de la création d’un modèle dans les actions Sales Insight, il est toujours recommandé d’intégrer les champs dynamiques à l’aide du bouton **Insérer un champ dynamique** .

Cet outil est utilisé pour `auto-personalize your email` et vous permet de gagner du temps en `pulling information from the People page`.

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

**Choses à noter** :

* Si les informations d’un contact sont incorrectement saisies ou sont manquantes dans la page Personnes, elles ne s’affichent pas correctement dans votre modèle.
* La différence entre `{{company}}` et `{{company_friendly}}` réside dans le fait que `{{company_friendly}}` supprimera tout titre formel, tel que Inc., LLC., etc., du nom de la société de votre contact.
* Lorsque vous utilisez `{{company_friendly}}`, veillez à séparer Inc. ou Co. avec une virgule dans les détails du contact. C’est ainsi que les actions Sales Insight savent quoi supprimer lors de l’extraction de la valeur.
* Nous vous permettons de personnaliser vos modèles d&#39;email avec des attributs prédéfinis tels que `{{my_name}}` ou `{{my_title}}`. Ces champs vous permettent de vous référencer rapidement dans vos modèles d’email.
* Le système ajoute automatiquement la signature de l’utilisateur à chaque e-mail envoyé. Si l’utilisateur utilise un modèle avec le champ dynamique `{{my_signature}}`, le système renseigne la signature où le champ dynamique `{{my_signature}}` a été placé. Il n&#39;est ajouté que pour éviter la duplication. Le système gère `{{team_unsubscribe}}` de la même manière que lorsque le paramètre de désabonnement global de l’ajout est activé.

>[!TIP]
>
>Si vos champs dynamiques ne sont pas renseignés, consultez [cet article](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
