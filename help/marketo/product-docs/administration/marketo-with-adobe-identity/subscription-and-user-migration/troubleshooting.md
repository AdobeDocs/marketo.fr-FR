---
description: Guide de dépannage de la migration des utilisateurs Adobe IMS - Documents Marketo - Documentation du produit
title: Guide de dépannage de la migration des utilisateurs Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e96bc8676a73694ec60f46bb045f2a6ea5d8069c
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Guide de dépannage de la migration des utilisateurs Adobe IMS {#adobe-ims-user-migration-troubleshooting-guide}

Lors du processus de migration des utilisateurs IMS, un utilisateur Adobe est créé pour chaque utilisateur Marketo Engage migré (à moins qu’il n’existe déjà avec la même adresse e-mail). Parfois, il n’est pas créé, ce qui peut être attribué à l’enregistrement de l’utilisateur dans Active Directory ou à des problèmes liés à l’adresse e-mail. Dans ce cas, l’administrateur Marketo Engage en voit la raison dans le champ du statut de migration de l’utilisateur dans la console d’auto-migration.

## Message d&#39;erreur {#error-messages}

Tout d’abord, déterminez si l’utilisateur doit être migré ou non, car cela affectera les étapes de résolution à suivre.

Utilisez la section « Sur cette page » sur la droite pour accéder directement à une erreur spécifique.

### Pas dans le répertoire {#not-in-directory}

**Cause principale** : l’utilisateur n’existe pas dans Active Directory (AD). Pour les organisations avec authentification unique dont la synchronisation des adresses AD est activée, la création d’utilisateurs n’est autorisée que par le biais du fournisseur d’identité (IdP). Par conséquent, l’utilisateur n’a pas pu être ajouté via Admin Console lors de la migration de l’utilisateur.

**Résolutions** :

_Si l’utilisateur n’a pas besoin d’être migré_ - L’administrateur Marketo Engage doit l’ignorer dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

_Si l’utilisateur doit faire l’objet d’une migration_ - L’utilisateur doit être ajouté à Active Directory avec les autorisations appropriées par un administrateur système. L’administrateur Marketo Engage pour réexécuter ensuite la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

### Caractère non valide dans Gmail {#gmail-invalid-character}

**Cause principale** : conformément à la politique de sécurité d’Adobe, les caractères `.` et `+` ne sont pas autorisés dans une adresse e-mail Gmail. Les deux caractères sont autorisés dans les adresses e-mail non Gmail.

**Résolutions** :

_Si l’utilisateur n’a pas besoin d’être migré_ - L’administrateur Marketo Engage doit l’ignorer dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

_Si l’utilisateur doit faire l’objet d’une migration_ - L’adresse e-mail doit être mise à jour dans Marketo Engage pour se conformer à la politique de sécurité d’Adobe et revérifiée. L’administrateur Marketo pour réexécuter ensuite la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

### Utilisateur inactif {#inactive-user}

**Cause principale** : la synchronisation des publicités est activée et le compte fédéré de l’utilisateur existe mais a le statut inactif/désactivé.

**Résolutions** :

_Si l’utilisateur n’a pas besoin d’être migré_ - L’administrateur Marketo Engage doit l’ignorer dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

_Si l’utilisateur doit faire l’objet d’une migration_ - Le statut de l’utilisateur et les autorisations appropriées doivent être restaurés. L’administrateur Marketo Engage pour réexécuter ensuite la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

### Pas dans le domaine {#not-in-domain}

**Cause principale** : l’application des domaines est activée dans Admin Console, mais le domaine de l’adresse e-mail de l’utilisateur n’est pas l’un des domaines autorisés.

**Résolutions** :

_Si l’utilisateur n’a pas besoin d’être migré_ - L’administrateur Marketo Engage doit l’ignorer dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

_Si l’utilisateur doit faire l’objet d’une migration_ - L’adresse e-mail doit être mise à jour dans Marketo Engage pour respecter la politique Application du domaine (DE). L’administrateur système peut également [déplacer le domaine](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} vers un autre répertoire désactivé par l’application de domaine (DE) ou [créer un nouveau répertoire](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"} qui n’est pas soumis à la stratégie DE. L’administrateur Marketo Engage pour réexécuter ensuite la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

### Échec de la création {#create-failure}

**Cause principale** : cette erreur peut être due à diverses raisons liées au serveur principal.

**Résolutions** :

Soumettez un dossier de support avec les détails pertinents pour la [Assistance Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

### Échec de l’utilisateur Type2e {#type2e-user-failure}

**Cause principale** : cette erreur peut être due à diverses raisons liées au serveur principal.

**Résolutions** :

Soumettez un dossier de support avec les détails pertinents pour la [Assistance Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
