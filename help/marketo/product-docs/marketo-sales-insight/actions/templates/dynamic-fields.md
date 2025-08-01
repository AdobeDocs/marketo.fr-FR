---
description: Dynamic Fields - Documents Marketo - Documentation du produit
title: Champs dynamiques
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 1%

---

# Champs dynamiques {#dynamic-fields}

Nous vous permettons de personnaliser vos modèles d’e-mail avec des attributs prédéfinis tels que `{{first_name}}` ou `{{company}}`. Ces champs vous permettent d’envoyer plusieurs e-mails à des contacts et de remplir automatiquement ces champs sans avoir à les saisir séparément pour chaque contact.

>[!TIP]
>
>Les champs « first_name » et « company » sont les seuls champs qui s’appliqueront à [!DNL Sales Insight Actions] et [!DNL Salesforce]. Cela signifie que si un contact n’existe pas dans l’[application web](https://toutapp.com/login), nous recherchons dans [!DNL Salesforce] si nous pouvons trouver un enregistrement contact/prospect avec une adresse e-mail correspondante. Nous utilisons ensuite les informations de cet enregistrement pour remplir le champ.

## Insertion d’un champ dynamique dans un modèle {#insert-a-dynamic-field-into-a-template}

1. Dans **[!UICONTROL Modèles et campagnes]**, recherchez le modèle à modifier, puis cliquez sur **[!UICONTROL Modifier le modèle]**.

1. Cliquez sur **[!UICONTROL Insérer un champ dynamique]**.

   >[!NOTE]
   >
   >Lors de l’envoi d’e-mails à des contacts qui existent dans [!DNL Sales Insight Actions], vous pouvez utiliser les champs dynamiques de base. Ceux-ci tireront directement du contact.

Si vous envoyez un e-mail à des contacts qui existent dans [!DNL Salesforce], vous pouvez tirer parti des champs dynamiques [!DNL Salesforce]. Tout commence par « sfdc ». Tant que vous disposez d’une connexion à [!DNL Salesforce], ces champs appellent directement le prospect/contact dans [!DNL Salesforce] pour renseigner les informations dans le modèle.

## Insertion de champs dynamiques dans une ligne d&#39;objet {#insert-dynamic-fields-in-a-subject-line}

Il vous suffit de les copier et de les coller manuellement dans le champ Objet d’un e-mail, en veillant à disposer de la mise en forme appropriée.

## Valeurs par défaut des champs dynamiques {#dynamic-field-default-values}

Lors de l’ajout de champs dynamiques à vos modèles d’e-mail, vous pouvez ajouter une valeur par défaut que le champ dynamique remplacera s’il n’existe aucune autre valeur disponible.

Pour ce faire, ajoutez « | » après le libellé du champ dynamique, puis ajoutez « default: » (les deux sans guillemets). Ajoutez ensuite la valeur que vous souhaitez que le champ résolve sur (entre guillemets) si aucune autre valeur n’a pu être trouvée.

**Exemple :**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## Glossaire des champs dynamiques {#dynamic-fields-glossary}

Lors de la création d&#39;un modèle dans [!DNL Sales Insight Actions], il est toujours recommandé d&#39;intégrer des champs dynamiques à l&#39;aide du bouton **[!UICONTROL Insérer un champ dynamique]**.

Cet outil est utilisé pour `auto-personalize your email` et vous faire gagner des tonnes de temps par `pulling information from the People page`.

| Champ dynamique | Exemple de ce qui apparaît dans votre email |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Si vous ne souhaitez plus recevoir d&#39;emails de notre part, cliquez ici |
| `{{friendly_unsubscribe}}` | Fatigué de tous les e-mails ? Prévenez-moi ici |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, rédacteur technique principal - Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Rédacteur technique principal |
| `{{work_website}}` | https://www.adobe.com |

**Points à noter** :

* Si les informations d&#39;un contact ne sont pas saisies correctement ou sont absentes de la page Personnes, elles ne s&#39;afficheront pas correctement dans votre modèle.
* La différence entre `{{company}}` et `{{company_friendly}}` est que `{{company_friendly}}` supprimera tout titre formel, tel que Inc., LLC., etc., du nom de la société de votre contact.
* Lorsque vous utilisez `{{company_friendly}}`, veillez à séparer Inc. ou Co. par une virgule dans les coordonnées. C’est ainsi que [!DNL Sales Insight Actions] savez quoi supprimer lors de l’extraction de la valeur.
* Nous vous permettons de personnaliser vos modèles d’e-mail avec des attributs prédéfinis tels que `{{my_name}}` ou `{{my_title}}`. Ces champs vous permettent de vous référencer rapidement dans vos modèles d’e-mail.
* Le système ajoute automatiquement la signature de l’utilisateur à chaque e-mail envoyé. Si l’utilisateur utilise un modèle avec le champ dynamique `{{my_signature}}`, le système renseigne la signature dans laquelle le champ dynamique `{{my_signature}}` a été placé. On ne l&#39;ajoute que pour éviter le dédoublement. Le système `{{team_unsubscribe}}` gère de la même manière lorsque le paramètre de désabonnement d’ajout global est activé.

>[!TIP]
>
>Si vos champs dynamiques ne sont pas renseignés, consultez [cet article](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
