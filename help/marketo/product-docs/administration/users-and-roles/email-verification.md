---
description: Vérification des courriers électroniques - Documents Marketo - Documentation du produit
title: Vérification des emails
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: e104a8bd41d61451202ba089512dc688680292ce
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Vérification des emails {#email-verification}

Les abonnements à Adobe Marketo Engage requièrent que tous les utilisateurs non-API uniquement, y compris les administrateurs de Marketo Engage, vérifient leur adresse électronique. Les utilisateurs de l’authentification unique (SSO) qui ne se voient pas attribuer un rôle d’administrateur ou qui se voient attribuer un rôle avec l’autorisation &quot;Contourner la connexion unique&quot; verront leur email automatiquement vérifié lorsque leur abonnement est activé avec la fonction de vérification des emails.

## Invitation d’utilisateur {#user-invite}

Lorsqu’un administrateur invite un utilisateur, celui-ci est automatiquement vérifié lorsqu’il clique sur le lien d’invitation. Les utilisateurs d’authentification unique, qui ne disposent pas du rôle d’administrateur, sont automatiquement vérifiés.

## Courrier électronique de vérification {#verification-email}

Les utilisateurs invités recevront le courrier électronique suivant :

![](assets/email-verification-1.png)

>[!NOTE]
>
>Pour renvoyer un email de vérification à un utilisateur non vérifié, sélectionnez simplement son enregistrement et cliquez sur le bouton **Vérifier le courrier électronique** bouton .

## Modification d’une adresse électronique {#changing-an-email-address}

Lorsque l’adresse électronique d’un utilisateur est modifiée, elle n’est plus vérifiée. Un email leur sera envoyé pour leur permettre de vérifier à nouveau. Les utilisateurs peuvent renvoyer manuellement cet email en cliquant sur **Vérification du renvoi**.

![](assets/email-verification-2.png)

![](assets/email-verification-3.png)

## Utilisateurs et rôles {#users-and-roles}

Dans **Administration** > **Utilisateurs et rôles**, la colonne État de l’email indique l’état de vérification de chaque utilisateur.

![](assets/email-verification-4.png)

## Plusieurs ID de connexion utilisateur {#multiple-user-login-ids}

Un seul compte utilisateur peut être associé à une seule adresse électronique. Si plusieurs comptes d’utilisateurs sont associés à une seule adresse électronique, Marketo Engage exige que le conflit soit résolu et affiche toutes les connexions d’utilisateurs associées à l’adresse électronique, ainsi que trois options de résolution :

* Utiliser le courrier électronique actuel pour l’ID de connexion de l’utilisateur actuel
* Utiliser un nouveau courrier électronique pour l’ID de connexion de l’utilisateur actuel
* Retarder la décision jusqu’à la prochaine connexion

   ![](assets/email-verification-5.png)

>[!NOTE]
>
>Bien qu’un compte utilisateur doive être associé à une seule adresse, un compte utilisateur peut être utilisé pour de nombreux abonnements via un ID universel.
