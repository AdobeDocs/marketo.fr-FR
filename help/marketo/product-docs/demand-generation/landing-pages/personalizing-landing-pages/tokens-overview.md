---
unique-page-id: 2950799
description: Présentation des jetons - Documents marketing - Documentation du produit
title: Présentation des jetons
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# Présentation des jetons {#tokens-overview}

Un jeton est une variable qui peut être utilisée dans les étapes de flux de campagne intelligente de Marketing Cloud, les courriels, les landings page, les fragments de code et les campagnes Web.

## Présentation des valeurs par défaut {#understanding-default-values}

Lorsque vous utilisez un jeton, vous souhaitez également fournir une valeur par défaut. Il s’agit du texte qui indique si une personne n’a pas de valeur pour le champ référencé.

![](assets/image2014-12-2-13-3a16-3a48.png)

Dans cet exemple, le courrier électronique indique &quot;Salutations (prénom)&quot; ou &quot;Salutations, tremblement de terre&quot; (valeur par défaut).

![](assets/two.png)

>[!CAUTION]
>
>Les jetons ne fonctionnent pas dans le préen-tête lors de l’utilisation de l’éditeur de courrier électronique de Marketo. Pour utiliser un jeton dans le préen-tête, il doit se trouver par le biais de votre propre code HTML dans un modèle de courrier électronique.

>[!NOTE]
>
>Cette liste n&#39;est pas exhaustive. Les jetons sont également créés pour chaque champ personnalisé de Marketo.

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

## Jetons de société {#company-tokens}

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
* Les champs de société personnalisée fonctionnent également si vous utilisez leur nom d’affichage, par exemple. `{{Company.Custom Field Name}}`

## Jetons Campaign {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## Jetons système {#system-tokens}

>[!NOTE]
>
>Pour en savoir plus sur ces jetons, consultez le [glossaire des jetons système](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

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
>Pour plus d&#39;informations sur les jetons [pour les moments intéressants](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/tokens-for-interesting-moments.md) en fonction des déclencheurs utilisés dans une campagne dynamique,

## Jetons de programme {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## Mes jetons {#my-tokens}

Mes jetons sont définis dans un programme et commencent par `{{my.` suivi du nom que vous avez créé pour le jeton. En savoir plus sur [Mes jetons dans un programme](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Jeton de membre {#member-token}

Les jetons de membre sont utilisés pour insérer des valeurs uniques provenant de partenaires de services intégrés. Les jetons de membre sont couramment utilisés pour les URL uniques des participants au webinaire. Chaque personne dispose d’une URL unique pour accéder au webinaire qui peut être insérée à l’aide d’un jeton `{{member.webinar url}}`. Le jeton `{{member.webinar url}}` résout automatiquement l’URL de confirmation unique de la personne générée par le prestataire.

* `{{member.webinar url}}`

>[!CAUTION]
>
>Le jeton `{{member.webinar url}}` ne sera renseigné que si la campagne dynamique qui envoie le courriel est un actif enfant du Programme de Événement.
