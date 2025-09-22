---
unique-page-id: 14352509
description: Glossaire des champs dynamiques - Documents Marketo - Documentation du produit
title: Glossaire des champs dynamiques
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 4%

---

# Glossaire des champs dynamiques {#dynamic-fields-glossary}

Lors de la création d’un modèle dans [!DNL Sales Connect], il est toujours recommandé d’intégrer des champs dynamiques à l’aide du bouton **[!UICONTROL Champs dynamiques MSE]**.

Cet outil est utilisé pour `auto-personalize your email` et vous faire gagner des tonnes de temps par `pulling information from the [!UICONTROL People] page`.

| Champ dynamique | Exemple de ce qui apparaît dans votre email |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Si vous ne souhaitez plus recevoir d&#39;emails de notre part, cliquez ici |
| `{{friendly_unsubscribe}}` | Fatigué de tous les e-mails ? Prévenez-moi ici |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, rédacteur technique principal - Adobe |
| `{{personal_email}}` | <keith@pickyouremail.com> |
| `{{title}}` | Rédacteur technique principal |
| `{{work_website}}` | <https://www.adobe.com> |

**Points à noter** :

* Si les informations d&#39;un contact ne sont pas saisies correctement ou sont absentes de la page Personnes, elles ne s&#39;afficheront pas correctement dans votre modèle.
* La différence entre `{{company}}` et `{{company_friendly}}` est que `{{company_friendly}}` supprimera tout titre formel, tel que Inc., LLC., etc., du nom de la société de votre contact.
* Lorsque vous utilisez `{{company_friendly}}`, veillez à séparer Inc. ou Co. par une virgule dans les coordonnées. C’est ainsi que Sales Connect sait ce qu’il faut supprimer lors de l’extraction de la valeur.
* Le système ajoute automatiquement la signature de l’utilisateur à chaque e-mail envoyé. Si l’utilisateur utilise un modèle avec le champ dynamique `{{my_signature}}`, le système renseigne la signature dans laquelle le champ dynamique `{{my_signature}}` a été placé. On ne l&#39;ajoute que pour éviter le dédoublement. Le système `{{team_unsubscribe}}` gère de la même manière lorsque le paramètre de désabonnement d’ajout global est activé.

>[!TIP]
>
>Vous pouvez créer votre propre [champ dynamique personnalisé](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) pour tout ce que vous souhaitez avoir automatiquement extrait dans vos emails
