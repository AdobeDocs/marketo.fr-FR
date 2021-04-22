---
unique-page-id: 2360358
description: Restreindre la connexion utilisateur à l’authentification unique - Marketo Docs - Documentation du produit
title: Limiter la connexion de l'utilisateur aux connexions par signature unique
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 5%

---

# Limiter la connexion de l&#39;utilisateur aux connexions par signature unique {#restrict-user-login-to-sso-only}

Si vous utilisez [SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) et souhaitez vous assurer que les utilisateurs ne peuvent pas contourner la sécurité de l’authentification unique, suivez ces instructions.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à **Admin** et cliquez sur **Paramètres de connexion**.

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. Cliquez sur **Modifier les paramètres de sécurité**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Développez les paramètres Avancées, cochez **Requiert SSO**, puis cliquez sur **Enregistrer**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>Il est recommandé que le ou les utilisateurs soient invités et acceptent l’invitation. _Une_ fois l’invitation acceptée, les administrateurs doivent alors la définir sur &quot;Exiger une authentification unique&quot;.

>[!TIP]
>
>Si vous sélectionnez **Exiger une authentification unique**, vous pouvez exclure un [rôle utilisateur](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) de cette restriction en cochant l&#39;option **Contourner la connexion unique** lors de la configuration du rôle. Cela permet aux utilisateurs de se connecter normalement. Par exemple, les utilisateurs administrateurs peuvent encore avoir à se connecter à Marketo par le biais de l’écran de connexion.

>[!CAUTION]
>
>Lorsque de nouveaux utilisateurs sont invités, ils reçoivent un courrier électronique d’invitation. Cependant, si **Require SSO** est sélectionné, ils ne recevront pas ces courriels, à moins qu&#39;ils ne soient affectés à un rôle défini sur **Contourner la connexion unique**.

C&#39;est tout ! Désormais, tous les utilisateurs (à l’exception des utilisateurs autorisés à contourner la connexion unique) seront limités à l’utilisation de la connexion SSO uniquement.

>[!MORELIKETHIS]
>
>* [Ajouter la connexion unique à un portail](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Utilisation d’un ID universel pour la connexion à un Abonnement](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invitation d’utilisateurs Marketo à deux instances avec un identifiant universel](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

