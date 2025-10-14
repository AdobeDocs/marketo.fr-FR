---
unique-page-id: 2953467
description: Synchronisation de SFDC - Synchronisation des opportunités - Documents Marketo - Documentation du produit
title: Synchronisation de SFDC - Synchronisation des opportunités
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 8%

---

# Synchronisation SFDC : synchronisation d’opportunité {#sfdc-sync-opportunity-sync}

## Comment les détails des opportunités sont-ils synchronisés entre les deux systèmes ? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La synchronisation fonctionne dans un sens : de [!DNL Salesforce] à Marketo. Les mises à jour des opportunités dans [!DNL Salesforce] seront synchronisées avec Marketo.

>[!NOTE]
>
>Les [&#x200B; informations d’identification que vous saisissez dans Marketo pour  [!DNL Salesforce]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) sont utilisées pour synchroniser les données. Seules les données auxquelles ces informations d’identification ont accès seront incluses.

## Puis-je lancer une synchronisation d’opportunité ? {#can-i-initiate-an-opportunity-sync}

Non, tu ne peux pas. Les modifications apportées à n’importe quelle opportunité dans [!DNL Salesforce] seront automatiquement synchronisées avec Marketo.

## Marketo Le montant de l’opportunité prend-il en charge plusieurs devises ? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Non, Marketo ne prend en charge qu’une seule devise. Le montant de l’opportunité sera synchronisé à partir de [!DNL Salesforce], mais la devise sera la [&#x200B; devise par défaut](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) dans votre abonnement Marketo.

## Comment Marketo associe-t-il les opportunités et les contacts ? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo associe les opportunités et les contacts à l’aide des [rôles de contact d’opportunité](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm){target="_blank"}. Les opportunités sans aucun rôle de contact affecté seront synchronisées avec Marketo, mais n’appartiendront à personne. Par exemple, la personne ne remplit pas les critères du filtre A une opportunité .

## Comment puis-je voir toutes les opportunités d’une personne ? {#how-can-i-see-all-the-opportunities-of-a-person}

Vous pouvez afficher une liste d’opportunités sous l’onglet **[!UICONTROL Informations sur l’opportunité]** de la page [Détails de la personne](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Quels sont les déclencheurs/filtres liés à l’opportunité ? {#what-are-the-triggers-filters-related-to-opportunity}

Déclencheurs :

* Ajouté à l’opportunité
* Supprimé de l&#39;opportunité
* Mise à jour de l’opportunité

Filtres:

* A une opportunité
* L’opportunité a été mise à jour/non l’opportunité a été mise à jour
* A été ajouté à l’opportunité/Non a été ajouté à l’opportunité
* A été supprimé de l’opportunité/Non a été supprimé de l’opportunité
* Montant total de l&#39;opportunité
* Nombre d&#39;opportunités
* Total du chiffre d&#39;affaires souhaité de l&#39;opportunité

>[!TIP]
>
>Consultez les contraintes sur les filtres et les déclencheurs. Il y a plein de détails sympas.
>
>Créez simplement un nouveau champ dans l’objet d’opportunité en [!DNL Salesforce] et il deviendra automatiquement une contrainte.
