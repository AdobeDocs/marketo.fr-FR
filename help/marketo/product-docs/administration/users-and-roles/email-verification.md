---
description: Vérification par e-mail - Documents Marketo - Documentation du produit
title: Vérification par e-mail
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 1%

---

# Vérification par e-mail {#email-verification}

Les abonnements Adobe Marketo Engage nécessitent que tous les utilisateurs et utilisatrices ne disposant pas d’API uniquement, y compris les administrateurs et administratrices Marketo Engage, vérifient leur adresse e-mail.

## Raison Pour Laquelle Cette Fonctionnalité A Été Introduite {#why-this-feature-was-introduced}

Marketo Engage poursuit le déploiement de la vérification par e-mail en vue de la migration des clients vers Adobe Business Platform, y compris la migration des utilisateurs vers les Adobe ID. Cette fonctionnalité améliore la sécurité des comptes utilisateur Marketo Engage existants. Pour vous assurer qu’un utilisateur Marketo Engage est associé à l’Adobe ID approprié, les utilisateurs Marketo Engage existants doivent vérifier leur adresse e-mail. Un utilisateur Marketo Engage doit disposer d’une adresse e-mail vérifiée pour pouvoir migrer vers Adobe ID. Si un utilisateur Marketo Engage ne vérifie pas son adresse e-mail, il ne peut pas être migré vers une Adobe ID et perdra l’accès à un abonnement Marketo une fois la migration de l’utilisateur pour l’abonnement terminée.

## Invitation d’utilisateur {#user-invite}

Lorsqu’un administrateur invite un utilisateur, celui-ci est automatiquement vérifié lorsqu’il clique sur le lien d’invitation.

>[!IMPORTANT]
>
>L’exception à la règle ci-dessus est que, _dans un abonnement SSO uniquement_, les administrateurs recevront une nouvelle invitation d’utilisateur, mais pas les utilisateurs non administrateurs. Les utilisateurs qui ne sont pas administrateurs doivent toujours passer par le processus de vérification des e-mails pour assurer la migration de leurs enregistrements. Les utilisateurs peuvent s’envoyer le lien de vérification par e-mail en cliquant sur l’icône « Mon profil » et en accédant à **Mon compte** > **Paramètres du compte** > **Renvoyer la vérification**.

![](assets/email-verification-1.png)

## Vérification de l’e-mail {#verification-email}

Les utilisateurs recevront l’e-mail ci-dessous lorsque la vérification par e-mail sera activée pour un abonnement ou si elle est déclenchée par un administrateur/utilisateur.

Une session utilisateur active est requise pour que la vérification par e-mail réussisse. L’utilisateur doit d’abord se connecter à son abonnement Marketo à l’aide de son URL de fournisseur d’identité (IdP). Une fois une session établie, ils cliqueraient _puis_ sur le lien **Vérifier l’adresse e-mail** contenu dans l’e-mail.

![](assets/email-verification-2.png)

>[!TIP]
>
>Pour renvoyer un e-mail de vérification à un utilisateur non vérifié, sélectionnez simplement son enregistrement et cliquez sur le bouton **[!UICONTROL Vérifier l’e-mail]**.

## Modification d’une adresse e-mail {#changing-an-email-address}

Lorsque l’adresse e-mail d’un utilisateur est modifiée, elle n’est plus vérifiée. Un e-mail leur sera envoyé pour leur permettre de revérifier. Les utilisateurs peuvent renvoyer manuellement cet e-mail en cliquant sur **[!UICONTROL Renvoyer la vérification]**.

![](assets/email-verification-3.png)

![](assets/email-verification-4.png)

## Utilisateurs et utilisatrices et rôles {#users-and-roles}

Dans **[!UICONTROL Admin]** > **[!UICONTROL Utilisateurs et rôles]**, la colonne État de l’e-mail affiche l’état de vérification de chaque utilisateur.

![](assets/email-verification-5.png)

## Plusieurs ID de connexion d’utilisateur {#multiple-user-login-ids}

Un seul compte utilisateur peut être associé à une seule adresse électronique. Si plusieurs comptes utilisateur sont associés à une seule adresse e-mail, Marketo Engage exige que le conflit soit résolu et affiche toutes les connexions utilisateur associées à l’adresse e-mail, ainsi que trois options de résolution :

* Utiliser l’e-mail actuel pour l’ID de connexion de l’utilisateur actuel
* Utiliser un nouvel e-mail pour l’ID de connexion de l’utilisateur actuel
* Retarder la décision jusqu’à la prochaine connexion

  ![](assets/email-verification-6.png)

>[!NOTE]
>
>Bien qu’un compte utilisateur doive être associé à une seule adresse, il peut être utilisé pour de nombreux abonnements via l’Universal ID.
