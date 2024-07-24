---
description: Vérification des courriers électroniques - Documents Marketo - Documentation du produit
title: Vérification des emails
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: 7b64e6e9bbd282b1e27f4c9c862df07642e9a35b
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Vérification des emails {#email-verification}

Les abonnements à Adobe Marketo Engage requièrent que tous les utilisateurs non-API uniquement, y compris les administrateurs de Marketo Engage, vérifient leur adresse électronique.

## Pourquoi Cette Fonctionnalité A Été Introduite {#why-this-feature-was-introduced}

Marketo Engage continue le déploiement de la vérification des courriers électroniques en vue de la migration des clients vers Adobe Business Platform, y compris la migration des utilisateurs vers les identifiants d’Adobe. Cette fonctionnalité renforce la sécurité des comptes d’utilisateurs de Marketo Engage existants. Pour s’assurer qu’un utilisateur Marketo Engage est associé à l’Adobe ID approprié, les utilisateurs Marketo Engage existants doivent vérifier leur adresse électronique. Un utilisateur Marketo Engage doit disposer d’une adresse électronique vérifiée pour effectuer la migration vers Adobe ID. Si un utilisateur Marketo Engage ne vérifie pas son adresse électronique, il ne peut pas être migré vers un Adobe ID et n’aura plus accès à un abonnement Marketo une fois la migration de l’utilisateur terminée.

## Invitation d’utilisateur {#user-invite}

Lorsqu’un administrateur invite un utilisateur, celui-ci est automatiquement vérifié lorsqu’il clique sur le lien d’invitation.

>[!IMPORTANT]
>
>L’exception à cette règle est : _dans un abonnement SSO uniquement_, les administrateurs recevront une nouvelle invitation d’utilisateur, mais pas les utilisateurs non-administrateurs. Les utilisateurs qui ne sont pas administrateurs doivent toujours passer par le processus de vérification des emails pour garantir la migration de leurs enregistrements. Les utilisateurs peuvent envoyer eux-mêmes le lien de vérification par e-mail en cliquant sur l’icône de leur profil, en accédant à **Mon compte** > **Paramètres du compte** et en cliquant sur **Renvoyer la vérification**.

![](assets/email-verification-1.png)

## Vérification de l’e-mail {#verification-email}

Les utilisateurs recevront l’e-mail ci-dessous lorsque la vérification de l’e-mail est activée pour un abonnement, ou s’il est déclenché par un administrateur/utilisateur.

Une session d’utilisateur active est requise pour la réussite de la vérification d’email. L’utilisateur doit d’abord se connecter à son abonnement Marketo à l’aide de son URL de fournisseur d’identité (IdP). Une fois une session établie, ils _puis_ cliquent sur le lien **Vérifier l’adresse électronique** dans le courrier électronique.

![](assets/email-verification-2.png)

>[!TIP]
>
>Pour renvoyer un courrier électronique de vérification à un utilisateur non vérifié, sélectionnez simplement son enregistrement et cliquez sur le bouton **[!UICONTROL Vérifier l’adresse électronique]**.

## Modification d’une adresse électronique {#changing-an-email-address}

Lorsque l’adresse électronique d’un utilisateur est modifiée, elle n’est plus vérifiée. Un email leur sera envoyé pour leur permettre de vérifier à nouveau. Les utilisateurs peuvent renvoyer manuellement cet email en cliquant sur **[!UICONTROL Renvoyer la vérification]**.

![](assets/email-verification-3.png)

![](assets/email-verification-4.png)

## Utilisateurs et rôles {#users-and-roles}

Dans **[!UICONTROL Admin]** > **[!UICONTROL Utilisateurs et rôles]**, la colonne État du courrier électronique affiche l’état de vérification de chaque utilisateur.

![](assets/email-verification-5.png)

## Plusieurs ID de connexion utilisateur {#multiple-user-login-ids}

Un seul compte utilisateur peut être associé à une seule adresse électronique. Si plusieurs comptes utilisateur sont associés à une seule adresse électronique, Marketo Engage exige que le conflit soit résolu et affiche toutes les connexions utilisateur associées à l’adresse électronique, ainsi que trois options de résolution :

* Utiliser le courrier électronique actuel pour l’ID de connexion de l’utilisateur actuel
* Utiliser un nouveau courrier électronique pour l’ID de connexion de l’utilisateur actuel
* Retarder la décision jusqu’à la prochaine connexion

  ![](assets/email-verification-6.png)

>[!NOTE]
>
>Bien qu’un compte utilisateur doive être associé à une seule adresse, un compte utilisateur peut être utilisé pour de nombreux abonnements via un ID universel.
