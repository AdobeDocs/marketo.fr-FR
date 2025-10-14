---
unique-page-id: 2950799
description: Présentation Des Jetons - Documents Marketo - Documentation Du Produit
title: Vue d’ensemble des jetons
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 2%

---

# Vue d’ensemble des jetons {#tokens-overview}

Un jeton est une variable qui peut être utilisée dans les étapes de flux de campagne intelligente Marketo, les e-mails, les pages de destination, les fragments de code et les campagnes web.

## Comprendre les valeurs par défaut {#understanding-default-values}

Lorsque vous utilisez un jeton, vous souhaitez également fournir une valeur par défaut. Il s’agit du texte qui indique si une personne ne dispose pas d’une valeur pour le champ que vous référencez.

![](assets/image2014-12-2-13-3a16-3a48.png)

Dans cet exemple, l’e-mail dira « Salutations, (prénom) » ou « Salutations, mise à la terre » (valeur par défaut).

![](assets/two.png)

>[!CAUTION]
>
>Les jetons ne fonctionnent pas dans le pré-titre lors de l’utilisation de l’éditeur d’e-mail Marketo. Pour utiliser un jeton dans le pré-titre, il doit passer par votre propre HTML dans un modèle d’e-mail.

>[!NOTE]
>
>Cette liste n’est pas exhaustive. Des jetons sont également créés pour chaque champ personnalisé que vous avez dans Marketo.

## Jetons de personne {#person-tokens}

* `{{lead.Acquisition Date}}`
* `{{lead.Acquisition Program Name}}`
* `{{lead.Acquisition Program}}`
* `{{lead.Address}}`
* `{{lead.Anonymous IP}}`
* `{{lead.Black Listed}}`
* `{{lead.City}}`
* `{{lead.Country}}`
* `{{lead.Created At}}`
* `{{lead.Date of Birth}}`
* `{{lead.Department}}`
* `{{lead.Do Not Call}}`
* `{{lead.Do Not Call Reason}}`
* `{{lead.Email Address}}`
* `{{lead.Email Invalid}}`
* `{{lead.Email Invalid Cause}}`
* `{{lead.Fax Number}}`
* `{{lead.First Name}}`
* `{{lead.Full Name}}`
* `{{lead.Id}}`
* `{{lead.Inferred City}}`
* `{{lead.Inferred Company}}`
* `{{lead.Inferred Country}}`
* `{{lead.Inferred Metropolitan Area}}`
* `{{lead.Inferred Phone Area Code}}`
* `{{lead.Inferred Postal Code}}`
* `{{lead.Inferred State Region}}`
* `{{lead.Is Customer}}`
* `{{lead.Is Employee}}`
* `{{lead.Is Partner}}`
* `{{lead.Job Title}}`
* `{{lead.Last Name}}`
* `{{lead.Lead Source}}`
* `{{lead.Marketing Suspended}}`
* `{{lead.Middle Name}}`
* `{{lead.Mobile Phone Number}}`
* `{{lead.Original Referrer}}`
* `{{lead.Original Search Engine}}`
* `{{lead.Original Search Phrase}}`
* `{{lead.Original Source Info}}`
* `{{lead.Original Source Type}}`
* `{{lead.Person Notes}}`
* `{{lead.Phone Number}}`
* `{{lead.Registration Source Info}}`
* `{{lead.Registration Source Type}}`
* `{{lead.Salutation}}`
* `{{lead.SFDC Created Date}}`
* `{{lead.SFDC Is Deleted}}`
* `{{lead.SFDC Type}}`
* `{{lead.Unsubscribed}}`
* `{{lead.Unsubscribed Reason}}`
* `{{lead.Updated At}}`
* Les champs de personne personnalisés fonctionnent également si vous utilisez leur nom d’affichage, par exemple `{{lead.Custom Field Name}}`

## Jetons d’entreprise {#company-tokens}

* `{{Company.Account Owner Email Address}}`
* `{{Company.Address}}`
* `{{Company.Annual Revenue}}`
* `{{Company.City}}`
* `{{Company.Company Name}}`
* `{{Company.Company Notes}}`
* `{{Company.Country}}`
* `{{Company.Industry}}`
* `{{Company.Main Phone}}`
* `{{Company.Num Employees}}`
* `{{Company.Parent Company Name}}`
* `{{Company.Postal Code}}`
* `{{Company.SFDC Account Num}}`
* `{{Company.SFDC Created Date}}`
* `{{Company.SFDC Type}}`
* `{{Company.SIC Code}}`
* `{{Company.Site}}`
* `{{Company.State}}`
* `{{Company.Website}}`
* Les champs de société personnalisés fonctionnent également si vous utilisez leur nom d’affichage, par exemple. `{{Company.Custom Field Name}}`

## Jetons de campagne {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## Jetons système {#system-tokens}

>[!NOTE]
>
>Pour en savoir plus sur ces jetons, consultez le [Glossaire des jetons système](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## Jetons de déclenchement {#trigger-tokens}

* `{{trigger.Trigger Name}}`
* `{{trigger.Name}}`
* `{{trigger.Link}}`
* `{{trigger.Subject}}`
* `{{trigger.Category}}`
* `{{trigger.Details}}`
* `{{trigger.Web Page}}`
* `{{trigger.Client IP Address}}`
* `{{trigger.Sent By}}`
* `{{trigger.Received By}}`
* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!NOTE]
>
>Obtenez plus d’informations sur les [jetons pour les moments intéressants](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) en fonction des déclencheurs utilisés dans une campagne intelligente.

## Jetons de programme {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## [!UICONTROL Mes jetons] {#my-tokens}

[!UICONTROL Mes jetons] sont définis dans un programme et commencent par `{{my.` suivi du nom que vous avez créé pour le jeton. En savoir plus sur [&#x200B; Mes jetons dans un programme &#x200B;](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Jeton de membre {#member-token}

Les jetons de membre sont utilisés pour insérer des valeurs uniques provenant de partenaires de services intégrés. Les jetons de membre sont fréquemment utilisés pour les URL uniques des participants au webinaire. Chaque personne dispose d’une URL unique pour accéder au webinaire, qui peut être insérée à l’aide d’un jeton `{{member.webinar url}}`. Le jeton d’`{{member.webinar url}}` résout automatiquement l’URL de confirmation unique de la personne générée par le fournisseur d’accès d’accès.

* `{{member.webinar url}}`

>[!CAUTION]
>
>Le jeton `{{member.webinar url}}` n’est renseigné que si la campagne intelligente qui envoie l’e-mail est une ressource enfant du programme d’événement.
