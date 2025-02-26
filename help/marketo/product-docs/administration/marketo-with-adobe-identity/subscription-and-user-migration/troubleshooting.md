---
description: Guide de dépannage d’Adobe IMS - Documents Marketo - Documentation du produit
title: Guide de dépannage d’Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
source-git-commit: eccebb8352c56770dea5af9395c8bc83a08525dd
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Guide de dépannage d’Adobe IMS {#adobe-ims-troubleshooting-guide}

Au cours du processus de migration des utilisateurs IMS, un utilisateur Adobe est créé pour chaque utilisateur Marketo Engage en cours de migration. Parfois, elle n’est pas créée (pour diverses raisons, liées à l’enregistrement de l’utilisateur dans Active Directory ou à des problèmes liés à l’adresse e-mail). Lorsque cela se produit, l’administrateur Marketo Engage voit les raisons dans le champ statut de migration de l’utilisateur sur la console d’auto-migration. Découvrez comment résoudre divers problèmes de création d’utilisateurs Adobe ci-dessous.

## Message d&#39;erreur {#error-messages}

* <a href="#not-in-directory">Pas dans le répertoire</a>
* <a href="#gmail-invalid-character">Caractère Non Valide De Gmail</a>
* <a href="#inactive-user"> Utilisateur inactif </a>
* <a href="#not-in-domain">Pas dans le domaine</a>
* <a href="#create-failure">Échec de la création</a>
* <a href="#type2e-user-failure">Échec de l’utilisateur Type2e</a>



<table>
<thead>
  <tr>
    <th style="width:20%">Message d'erreur</th>
    <th style="width:40%">Cause principale</th>
    <th style="width:40%">Résolutions</th>
  </tr>
  </thead>
<tbody>
  <tr>
    <td><i><a id="not-in-directory">Pas dans le répertoire</a></i></td>
    <td>L'utilisateur n'existe pas dans Active Directory (AD). Pour les organisations avec authentification unique dont la synchronisation des comptes publicitaires est activée, la création d’utilisateurs n’est autorisée que par le biais du fournisseur d’identité (IdP). Par conséquent, l’utilisateur n’a pas pu être ajouté via Admin Console lors de la migration de l’utilisateur.</td>
    <td>Migrer : l’utilisateur doit être ajouté à Active Directory avec les autorisations appropriées. L’administrateur Marketo doit exécuter à nouveau la migration des utilisateurs pour cet utilisateur à partir de la console de migration. 
    <br>Ne pas migrer - l’administrateur Marketo doit ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez dessus pour terminer le processus de migration des utilisateurs.</td>
  </tr>
  <tr>
    <td><i><a id="gmail-invalid-character">Caractère non valide dans Gmail</a></i></td>
    <td>Selon la politique de sécurité d’Adobe, « . » Les signes « + » et « + » ne sont pas autorisés dans une adresse e-mail du domaine Gmail uniquement  
    <br>Les deux caractères spéciaux sont autorisés dans une adresse e-mail n’appartenant pas au domaine Gmail. </td>
    <td>Migrer : l’adresse e-mail doit être mise à jour dans Marketo Engage pour se conformer à la politique de sécurité d’Adobe. L’administrateur Marketo doit exécuter à nouveau la migration des utilisateurs pour cet utilisateur à partir de la console de migration.<br>Ne pas migrer - l’administrateur Marketo doit ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez dessus pour terminer le processus de migration des utilisateurs.</td>
  </tr>
  <tr>
    <td><i><a id="inactive-user">Utilisateur inactif</a></i></td>
    <td>La synchronisation des annonces est activée et le compte fédéré de l’utilisateur existe mais a le statut inactif/désactivé.</td>
    <td>Migrer - Le statut et les autorisations appropriées de l’utilisateur doivent être restaurés. L’administrateur Marketo doit exécuter à nouveau la migration des utilisateurs pour cet utilisateur à partir de la console de migration.
    <br>Ne pas migrer - l’administrateur Marketo doit ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez dessus pour terminer le processus de migration des utilisateurs.</td>
  </tr>
  <tr>
    <td><i><a id="not-in-domain">Pas dans le domaine</a></i></td>
    <td>L’application des domaines est activée dans Admin Console, mais le domaine de l’adresse e-mail de l’utilisateur n’est pas l’un des domaines autorisés. 
    <br>Les politiques d’application de domaine sont définies au niveau du répertoire.</td>
    <td>Migrer : l’adresse e-mail doit être mise à jour dans Marketo Engage pour se conformer à la politique d’application du domaine, ou l’administrateur système peut <a href="https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories"> 
    Déplacez le domaine vers un autre répertoire désactivé par l'application de domaine (DE) </a>ou <a href="https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html">créez un nouveau répertoire</a>, qui n'est pas sous la stratégie DE. L’administrateur Marketo doit exécuter à nouveau la migration des utilisateurs pour cet utilisateur à partir de la console de migration. <br>Ne pas migrer - l’administrateur Marketo doit ignorer l’utilisateur dans la console de migration. Le bouton « Migration terminée » s’affiche lorsque la migration ou l’omission prend en compte tous les utilisateurs. Cliquez dessus pour terminer le processus de migration des utilisateurs.</td>
  </tr>
  <tr>
    <td><i><a id="create-failure">Échec de la création</a></i></td>
    <td>Diverses raisons sur le serveur principal.</td>
    <td>Veuillez soumettre un dossier d’assistance.</td>
  </tr>
  <tr>
    <td><i><a id="type2e-user-failure">Échec de l’utilisateur Type2e</a></i></td>
    <td>Diverses raisons sur le serveur principal.</td>
    <td>Veuillez soumettre un dossier d’assistance.</td>
  </tr>
</tbody>
</table>
