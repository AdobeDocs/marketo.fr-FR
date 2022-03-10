---
unique-page-id: 2360358
description: Limitation de la connexion des utilisateurs à l’authentification unique - Documents Marketo - Documentation du produit
title: Limiter la connexion de l'utilisateur aux connexions par signature unique
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
source-git-commit: a21db1586166b7530bbbb18759752ef834cdc46a
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 5%

---

# Limiter la connexion de l&#39;utilisateur aux connexions par signature unique {#restrict-user-login-to-sso-only}

Si vous êtes [utilisation de SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) et assurez-vous que les utilisateurs ne peuvent pas contourner la sécurité d’authentification unique, suivez ces instructions.

>[!IMPORTANT]
>
>Cet article ne s’applique pas à [Compatibilité Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/overview.md) Abonnements Marketo.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à **Administration** et cliquez sur **Paramètres de connexion**.

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. Cliquez sur **Modifier les paramètres de protection**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Développez les paramètres avancés, puis cochez la case **Requiert SSO**, puis cliquez sur **Enregistrer**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>Il est recommandé que le ou les utilisateurs soient invités et acceptent l’invitation. _Après_ Si l’invitation est acceptée, les administrateurs doivent alors la définir sur &quot;Exiger une authentification unique&quot;.

>[!TIP]
>
>Si vous sélectionnez **Requiert SSO**, vous pouvez exclure une [rôle utilisateur](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) de cette restriction en cochant la variable **Contournement de l’authentification unique** lors de la configuration du rôle. Cela permet aux utilisateurs de se connecter normalement. Par exemple, les utilisateurs administrateurs peuvent toujours avoir besoin de se connecter à Marketo par le biais de l’écran de connexion.

>[!CAUTION]
>
>Lorsque de nouveaux utilisateurs sont invités, ils reçoivent des e-mails d’invitation. Cependant, si **Requiert SSO** est sélectionné, ils ne recevront pas ces e-mails, à moins qu’ils ne soient affectés à un rôle défini sur **Contournement de l’authentification unique**.

C&#39;est tout ! Désormais, tous les utilisateurs (à l’exception des utilisateurs autorisés à contourner l’authentification unique) seront limités à l’utilisation de la connexion unique.

>[!MORELIKETHIS]
>
>* [Ajout d’une authentification unique à un portail](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Utilisation d’un ID universel pour la connexion à l’abonnement](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invitation d’utilisateurs Marketo à deux instances avec un ID universel](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

