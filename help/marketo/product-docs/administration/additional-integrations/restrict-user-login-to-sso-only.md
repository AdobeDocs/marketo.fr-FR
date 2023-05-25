---
unique-page-id: 2360358
description: Limitation de la connexion des utilisateurs à l’authentification unique - Documents Marketo - Documentation du produit
title: Limiter la connexion de l'utilisateur aux connexions par signature unique
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
source-git-commit: 1f10e1fcdbd5cf91481f749236fd37050ade29f8
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 7%

---

# Limiter la connexion de l&#39;utilisateur aux connexions par signature unique {#restrict-user-login-to-sso-only}

Si vous êtes [utilisation de SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) et assurez-vous que les utilisateurs ne peuvent pas contourner la sécurité d’authentification unique, suivez ces instructions.

>[!IMPORTANT]
>
>Cet article ne s’applique pas à [Compatibilité Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Abonnements Marketo.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Cliquez sur **[!UICONTROL Paramètre de connexion]s**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Cliquez sur **[!UICONTROL Modifier les paramètres de protection]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Développez l’objet **[!UICONTROL Avancé]** paramètres, vérifier **[!UICONTROL Requiert SSO]**, puis cliquez sur **[!UICONTROL Enregistrer]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Il est recommandé que le ou les utilisateurs soient invités et acceptent l’invitation. _Après_ Si l’invitation est acceptée, les administrateurs doivent alors la définir sur &quot;[!UICONTROL Requiert SSO].&quot;

>[!TIP]
>
>Si vous sélectionnez **[!UICONTROL Requiert SSO]**, vous pouvez exclure une [rôle utilisateur](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) de cette restriction en cochant la variable **[!UICONTROL Contournement de l’authentification unique]** lors de la configuration du rôle. Cela permet aux utilisateurs de se connecter normalement. Par exemple, les utilisateurs administrateurs peuvent toujours avoir besoin de se connecter à Marketo par le biais de l’écran de connexion.

>[!CAUTION]
>
>Lorsque de nouveaux utilisateurs sont invités, ils reçoivent des e-mails d’invitation. Cependant, si **[!UICONTROL Requiert SSO]** est sélectionné, ils ne recevront pas ces e-mails, à moins qu’ils ne soient affectés à un rôle défini sur **[!UICONTROL Contournement de l’authentification unique]**.

C&#39;est tout ! Désormais, tous les utilisateurs (à l’exception des utilisateurs autorisés à contourner l’authentification unique) seront limités à l’utilisation de la connexion unique.

>[!MORELIKETHIS]
>
>* [Ajout d’une authentification unique à un portail](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Utilisation d’un ID universel pour la connexion à l’abonnement](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invitation d’utilisateurs Marketo à deux instances avec un ID universel](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

