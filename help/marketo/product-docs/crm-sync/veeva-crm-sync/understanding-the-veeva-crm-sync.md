---
description: Présentation de la synchronisation CRM Veeva - Documents Marketo - Documentation du produit
title: Présentation de la synchronisation CRM Veeva
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Présentation de la synchronisation CRM Veeva {#understanding-the-veeva-crm-sync}

En quelques étapes simples, il est facile d&#39;exécuter une synchronisation entre Adobe Marketo Engage et la CRM Veeva.

## Fonctionnement de la synchronisation {#how-the-sync-works}

Les Marketo Engage se synchronisent avec Veeva CRM toute la journée, tous les jours. Chaque synchronisation prend un certain temps, s’interrompt pendant 5 minutes, puis recommence.

>[!NOTE]
>
>La toute première synchronisation peut prendre des heures, voire des jours, car Marketo Engage copie la totalité de la base de données depuis Veeva. Ensuite, chaque synchronisation prend généralement des minutes (parfois des secondes) et synchronise uniquement les données qui ont changé.

![](assets/understanding-the-veeva-sync-1.png)

La synchronisation entre Veeva et Marketo Engage est bidirectionnelle uniquement pour les champs Contact de l’objet de compte Personne. Dans ce cas, chaque fois que vous apportez des modifications à Veeva ou à Marketo Engage, vos mises à jour seront répercutées dans les deux systèmes. Toutes les autres synchronisations sont de Veeva à Marketo Engage uniquement. Cliquez sur les liens ci-dessous pour plus de détails sur chacun d’eux.

## Ce qui est synchronisé entre Marketo Engage et Veeva {#what-is-synced-between-marketo-engage-and-veeva}

* [Comptes de personne](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Utilisateurs et utilisatrices
* [Appeler et appeler des objets clés](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Objets personnalisés](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## Informations à connaître {#things-to-know}

* La variable [informations d’identification que vous saisissez en Marketo Engage pour Veeva](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

* Veeva CRM est basé sur force.com et le Marketo Engage d’expérience riche de la plateforme est hérité dans cette synchronisation.

* La Gestion de la relation client Veeva affiche : prospect, contact, comptes, comptes, opportunités, campagne et activité. Toutefois, ils ne sont pas pris en charge dans la synchronisation avec Marketo Engage.
