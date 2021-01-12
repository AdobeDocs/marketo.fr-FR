---
unique-page-id: 2360358
description: Limiter la connexion de l’utilisateur à l’authentification unique - Documents marketing - Documentation du produit
title: Restreindre la connexion utilisateur à SSO uniquement
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Limiter la connexion de l’utilisateur à l’authentification unique {#restrict-user-login-to-sso-only}

Si vous utilisez [SSO](add-single-sign-on-to-a-portal.md) et souhaitez vous assurer que les utilisateurs ne peuvent pas contourner la sécurité de l’authentification unique, suivez ces instructions.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à **Admin** et cliquez sur **Paramètres de connexion**.

![](assets/image2014-9-24-14-3a44-3a40.png)

1. Cliquez sur **Modifier les paramètres de sécurité**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Développez les paramètres Avancées, cochez **Requiert SSO**, puis cliquez sur **Enregistrer**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!TIP]
>
>Si vous sélectionnez **Exiger une authentification unique**, vous pouvez exclure un [rôle utilisateur](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) de cette restriction en cochant l&#39;option **Contourner la connexion unique** lors de la configuration du rôle. Cela permet aux utilisateurs de se connecter normalement. Par exemple, les administrateurs peuvent toujours avoir à se connecter à Marketing Cloud par l’intermédiaire de l’écran de connexion.

>[!CAUTION]
>
>Lorsque de nouveaux utilisateurs sont invités, ils reçoivent un courrier électronique d’invitation. Cependant, si **Require SSO** est sélectionné, ils ne recevront pas ces courriels, à moins qu&#39;ils ne soient affectés à un rôle défini sur **Contourner la connexion unique**.

C&#39;est tout ! Désormais, tous les utilisateurs (à l’exception des utilisateurs autorisés à contourner la connexion unique) seront limités à l’utilisation de la connexion SSO uniquement.
