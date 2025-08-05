---
unique-page-id: 3571844
description: Synchronisation de Microsoft Dynamics - Synchronisation des opportunités - Documents Marketo - Documentation du produit
title: Synchronisation de Microsoft Dynamics - Synchronisation des opportunités
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Synchronisation des [!DNL Microsoft Dynamics] : synchronisation des opportunités {#microsoft-dynamics-sync-opportunity-sync}

La synchronisation de Marketo vers [!DNL Dynamics] est très puissante. Voici tous les détails de la synchronisation des opportunités :

## Comment les détails des opportunités sont-ils synchronisés entre les deux systèmes ? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

La synchronisation des opportunités est une méthode : [!DNL Dynamics] à Marketo. Si vous apportez des modifications à une opportunité dans [!DNL Dynamics], votre mise à jour sera répercutée dans Marketo.

## Puis-je créer une opportunité dans [!DNL Dynamics] à l’aide de Marketo ? {#can-i-create-an-opportunity-in-dynamics-using-marketo}

Non, vous devez créer l’opportunité dans [!DNL Dynamics]. Elle sera automatiquement synchronisée dans Marketo.

## Quels champs vont être synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} lors de la configuration.

## Comment un compte/contact est-il associé à une opportunité ? {#how-is-an-account-contact-associated-with-an-opportunity}

Le contact/compte peut être associé à l’opportunité de deux manières :

* Lors de la création d’une opportunité, le Contact (champ de recherche du formulaire à contacter) et/ou le Compte (champ de recherche du formulaire à compte) peuvent être définis. Dans les deux cas, ces valeurs sont stockées dans le champ Client potentiel (customerid) de Dynamics. Ce champ n’apparaît pas dans le formulaire d’opportunité, mais peut être ajouté à partir des paramètres. Ce champ ne peut contenir qu’une seule valeur, contact ou compte. Marketo effectue les opérations suivantes :

   * Si la valeur du contact est définie et que le compte n’est pas renseigné, Marketo crée un `opportunitycontactrole` et définit le compte sur l’opportunité pour le compte du contact. Si le contact n’a pas de compte, ce champ reste vide.
   * Si la valeur du compte est définie et que le contact n’est pas renseigné, Marketo définit uniquement le compte sur l’opportunité de ce compte.
   * Si les deux valeurs sont définies, Dynamics sélectionne le compte comme valeur pour l’ID client, de sorte que le comportement soit le même que ci-dessus.

* Via les parties prenantes : Dynamics utilise des connexions pour connecter l’opportunité à contacter via les parties prenantes à partir de la page de création d’opportunité. Pour ce faire, nous créerons un dossier `opportunitycontactrole` pour chaque nouvelle partie prenante.
