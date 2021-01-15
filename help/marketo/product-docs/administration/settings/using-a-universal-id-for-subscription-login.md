---
unique-page-id: 10100311
description: Utilisation d’un ID universel pour la connexion à l’Abonnement - Documents marketing - Documentation du produit
title: Utilisation d’un ID universel pour la connexion à un Abonnement
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---


# Utilisation d’un ID universel pour la connexion à l’Abonnement {#using-a-universal-id-for-subscription-login}

Un ID universel vous permet d’accéder à plusieurs abonnements du marketing à l’aide d’une seule connexion et de basculer rapidement d’un abonnement à l’autre. Cependant, si vous le souhaitez, vous pouvez utiliser des identifiants de connexion différents pour vos abonnements.

Avec l’ID universel, vous créez toujours des tickets d’assistance pour chacun de vos abonnements.

Les paramètres au niveau de l’Abonnement sont respectés pour les utilisateurs qui utilisent l’ID universel, par exemple, les rôles, les autorisations et les stratégies de mot de passe. Les modifications au niveau du profil utilisateur sont répercutées dans tous les abonnements, par exemple, le prénom, le nom et l’adresse électronique.

## Configuration d’un ID universel {#setting-up-a-universal-id}

De chaque instance individuelle, l’administrateur de Marketing Cloud doit vous inviter à accéder à chacun de vos abonnements différents avec la même connexion. Marketo ne peut pas fusionner automatiquement vos identifiants de connexion existants. Une fois que vous avez activé l’ID universel, **votre instance de Marketo sera indisponible** pendant 30 minutes au maximum. Si vous disposez d’une plus grande base d’utilisateurs, elle peut être un peu plus longue.

>[!CAUTION]
>
>Si l’ID unique ou l’ID universel est activé pour un utilisateur, ses rôles et espaces de travail peuvent **ne pas** être modifiés après leur configuration initiale.

>[!NOTE]
>
>Si vous avez plusieurs identifiants de connexion d’abonnement, vous pouvez également avoir plusieurs profils de communauté. Veillez à choisir l’identifiant de votre ID universel qui est connecté au profil que vous souhaitez utiliser, c’est-à-dire pour votre instance de production, et non pour votre sandbox.

## Connexion {#logging-in}

Lorsque vous vous connectez pour accepter une invitation à un deuxième abonnement à l’aide d’un ID universel, la page de connexion d’inclusion s’affiche. Ici, vous devez cocher une case pour accepter les termes et conditions. Après avoir accepté, vous verrez la page de réinitialisation normale, pas celle-ci, pour les connexions suivantes. En acceptant les termes et conditions, vous autorisez Marketing à distribuer vos données de profil de base (telles que le prénom, le nom et l’adresse électronique) aux centres de données dans différents emplacements où votre abonnement est hébergé.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>Les identifiants que vous n’utilisez plus restent, sauf si l’administrateur de l’abonnement les supprime. Nous vous recommandons de les conserver, au cas où, par exemple, un rapport privé vous est attribué, qui ne peut être consulté qu’à l’aide de cet identifiant. Dans ce cas, il est logique de déplacer ces rapports privés vers votre nouvel identifiant universel, puis de supprimer votre identifiant existant.

## Mots de passe {#passwords}

Avec l’ID universel pour plusieurs abonnements, Marketo applique automatiquement la stratégie de mot de passe la plus stricte. Par exemple, si certains abonnements exigent une longueur minimale de mot de passe et que d’autres ne le font pas, la longueur minimale sera appliquée à tous les abonnements.

Avec un ID universel pour plusieurs abonnements, vous seul pouvez modifier le mot de passe.

>[!NOTE]
>
>Marketo demandera aux utilisateurs qui souhaitent utiliser l’ID universel de réinitialiser leur mot de passe si le mot de passe de l’abonnement actuel n’est pas conforme à la stratégie de mot de passe du deuxième abonnement auquel ils sont invités.

## Basculement entre les Abonnements {#switching-between-subscriptions}

A l’aide d’un ID universel, vous pouvez voir l’abonnement dans lequel vous êtes connecté et sélectionner d’autres abonnements auxquels vous avez accès. Dans la plupart des cas, vous pouvez basculer entre eux sans avoir à vous déconnecter puis à vous reconnecter.

![](assets/image2016-11-3-15-3a10-3a16.png)

Lorsque vous vous déconnectez puis vous reconnectez, Marketo vous connecte automatiquement à l’abonnement dans lequel vous avez été connecté pour la dernière fois. Vous pouvez ensuite passer à un autre abonnement si nécessaire.

## Profils communautaires {#community-profiles}

Si vous avez plusieurs abonnements, vous pouvez avoir plusieurs profils de communauté. Nous vous recommandons de choisir la connexion qui est liée à votre profil communautaire le plus principal.

## Plateforme mobile {#mobile-platform}

Les utilisateurs disposant d’un ID universel peuvent consulter leurs données sur les moments marketing et l’application d’enregistrement de événement iPad depuis l’abonnement sur lequel ils se sont connectés pour la dernière fois. Vous ne pouvez pas modifier les abonnements à partir de la plate-forme mobile elle-même.
