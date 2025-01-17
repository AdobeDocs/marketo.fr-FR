---
unique-page-id: 10100311
description: Utilisation d’un ID universel pour la connexion à l’abonnement - Documents Marketo - Documentation du produit
title: Utilisation d’un ID universel pour la connexion à l’abonnement
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
feature: Administration
source-git-commit: 5a8ea3c5356cb370b4e502b23eea8a457bfc97f1
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Utilisation d’un ID universel pour la connexion à l’abonnement {#using-a-universal-id-for-subscription-login}

Un ID universel permet d’accéder à plusieurs abonnements Marketo à l’aide d’une seule connexion et de basculer rapidement entre les abonnements. Cependant, si vous le souhaitez, vous pouvez utiliser des identifiants de connexion différents pour vos abonnements.

Avec l’ID universel, vous créez toujours des tickets d’assistance pour chacun de vos abonnements individuels.

Les paramètres de niveau d’abonnement sont respectés pour les utilisateurs qui utilisent l’ID universel, par exemple les rôles, les autorisations et les stratégies de mot de passe. Les modifications au niveau du profil utilisateur sont répercutées dans tous les abonnements, par exemple, le prénom, le nom et l’adresse électronique.

## Configuration d’un ID universel {#setting-up-a-universal-id}

Tous les abonnements Marketo sont fournis avec la fonction d’identification universelle facultative. Depuis chaque instance, votre administrateur Marketo doit vous inviter à rejoindre chacun de vos abonnements avec le même identifiant. Marketo ne peut pas fusionner automatiquement vos connexions existantes.

>[!NOTE]
>
>Si vous disposez de plusieurs ID de connexion d’abonnement, vous pouvez également disposer de plusieurs profils de communauté. Veillez à choisir l’identifiant de votre ID universel qui est connecté au profil que vous souhaitez utiliser, c’est-à-dire pour votre instance de production, et non votre environnement de test.

## Connexion {#logging-in}

Lorsque vous vous connectez pour accepter une invitation à un second abonnement à l’aide d’un ID universel, la page de connexion d’Opt-in s’affiche. Vous devez cocher une case pour accepter les conditions générales. Une fois que vous avez accepté, vous verrez la page de réinitialisation normale, et non celle-ci, pour toutes les connexions suivantes. En acceptant les conditions générales, vous autorisez Marketo à distribuer vos données de profil de base (prénom, nom et adresse électronique, par exemple) aux centres de données aux différents emplacements où votre abonnement est hébergé.

![](assets/using-a-universal-id-for-subscription-login-1.png)

>[!TIP]
>
>Les identifiants que vous n’utilisez plus restent sauf si l’administrateur des abonnements les supprime. Nous vous recommandons de les conserver, au cas où, par exemple, un rapport privé, qui ne peut être accessible qu’à l’aide de cet identifiant, vous vous êtes attribué. Dans ce cas, il est logique de déplacer ces rapports privés vers votre nouvel ID universel, puis de supprimer votre ID existant.

## Mots de passe {#passwords}

Avec l’identifiant universel pour plusieurs abonnements, Marketo applique automatiquement la stratégie de mot de passe la plus stricte. Par exemple, si certains abonnements requièrent une longueur de mot de passe minimale, tandis que d’autres ne le font pas, la longueur minimale est appliquée à tous les abonnements.

Avec un ID universel pour plusieurs abonnements, seul vous pouvez modifier le mot de passe.

>[!NOTE]
>
>Marketo demandera aux utilisateurs qui souhaitent utiliser l’ID universel de réinitialiser leur mot de passe si le mot de passe de l’abonnement actuel ne respecte pas la politique de mot de passe du deuxième abonnement auquel ils sont invités.

## Changement d’abonnement {#switching-between-subscriptions}

À l’aide d’un ID universel, vous pouvez voir l’abonnement auquel vous êtes connecté et sélectionner d’autres abonnements auxquels vous avez accès pour vous connecter. Dans la plupart des cas, vous pouvez basculer entre les deux sans avoir à vous déconnecter puis à vous reconnecter.

Si [Authentification unique](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) et ID universel sont activés, l’autorisation &quot;Contournement de la connexion unique&quot; doit être définie pour basculer entre les abonnements.

![](assets/using-a-universal-id-for-subscription-login-2.png)

Lorsque vous vous déconnectez puis vous reconnectez, Marketo vous connecte automatiquement à l’abonnement pour la dernière fois que vous vous êtes connecté. Vous pouvez ensuite passer à un autre abonnement si nécessaire.

## Profils de communauté {#community-profiles}

Si vous disposez de plusieurs abonnements, vous pouvez disposer de plusieurs profils de communauté. Nous vous recommandons de choisir la connexion qui est liée à votre profil de communauté le plus actif.

>[!MORELIKETHIS]
>
>* [Ajout d’une connexion unique à un portail](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md){target="_blank"}
>* [Limiter la connexion de l’utilisateur à SSO uniquement](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [Invitation d’utilisateurs Marketo à deux instances avec un ID universel](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
