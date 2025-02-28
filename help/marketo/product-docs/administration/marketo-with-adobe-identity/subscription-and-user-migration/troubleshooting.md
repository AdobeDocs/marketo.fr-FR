---
description: Guide de dépannage d’Adobe IMS - Documents Marketo - Documentation du produit
title: Guide de dépannage d’Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: 2a01045abbc23bce9531c64e3494fb12a9adf1bd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Guide de dépannage d’Adobe IMS {#adobe-ims-troubleshooting-guide}

Au cours du processus de migration des utilisateurs IMS, un utilisateur Adobe est créé pour chaque utilisateur Marketo Engage en cours de migration. Parfois, elle n’est pas créée (pour diverses raisons, liées à l’enregistrement de l’utilisateur dans Active Directory ou à des problèmes liés à l’adresse e-mail). Lorsque cela se produit, l’administrateur Marketo Engage en voit la raison dans le champ du statut de migration de l’utilisateur sur la console d’auto-migration.

## Message d&#39;erreur {#error-messages}

Utilisez la section « Sur cette page » sur la droite pour accéder directement à une erreur spécifique et apprendre à la résoudre.

### Pas dans le répertoire {#not-in-directory}

_Cause principale_ : l’utilisateur n’existe pas dans Active Directory (AD). Pour les organisations avec authentification unique dont la synchronisation des adresses AD est activée, la création d’utilisateurs n’est autorisée que par le biais du fournisseur d’identité (IdP). Par conséquent, l’utilisateur n’a pas pu être ajouté via Admin Console lors de la migration de l’utilisateur.

_Résolutions_ :

Prémigration : demandez à l’administrateur Marketo d’ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

Après la migration : l’utilisateur doit être ajouté à Active Directory avec les autorisations appropriées. L’administrateur Marketo Engage doit ensuite exécuter à nouveau la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

### Caractère non valide dans Gmail {#gmail-invalid-character}

_Cause principale_ : conformément à la politique de sécurité d’Adobe, les caractères `.` et `+` ne sont pas autorisés dans une adresse e-mail Gmail. Les deux caractères sont autorisés dans les adresses e-mail non Gmail.

_Résolutions_ :

Prémigration : demandez à l’administrateur Marketo d’ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

Après la migration : l’adresse e-mail doit être mise à jour dans Marketo Engage pour se conformer à la politique de sécurité d’Adobe. L’administrateur Marketo doit exécuter à nouveau la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

### Utilisateur inactif {#inactive-user}

_Cause principale_ : la synchronisation des publicités est activée et le compte fédéré de l’utilisateur existe mais a le statut inactif/désactivé.

_Résolutions_ :

Prémigration : demandez à l’administrateur Marketo d’ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

Après la migration : le statut et les autorisations appropriées de l’utilisateur doivent être restaurés. L’administrateur Marketo Engage doit ensuite exécuter à nouveau la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

### Pas dans le domaine {#not-in-domain}

_Cause principale_ : l’application des domaines est activée dans Admin Console, mais le domaine de l’adresse e-mail de l’utilisateur n’est pas l’un des domaines autorisés.

_Résolutions_ :

Prémigration : demandez à l’administrateur Marketo d’ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

Après la migration : l’adresse e-mail doit être mise à jour dans Marketo Engage pour se conformer à la politique Application des domaines (DE) . L’administrateur système peut également [déplacer le domaine](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} vers un autre répertoire désactivé par l’application de domaine (DE) ou [créer un nouveau répertoire](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"} qui n’est pas soumis à la stratégie DE. L’administrateur Marketo Engage doit ensuite exécuter à nouveau la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

### Échec de la création {#create-failure}

_Cause principale_ : cette erreur peut être due à diverses raisons liées au serveur principal.

_Résolutions_ :

Prémigration : soumettez un dossier d’assistance pour les utilisateurs [ n’ont pas encore été migrés](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Après la migration : veuillez soumettre un dossier d’assistance pour les personnes [déjà migrées](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.

### Échec de l’utilisateur Type2e {#type2e-user-failure}

_Cause principale_ : cette erreur peut être due à diverses raisons liées au serveur principal.

_Résolutions_ :

Prémigration : soumettez un dossier d’assistance pour les utilisateurs [ n’ont pas encore été migrés](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Après la migration : veuillez soumettre un dossier d’assistance pour les personnes [déjà migrées](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.
