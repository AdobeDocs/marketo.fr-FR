---
unique-page-id: 2953467
description: Synchronisation SFDC - Synchronisation des opportunités - Documents Marketo - Documentation du produit
title: Synchronisation SFDC - Synchronisation des opportunités
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 6%

---

# Synchronisation SFDC : Synchronisation des opportunités {#sfdc-sync-opportunity-sync}

## Comment les détails des opportunités sont-ils synchronisés entre les deux systèmes ? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La synchronisation est une méthode : de Salesforce à Marketo. Les mises à jour des opportunités dans Salesforce seront synchronisées avec Marketo.

>[!NOTE]
>
>Le [informations d’identification que vous saisissez dans Marketo pour Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

## Puis-je lancer une synchronisation des opportunités ? {#can-i-initiate-an-opportunity-sync}

Non, vous ne pouvez pas. Les modifications apportées à toute opportunité dans Salesforce seront automatiquement synchronisées avec Marketo.

## Marketo prend-il en charge plusieurs devises dans le montant de l’opportunité ? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Non, Marketo ne prend en charge qu’une seule devise. Le montant de l’opportunité sera synchronisé à partir de Salesforce, mais la devise sera [devise par défaut](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) dans votre abonnement Marketo.

## Comment Marketo associe-t-il les opportunités et les contacts ? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo associe des opportunités et des contacts à l’aide de [Rôles de contact d’opportunité](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). Les opportunités sans rôle de contact affecté seront synchronisées avec Marketo, mais n’appartiendront à personne. Par exemple, la personne ne remplit pas les critères du filtre Avec opportunité .

## Comment puis-je voir toutes les opportunités d&#39;une personne ? {#how-can-i-see-all-the-opportunities-of-a-person}

Vous pouvez afficher une liste des opportunités dans la variable **Informations sur l’opportunité** dans le [Détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) page.

## Quels sont les déclencheurs/filtres liés à une opportunité ? {#what-are-the-triggers-filters-related-to-opportunity}

Déclencheurs :

* Ajout à l’opportunité
* Supprimé de l&#39;opportunité
* Mise à jour de l&#39;opportunité

Filtres:

* A une opportunité
* Mise à jour/non de l’opportunité
* A été ajouté à Opportunity/Not a été ajouté à Opportunity
* A été supprimé de l’opportunité/n’a pas été supprimé de l’opportunité
* Montant total de l&#39;opportunité
* Nombre d&#39;opportunités
* Total du chiffre d&#39;affaires souhaité de l&#39;opportunité

>[!TIP]
>
>Vérifiez les contraintes sur les filtres et les déclencheurs. Beaucoup de détails sympas là dedans.
>
>Créez simplement un nouveau champ dans l’objet d’opportunité dans Salesforce et il deviendra automatiquement une contrainte !
