---
description: Présentation de la synchronisation  [!DNL Veeva]  CRM - Documentation de Marketo - Documentation du produit
title: Comprendre la synchronisation  [!DNL Veeva]  CRM
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Comprendre la synchronisation du CRM [!DNL Veeva] {#understanding-the-veeva-crm-sync}

En quelques étapes simples, il est facile d’exécuter une synchronisation entre Adobe Marketo Engage et le CRM [!DNL Veeva].

## Fonctionnement de la synchronisation {#how-the-sync-works}

Marketo Engage se synchronise avec [!DNL Veeva] CRM toute la journée, tous les jours. Chaque synchronisation prend du temps, s’interrompt pendant 5 minutes, puis redémarre.

>[!NOTE]
>
>La toute première synchronisation peut prendre des heures, voire des jours, car Marketo Engage copie l’intégralité de la base de données depuis [!DNL Veeva]. Ensuite, chaque synchronisation prend généralement quelques minutes (parfois quelques secondes) et synchronise uniquement les données qui ont changé.

![](assets/understanding-the-veeva-sync-1.png)

La synchronisation entre [!DNL Veeva] et Marketo Engage est bidirectionnelle uniquement pour les champs Contact sur l’objet Compte de personne. Dans ces cas, chaque fois que vous apportez des modifications à [!DNL Veeva] ou à Marketo Engage, vos mises à jour sont répercutées sur les deux systèmes. Toutes les autres synchronisations vont de [!DNL Veeva] à Marketo Engage uniquement. Cliquez sur les liens ci-dessous pour plus de détails sur chacun d’eux.

## Éléments synchronisés entre Marketo Engage et [!DNL Veeva] {#what-is-synced-between-marketo-engage-and-veeva}

* [Comptes de personne](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Utilisateurs et utilisatrices
* [Appeler et appeler des objets de clé](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Objets personnalisés](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## Informations à connaître {#things-to-know}

* Les [&#x200B; informations d’identification que vous saisissez dans Marketo Engage pour  [!DNL Veeva]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

* [!DNL Veeva] CRM est basé sur force.com et la riche expérience de Marketo Engage avec la plateforme est héritée dans cette synchronisation.

* Veeva CRM affiche : Lead, Contact, Comptes, Comptes professionnels, Opportunité, Campagne et Activité. Toutefois, ils ne sont pas pris en charge dans la synchronisation avec Marketo Engage.
