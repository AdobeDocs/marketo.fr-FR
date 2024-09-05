---
unique-page-id: 2360358
description: Limitation de la connexion des utilisateurs à l’authentification unique - Documents Marketo - Documentation du produit
title: Limiter la connexion de l'utilisateur aux connexions par signature unique
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: a12e4e420c01623305a0fa34b1e3973162e24d68
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 5%

---

# Limiter la connexion de l&#39;utilisateur aux connexions par signature unique {#restrict-user-login-to-sso-only}

Si vous [ utilisez SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) et souhaitez vous assurer que les utilisateurs ne peuvent pas contourner la sécurité SSO, suivez ces instructions.

>[!IMPORTANT]
>
>Cet article ne s’applique pas aux abonnements Marketo [Adobe IMS-enabled](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md).

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Cliquez sur **[!UICONTROL Paramètre de connexion]s**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Cliquez sur **[!UICONTROL Modifier les paramètres de sécurité]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Développez les paramètres **[!UICONTROL Avancé]**, cochez la case **[!UICONTROL Require SSO]**, puis cliquez sur **[!UICONTROL Enregistrer]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Il est recommandé que le ou les utilisateurs soient invités et acceptent l’invitation. _Après_ l’invitation est acceptée, les administrateurs doivent ensuite la définir sur &quot;[!UICONTROL Require SSO]&quot;.

>[!TIP]
>
>Si vous sélectionnez **[!UICONTROL Require SSO]**, vous pouvez exclure un [rôle d’utilisateur](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) de cette restriction en cochant l’option **[!UICONTROL Contournement de l’authentification unique]** lors de la configuration du rôle. Cela permet aux utilisateurs de se connecter normalement. Par exemple, les utilisateurs administrateurs peuvent toujours avoir besoin de se connecter à Marketo par le biais de l’écran de connexion. Si l’authentification unique et l’ID universel sont activés, l’autorisation &quot;Contourner l’authentification unique&quot; doit être définie pour basculer entre les abonnements.

>[!CAUTION]
>
>Lorsque de nouveaux utilisateurs sont invités, ils reçoivent des e-mails d’invitation. Cependant, si **[!UICONTROL Require SSO]** est sélectionné, ils ne recevront pas ces e-mails, sauf s’ils se voient attribuer un rôle défini sur **[!UICONTROL Contourner l’authentification unique]**.

Vous avez terminé. Désormais, tous les utilisateurs (à l’exception des utilisateurs autorisés à contourner l’authentification unique) seront limités à l’utilisation de la connexion unique.

>[!MORELIKETHIS]
>
>* [Ajout d’une connexion unique à un portail](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [ Utilisation d’un ID universel pour la connexion à l’abonnement ](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invitation d’utilisateurs Marketo à deux instances avec un ID universel](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
