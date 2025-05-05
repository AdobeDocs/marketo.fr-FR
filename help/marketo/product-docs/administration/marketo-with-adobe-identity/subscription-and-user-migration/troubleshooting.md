---
description: Guide de dépannage de la migration des utilisateurs Adobe IMS - Documents Marketo - Documentation du produit
title: Guide de dépannage de la migration des utilisateurs Adobe IMS
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: b3bc6a7ec14a513e4b294852d066f9e3d0f74ef8
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 1%

---

# Guide de dépannage de la migration des utilisateurs Adobe IMS {#adobe-ims-user-migration-troubleshooting-guide}

Lors du processus de migration des utilisateurs IMS, un utilisateur Adobe est créé pour chaque utilisateur Marketo Engage migré (à moins qu’il n’existe déjà avec la même adresse e-mail). Parfois, il n’est pas créé, ce qui peut être attribué à l’enregistrement de l’utilisateur dans Active Directory ou à des problèmes liés à l’adresse e-mail.

Cet article, destiné aux utilisateurs qui effectuent des migrations automatiques, répertorie chaque message d’erreur que vous pouvez voir dans le champ statut de la console de migration automatique.

>[!NOTE]
>
>Les erreurs liées au répertoire/domaine peuvent être déclenchées par une autre organisation ou un autre Admin Console où une approbation de répertoire est configurée ou où le domaine a été demandé.

## Message d&#39;erreur {#error-messages}

Tout d’abord, déterminez si l’utilisateur doit être migré ou non, car cela affectera les étapes de résolution à suivre.

Utilisez la section « Sur cette page » sur la droite pour accéder directement à une erreur spécifique.

### Caractère non valide dans Gmail {#gmail-invalid-character}

**Cause principale** : conformément à la politique de sécurité d’Adobe, les caractères `.` et `+` ne sont pas autorisés dans une adresse e-mail Gmail. Les deux caractères sont autorisés dans les adresses e-mail non Gmail.

**Résolutions** :

_Si l’utilisateur doit être migré_ - L’adresse e-mail doit être mise à jour dans Marketo Engage pour se conformer à la politique de sécurité d’Adobe et revérifiée. L’administrateur Marketo pour réexécuter ensuite la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

_Si l’utilisateur n’a **besoin**&#x200B;d’être migré_ - L’administrateur Marketo Engage peut ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

### L&#39;utilisateur n&#39;est pas dans le répertoire {#user-not-in-directory}

**Cause principale** : l’utilisateur n’existe pas dans Active Directory (AD). Pour les organisations avec authentification unique dont la synchronisation des adresses AD est activée, la création d’utilisateurs n’est autorisée que par le biais du fournisseur d’identité (IdP). Par conséquent, l’utilisateur n’a pas pu être ajouté via Admin Console lors de la migration de l’utilisateur.

**Résolutions** :

_Si l’utilisateur doit être migré_ - L’utilisateur doit être ajouté à Active Directory avec les autorisations appropriées par un administrateur système. L’administrateur Marketo Engage pour réexécuter ensuite la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

_Si l’utilisateur n’a **besoin**&#x200B;d’être migré_ - L’administrateur Marketo Engage peut ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

### Utilisateur inactif {#inactive-user}

**Cause principale** : la synchronisation des publicités est activée et le compte fédéré de l’utilisateur existe mais a le statut inactif/désactivé.

**Résolutions** :

_Si l’utilisateur doit être migré_ - Le statut de l’utilisateur et les autorisations appropriées doivent être restaurés par un administrateur système. L’administrateur Marketo Engage pour réexécuter ensuite la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

_Si l’utilisateur n’a **besoin**&#x200B;d’être migré_ - L’administrateur Marketo Engage peut ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

### Domaine non valide {#invalid-domain}

**Cause principale** : l’application de domaine est activée dans Admin Console. Cependant, le domaine de l’adresse e-mail de l’utilisateur n’est pas l’un des domaines autorisés ou le domaine a été demandé dans une autre organisation ou Admin Console.

**Résolutions** :

_Si l’utilisateur doit faire l’objet d’une migration_ (et si l’application du domaine est activée dans l’organisation en migration) : l’adresse e-mail doit être mise à jour dans Marketo Engage pour respecter la politique Application du domaine (DE). L’administrateur système peut également [déplacer le domaine](https://helpx.adobe.com/fr/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} vers un autre répertoire désactivé par l’application de domaine (DE) ou [créer un nouveau répertoire](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"} qui n’est pas soumis à la stratégie DE. L’administrateur Marketo Engage pour réexécuter ensuite la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

_Si l’utilisateur doit faire l’objet d’une migration_ (et si l’application du domaine est activée dans une autre organisation), un administrateur système de l’organisation dans laquelle le domaine a été demandé doit ajouter l’adresse électronique de l’utilisateur à la liste des exceptions. L’administrateur Marketo Engage pour réexécuter ensuite la migration des utilisateurs pour cet utilisateur à partir de la console de migration.

_Si l’utilisateur n’a **besoin**&#x200B;d’être migré_ - L’administrateur Marketo Engage peut ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez sur le bouton pour terminer le processus de migration des utilisateurs.

### Échec de la création de l’utilisateur {#user-creation-failed}

[Voir ci-dessous](#failed)

### Échec de Type2E {#type2e-failure}

[Voir ci-dessous](#failed)

### Échec de l&#39;autorisation Marketo {#marketo-entitlement-failed}

[Voir ci-dessous](#failed)

### Échec de la migration Pendo {#pendo-migration-failed}

[Voir ci-dessous](#failed)

### Échec de la migration des données utilisateur {#user-data-migration-failed}

[Voir ci-dessous](#failed)

### Échec de la synchronisation des données du produit {#product-data-sync-failed}

[Voir ci-dessous](#failed)

### Échec du droit d’Adobe {#adobe-entitlement-failed}

[Voir ci-dessous](#failed)

### Échec de la déconnexion de l&#39;utilisateur {#user-sign-out-failed}

[Voir ci-dessous](#failed)

### Échec de la création d’Adobe ID {#adobe-id-creation-failed}

[Voir ci-dessous](#failed)

### Échec {#failed}

**Cause principale** : ces erreurs peuvent être dues à diverses raisons qui se trouvent sur le serveur principal.

**Résolutions** :

Soumettez un dossier de support avec les détails pertinents pour la [Assistance Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
