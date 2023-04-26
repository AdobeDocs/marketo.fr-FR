---
description: Vérification des courriers électroniques - Documents Marketo - Documentation du produit
title: Vérification des emails
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: c45b3ab94b806b53768891613f15b8e9b694a440
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Vérification des emails {#email-verification}

Les abonnements à Adobe Marketo Engage requièrent que tous les utilisateurs non-API uniquement, y compris les administrateurs de Marketo Engage, vérifient leur adresse électronique. Les utilisateurs de l’authentification unique (SSO) qui ne se voient pas attribuer un rôle d’administrateur ou qui se voient attribuer un rôle avec l’autorisation &quot;Contourner la connexion unique&quot; verront leur email automatiquement vérifié lorsque leur abonnement est activé avec la fonction de vérification des emails.

**Invitation d’utilisateur**

Lorsqu’un administrateur invite un utilisateur, celui-ci est automatiquement vérifié lorsqu’il clique sur le lien d’invitation. Les utilisateurs d’authentification unique, qui ne disposent pas du rôle d’administrateur, sont automatiquement vérifiés.

**Modification d’une adresse électronique**

Lorsque l’adresse électronique d’un utilisateur est modifiée, elle n’est plus vérifiée. Un email leur sera envoyé pour leur permettre de vérifier à nouveau. Les utilisateurs peuvent renvoyer manuellement cet email en cliquant sur **Vérification du renvoi**.

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

**Utilisateurs et rôles**

Dans Admin > Utilisateurs et rôles, la colonne État de l’email indique l’état de vérification de chaque utilisateur.

![](assets/email-verification-3.png)

Pour renvoyer un email de vérification à un utilisateur non vérifié, sélectionnez simplement son enregistrement et cliquez sur le bouton **Vérifier le courrier électronique** bouton .
