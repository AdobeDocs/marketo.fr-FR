---
description: Pourquoi mes champs dynamiques ne sont-ils pas remplis ? - Documents Marketo - Documentation sur le produit
title: Pourquoi mes champs dynamiques ne sont-ils pas remplis ?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 6%

---

# Pourquoi mes champs dynamiques ne sont-ils pas remplis ? {#why-arent-my-dynamic-fields-filling-out}

Les champs dynamiques ne fonctionnent que lorsque vous utilisez un modèle. Les e-mails individuels que vous écrivez ne les rempliront pas.

## Éléments à vérifier {#what-to-check}

Il existe trois types de champs dynamiques dans les actions de Sales Insight : De base, Personnalisé et Salesforce. De base et personnalisé cherchent tous deux à extraire des informations de l’[application web](https://toutapp.com/login){target="_blank"}. Si l&#39;information n&#39;existe pas dans l&#39;application web, les champs seront vides. Les champs Salesforce extraient des informations de [Salesforce.com](https://salesforce.com){target="_blank"}.

**Résolution des problèmes liés [!DNL Salesforce] champs**

Champs [!DNL Salesforce] : par exemple, `{{sfdc_account_name}}`

* Assurez-vous qu’il est correctement connecté aux actions Sales Insight. Accédez à la page [Paramètres]&#x200B;(<https://toutapp.com/login{target="_blank"}> et cliquez sur **Gérer** en regard de votre CRM.

**Résolution des problèmes liés aux champs de base et personnalisés**

Marketo Sales Insight Actions Basic Fields : par exemple, `{{company}}`

Champs personnalisés des actions Marketo Sales Insight : par exemple, `{{custom_field_favorite_movie}}`

* Le champ correspondant doit être enregistré pour votre contact dans la [page Personnes](https://toutapp.com/next#relationships){target="_blank"} pour que notre champ dynamique puisse s’y référer. Par exemple, si vous envoyez un e-mail à Marie et que vous utilisez le champ `{{company}}`, mais que son enregistrement de contact ne répertorie pas une entreprise, nous ne serons pas en mesure de le remplir.

## Pourquoi Mon E-Mail A-T-Il Été Envoyé Sans Remplir Tous Les Champs Dynamiques ? {#why-did-my-email-send-without-populating-all-dynamic-fields}

[!DNL Sales Insight Actions] empêchera l’envoi de vos e-mails si nous ne pouvons pas remplir tous vos champs dynamiques dans l’e-mail. **Cependant** il existe quelques exceptions à cette règle. Certains champs envoient des champs vides ou renseignent automatiquement une valeur si nous en trouvons une. Ces champs et la manière dont ils réagiront s’ils ne peuvent pas les remplir sont répertoriés ci-dessous.

`{{first_name}}` = VIDE

`{{last_name}}` =VIDE

`{{title}}` = VIDE

`{{company}}` = « votre entreprise »

`{{friendly_company}}` = « votre entreprise »

>[!NOTE]
>
>Le champ `{{first_name}}` s’affiche dans [!DNL Sales Insight Actions] et [!DNL Salesforce] pour tenter d’extraire des informations. Tous les autres champs de cette liste ne recherchent que des [!DNL Sales Insight Actions] pour les remplir.
