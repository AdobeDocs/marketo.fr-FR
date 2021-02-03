---
unique-page-id: 2953467
description: Synchronisation SFDC - Synchronisation des opportunités - Documents marketing - Documentation du produit
title: Synchronisation SFDC - Synchronisation des opportunités
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# Synchronisation SFDC : Synchronisation des opportunités {#sfdc-sync-opportunity-sync}

## Comment les détails des opportunités sont-ils synchronisés entre les deux systèmes ? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La synchronisation est un moyen : de Salesforce à Marketo. Les mises à jour des opportunités dans Salesforce seront synchronisées avec Marketo.

>[!NOTE]
>
>Les [informations d&#39;identification que vous saisissez dans Marketo pour Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

## Puis-je lancer une synchronisation des opportunités ? {#can-i-initiate-an-opportunity-sync}

Non, vous ne pouvez pas. Les modifications apportées à toute opportunité dans Salesforce seront automatiquement synchronisées sur Marketo.

## Le marketing prend-il en charge plusieurs devises dans le montant de l&#39;opportunité ? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Non, Marketo ne prend en charge qu&#39;une seule devise. Le montant d&#39;opportunité sera synchronisé à partir de Salesforce mais la devise sera la [devise par défaut](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) dans votre abonnement Marketo.

## Comment Marketing associe-t-il les opportunités et les contacts ? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo associe Opportunités et contacts à l&#39;aide de [Rôles de contact Opportunité](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). Les opportunités sans aucun rôle de contact affecté seront synchronisées avec Marketo, mais n’appartiendront à personne. Par exemple, la personne ne sera pas admissible au filtre Avec opportunité.

## Comment puis-je voir toutes les opportunités d&#39;une personne ? {#how-can-i-see-all-the-opportunities-of-a-person}

Vous pouvez vue une liste d&#39;opportunités dans l&#39;onglet **Informations sur l&#39;opportunité** de la page [Détails sur la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Quels sont les déclencheurs/filtres liés à une opportunité ? {#what-are-the-triggers-filters-related-to-opportunity}

Déclencheurs :

* Ajouté à l&#39;opportunité
* Retiré de l&#39;opportunité
* L&#39;opportunité est mise à jour

Filtres :

* A une opportunité
* Opportunité mise à jour/Aucune opportunité mise à jour
* A été Ajouté à l&#39;opportunité/Non Ajouté à l&#39;opportunité
* A été supprimé de l&#39;opportunité/N&#39;a pas été supprimé de l&#39;opportunité
* Montant total d&#39;opacité
* Nombre d’options
* Total des recettes prévues de l&#39;Optimisation

>[!TIP]
>
>Vérifiez les contraintes sur les filtres et les déclencheurs. Beaucoup de détails sympas là-dedans.
>
>Il vous suffit de créer un nouveau champ dans l&#39;objet opportunité de Salesforce et il deviendra automatiquement une contrainte !
