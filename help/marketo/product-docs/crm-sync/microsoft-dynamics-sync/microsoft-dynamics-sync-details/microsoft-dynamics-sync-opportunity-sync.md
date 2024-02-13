---
unique-page-id: 3571844
description: Synchronisation Microsoft Dynamics - Synchronisation des opportunités - Documents Marketo - Documentation du produit
title: Synchronisation Microsoft Dynamics - Synchronisation des opportunités
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 9a130e0b2ec84b638adf37188b65b565b090fe1b
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Synchronisation Microsoft Dynamics : synchronisation des opportunités {#microsoft-dynamics-sync-opportunity-sync}

Marketo Engage à la synchronisation Dynamics est très puissant. Voici tous les détails de la synchronisation des opportunités.

## Comment les détails des opportunités sont-ils synchronisés entre les deux systèmes ? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La synchronisation des opportunités est un moyen : Dynamics vers Marketo. Si vous apportez des modifications à une opportunité dans Dynamics, votre mise à jour sera répercutée dans Marketo.

## Puis-je créer une opportunité dans Dynamics à l’aide de Marketo ? {#can-i-create-an-opportunity-in-dynamics-using-marketo}

Non, vous devez créer l’opportunité dans Dynamics et elle sera automatiquement synchronisée avec Marketo.

## Quels champs seront synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} lors de la configuration.

## Comment un compte/contact est-il associé à une opportunité ? {#how-is-an-account-contact-associated-with-an-opportunity}

Le contact/compte peut être associé à l’opportunité de deux manières :

* Lors de la création d’une opportunité, les champs Contact (champ de recherche sur le formulaire à contacter) et/ou Compte (champ de recherche sur le formulaire à mettre en compte) peuvent être définis. Dans les deux cas, ces valeurs sont stockées dans le champ Client potentiel (customerid) de Dynamics. Ce champ ne s’affiche pas dans le formulaire d’opportunité, mais il peut être ajouté à partir des paramètres. Ce champ ne peut contenir que 1 valeur, contact ou compte. Marketo effectue les opérations suivantes :

   * Si la valeur de contact est définie et que le compte est vide, Marketo crée une `opportunitycontactrole` et fixe le compte sur l&#39;opportunité pour le compte du contact. Si le contact n&#39;a pas de compte, ce champ est vide.
   * Si la valeur du compte est définie et que le contact est vide, Marketo définit uniquement le compte sur l’opportunité d’accès à ce compte.
   * Si les deux valeurs sont définies, Dynamics sélectionne le compte comme valeur de customerid, de sorte que le comportement serait le même que ci-dessus.


* Grâce aux parties prenantes : Dynamics utilise des connexions pour connecter l’opportunité de contacter les parties prenantes à partir de la page de création d’opportunité. Pour ce faire, nous allons créer une `opportunitycontactrole` enregistrement pour chaque nouvelle partie prenante.
