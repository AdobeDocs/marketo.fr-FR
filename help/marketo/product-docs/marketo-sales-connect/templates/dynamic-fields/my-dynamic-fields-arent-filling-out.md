---
unique-page-id: 14352602
description: Mes champs dynamiques ne sont pas renseignés - Documents Marketo - Documentation du produit
title: Mes champs dynamiques ne se remplissent pas.
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 4%

---

# Mes champs dynamiques ne se remplissent pas. {#my-dynamic-fields-arent-filling-out}

Les champs dynamiques ne fonctionnent que lorsque vous utilisez un modèle. Les e-mails individuels que vous écrivez ne les rempliront pas.

## Éléments à vérifier {#what-to-check}

Il existe trois types de champs dynamiques dans [!DNL Sales Connect] : De base, Personnalisé et [!DNL Salesforce]. De base et personnalisé cherchent tous deux à extraire des informations de l’[application web](https://toutapp.com/login). Si l&#39;information n&#39;existe pas dans l&#39;application web, les champs seront vides. Les champs [!DNL Salesforce] extraient des informations de [Salesforce.com](https://salesforce.com).

**Résolution des problèmes liés [!DNL Salesforce] champs**

Champs [!DNL Salesforce] : par exemple, `{{sfdc_account_name}}`

* Assurez-vous qu&#39;il est correctement connecté à [!DNL Sales Connect]. Accédez à la page [Paramètres](https://toutapp.com/login) et cliquez sur **[!UICONTROL Gérer]** en regard de votre CRM.

**Résolution des problèmes liés aux champs de base et personnalisés**

Tous les champs de base : par exemple, `{{company}}`

Tous les champs personnalisés : par exemple, `{{custom_field_favorite_movie}}`

* Le champ correspondant doit être enregistré pour votre contact dans la [page Personnes](https://toutapp.com/next#relationships) pour que notre champ dynamique puisse s’y référer. Par exemple, si vous envoyez un e-mail à Marie et que vous utilisez le champ `{{company}}`, mais que son enregistrement de contact ne répertorie pas une entreprise, nous ne serons pas en mesure de le remplir.

## Pourquoi Mon E-Mail A-T-Il Été Envoyé Sans Remplir Tous Les Champs Dynamiques ? {#why-did-my-email-send-without-populating-all-dynamic-fields}

[!DNL Sales Connect] empêchera l’envoi de vos e-mails si nous ne pouvons pas remplir tous vos champs dynamiques dans l’e-mail. **Cependant** il existe quelques exceptions à cette règle. Certains champs envoient des champs vides ou renseignent automatiquement une valeur si nous en trouvons une. Ces champs et la manière dont ils réagiront s’ils ne peuvent pas les remplir sont répertoriés ci-dessous.

`{{first_name}}` = VIDE

`{{last_name}}` =VIDE

`{{title}}` = VIDE

`{{company}}` = « votre entreprise »

`{{friendly_company}}` = « votre entreprise »

>[!NOTE]
>
>Le champ `{{first_name}}` s’affiche dans [!DNL Sales Connect] et [!DNL Salesforce] pour tenter d’extraire des informations. Tous les autres champs de cette liste ne recherchent que des [!DNL Sales Connect] pour les remplir.
