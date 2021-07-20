---
unique-page-id: 2360356
description: Ajout d’une authentification unique à un portail - Documents Marketo - Documentation du produit
title: Ajout d’une authentification unique à un portail
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
source-git-commit: e4d581ab258a875747a6d5323764e8b4a3949cba
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# Ajout d’une authentification unique à un portail {#add-single-sign-on-to-a-portal}

Si vous disposez d’un service d’annuaire qui authentifie les utilisateurs, vous pouvez autoriser l’authentification unique (SSO) dans Marketo. Cette fonctionnalité est prise en charge à l’aide du langage SAML (Security Assertion Markup Language) version 2.0 et ultérieure.

Marketo fonctionne comme fournisseur de services SAML et dépend d’un fournisseur d’identité externe (IdP) pour authentifier les utilisateurs.

Une fois l’authentification unique activée, l’IdP peut valider les informations d’identification d’un utilisateur. Lorsqu’un utilisateur souhaite utiliser le logiciel Marketo, l’IdP envoie alors un message SAML signé à Marketo, en tant que SP. Ce message garantit à Marketo que l’utilisateur est autorisé à utiliser le logiciel Marketo.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Êtes-vous un utilisateur de Microsoft Azure ? Consultez leur [tutoriel sur l’intégration](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/).

## Envoi de la requête {#how-to-send-the-request}

* Envoyez la requête SSO, qui est une réponse SAML, à `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Comme URL d’audience du SP. Utiliser `http://saml.marketo.com/sp`
* Si vous utilisez l’attribut SPNameQualifier , définissez l’élément NameID pour le sujet sur `http://saml.marketo.com/sp`
* Si vous fédérez plusieurs abonnements Marketo au même fournisseur d’authentification unique, vous pouvez utiliser des url SP uniques pour chaque sous-chaîne Marketo au format `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo ne prend en charge que les identifiants initiés par le fournisseur d’identité (également appelés IdP), dans lesquels l’utilisateur lance d’abord la page de connexion Idp, s’authentifie, puis accède à Mon Marketo.

## Remarques supplémentaires {#additional-notes}

* **Synchronisation**  : pour un nouvel utilisateur, un délai d’environ 10 minutes est nécessaire avant le traitement d’une demande d’authentification unique initiale.
* **Mise en service des utilisateurs**  : les utilisateurs sont configurés manuellement par Marketo.
* **Autorisation**  : les autorisations utilisateur sont conservées dans Marketo.
* **Prise en charge OAuth**  : Marketo ne prend actuellement pas en charge OAuth.
* **Propagation automatique des utilisateurs**  : également appelée &quot;Simplement dans l’approvisionnement temporel&quot;, c’est lorsque la première connexion SAML d’un utilisateur est capable de créer l’utilisateur dans l’application web à laquelle il accède (par exemple, Marketo) et qu’aucune action d’administration manuelle n’est requise. Pour l’instant, Marketo ne le prend pas en charge.
* **Chiffrement**  : Marketo ne prend actuellement pas en charge le chiffrement.

>[!NOTE]
>
>Avant de commencer, vous devez disposer de votre certificat de fournisseur d’identité au format X.509 et dans l’extension .crt, .der ou .cer.

## Mise à jour des paramètres SAML {#update-saml-settings}

SSO est désactivé par défaut. Pour activer SAML et le configurer, procédez comme suit.

1. Accédez à **Admin** et cliquez sur **Connexion unique**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Si vous ne voyez pas **Connexion unique** sous **Admin**, contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Sous la section **Paramètres SAML** , cliquez sur **Modifier**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Remplacez **Connexion unique SAML** par **Activé**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Saisissez votre **ID d’émetteur**, **ID d’entité**, sélectionnez l’**emplacement de l’ID utilisateur**, puis cliquez sur **Parcourir**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Sélectionnez votre fichier **Certificat du fournisseur d’identité** .

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Mettre à jour les paramètres de la page de redirection {#update-redirect-page-settings}

1. Dans la section **Rediriger les pages**, cliquez sur **Modifier**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Les clients qui utilisent un ID universel avec SSO doivent saisir l’URL de connexion du fournisseur d’identité dans le champ **URL de connexion** .

1. Saisissez une **URL de déconnexion**. Il s’agit de l’URL vers laquelle l’utilisateur doit être redirigé lorsqu’il se déconnecte de Marketo.

   ![](assets/eight.png)

1. Saisissez une **URL d’erreur**. Il s’agit de l’URL vers laquelle l’utilisateur doit être redirigé en cas d’échec de la connexion à Marketo. Cliquez sur **Enregistrer**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Ces deux pages doivent être disponibles publiquement.

>[!MORELIKETHIS]
>
>* [Utilisation d’un ID universel pour la connexion à l’abonnement](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
* [Limiter la connexion de l&#39;utilisateur aux connexions par signature unique](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
* [Invitation d’utilisateurs Marketo à deux instances avec un ID universel](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

