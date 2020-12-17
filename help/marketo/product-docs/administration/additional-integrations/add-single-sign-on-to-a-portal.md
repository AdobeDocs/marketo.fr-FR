---
unique-page-id: 2360356
description: Ajouter la connexion unique à un portail - Documents marketing - Documentation du produit
title: Ajouter la connexion unique à un portail
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---


# Ajouter la connexion unique à un portail {#add-single-sign-on-to-a-portal}

Si vous disposez d’un service d’annuaire qui authentifie les utilisateurs, vous pouvez autoriser l’authentification unique (SSO) dans Marketing Cloud. Nous prenons en charge cette fonctionnalité en utilisant le langage SAML (Security Assertion Markup Language) version 2.0 et ultérieure.

Marketo fonctionne en tant que Prestataire SAML (SP) et dépend d&#39;un fournisseur d&#39;identité externe (IdP) pour authentifier les utilisateurs.

Une fois l’authentification unique activée, l’IdP peut valider les informations d’identification d’un utilisateur. Lorsqu’un utilisateur souhaite utiliser le logiciel Marketo, l’IdP envoie alors un message SAML signé à Marketo, agissant en tant que SP. Ce message garantit à Marketo que l’utilisateur est autorisé à utiliser le logiciel Marketo.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>Êtes-vous un utilisateur Microsoft Azure ? Consultez leur [didacticiel d&#39;intégration](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/).

## Comment envoyer la requête {#how-to-send-the-request}

* Envoyer la demande d’authentification unique, qui est une réponse SAML, à `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* En tant qu’URL d’Audience du SP. Utiliser [http://saml.marketo.com/sp](http://saml.marketo.com/sp)
* Si vous utilisez l&#39;attribut SPNameQualifier, définissez l&#39;élément NameID pour Objet sur [http://saml.marketo.com/sp](http://saml.marketo.com/sp)
* Si vous fédérez plusieurs abonnements de marketing au même fournisseur d’authentification unique, vous pouvez utiliser des url SP uniques pour chaque sous- de marketing au format `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo ne prend en charge que les identifiants initiés par le fournisseur d’identité (également appelés IdP-started), dans lesquels l’utilisateur lance d’abord la page de connexion Idp, s’authentifie, puis accède à Mon marketing.

## Notes supplémentaires {#additional-notes}

* **Temps**  de synchronisation : pour un nouvel utilisateur, un délai d’environ 10 minutes est nécessaire avant le traitement d’une demande d’authentification unique initiale.
* **Approvisionnement**  des utilisateurs : les utilisateurs sont configurés manuellement par Marketo.
* **Autorisation**  - Les autorisations d’utilisateur sont conservées dans Marketing Cloud.
* **Prise en charge**  OAuth - Marketo ne prend actuellement pas en charge OAuth.

>[!NOTE]
>
>Avant de commencer, procurez-vous votre certificat de fournisseur d’identité au format X.509 et dans l’extension .crt, .der ou .cer.

## Mettre à jour les paramètres SAML {#update-saml-settings}

La fonction SSO est désactivée par défaut. Suivez ces étapes pour activer SAML et le configurer.

1. Accédez à **Admin **et cliquez sur **Connexion unique**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Si **Connexion unique** n&#39;apparaît pas sous **Admin**, contactez [`[email protected]`](http://mailto:support@marketo.com).

1. Sous la section **Paramètres SAML**, cliquez sur **Modifier**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Remplacez **Connexion unique SAML** par **Activé**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Saisissez votre **ID d’émetteur**, **ID d’entité**, sélectionnez **Emplacement de l’ID d’utilisateur**, puis cliquez sur **Parcourir**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Sélectionnez votre fichier **Certificat du fournisseur d&#39;identité**.

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Mettre à jour les paramètres de page de redirection {#update-redirect-page-settings}

1. Sous la section **Rediriger les pages**, cliquez sur **Modifier**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Les clients qui utilisent un ID universel avec une authentification unique doivent saisir l’URL de connexion du fournisseur d’identité dans le champ **URL de connexion**.

1. Saisissez une **URL de déconnexion**. Il s’agit de l’URL à laquelle l’utilisateur doit être redirigé lorsqu’il se déconnecte de Marketing Cloud.

   ![](assets/eight.png)

1. Saisissez une **URL d’erreur**. Il s’agit de l’URL à laquelle l’utilisateur doit être redirigé en cas d’échec de la connexion à Marketing Cloud. Cliquez sur **Enregistrer**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Ces deux pages doivent être accessibles au public.

