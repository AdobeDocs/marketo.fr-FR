---
unique-page-id: 2360358
description: Restreindre la connexion utilisateur à l’authentification unique uniquement - Documents Marketo - Documentation du produit
title: Limiter la connexion de l'utilisateur aux connexions par signature unique
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 5%

---

# Limiter la connexion de l&#39;utilisateur aux connexions par signature unique {#restrict-user-login-to-sso-only}

Si vous [utilisez SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) et souhaitez vous assurer que les utilisateurs ne peuvent pas contourner la sécurité SSO, suivez ces instructions.

>[!IMPORTANT]
>
>Cet article ne s’applique pas aux abonnements [Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Cliquez sur **[!UICONTROL Paramètres de connexion]**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Cliquez sur **[!UICONTROL Modifier les paramètres de sécurité]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Développez les paramètres **[!UICONTROL Avancé]**, cochez la case **[!UICONTROL Exiger une authentification unique]**, puis cliquez sur **[!UICONTROL Enregistrer]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Une bonne pratique consiste à inviter le(s) utilisateur(s) et à accepter l’invitation. _Une fois_ l’invitation acceptée, les administrateurs doivent la définir sur « [!UICONTROL  Exiger une authentification unique ]. »

>[!TIP]
>
>Si vous sélectionnez **[!UICONTROL Exiger une authentification unique]**, vous pouvez exclure un [rôle utilisateur](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) de cette restriction en cochant l’option **[!UICONTROL Contourner l’authentification unique]** lors de la configuration du rôle. Cela permettra aux utilisateurs de se connecter normalement. Par exemple, les utilisateurs administrateurs peuvent toujours avoir besoin de se connecter à Marketo via l’écran de connexion. Si la connexion unique et l’identifiant universel sont activés, l’autorisation « Contourner l’authentification unique » doit être définie pour basculer entre les abonnements.

>[!CAUTION]
>
>Lorsque de nouveaux utilisateurs sont invités, ils reçoivent des e-mails d’invitation. Cependant, si l’option **[!UICONTROL Exiger une authentification unique]** est sélectionnée, ils ne recevront pas ces e-mails, sauf s’ils sont affectés à un rôle défini sur **[!UICONTROL Contourner l’authentification unique]**.

Vous avez terminé. Désormais, tous les utilisateurs (à l’exception des utilisateurs autorisés à contourner l’authentification unique) ne pourront utiliser que la connexion SSO.

>[!MORELIKETHIS]
>
>* [Ajouter l&#39;authentification SSO à un portail](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Utilisation d’un identifiant universel pour la connexion à l’abonnement](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Invitation d’utilisateurs Marketo à deux instances avec un ID universel](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
