---
unique-page-id: 2360358
description: Exiger une authentification unique pour tous les utilisateurs afin qu’ils ne puissent pas contourner la sécurité de l’authentification unique via les paramètres de connexion administrateur (ne s’applique pas à Adobe IMS).
title: Limiter la connexion de l’utilisateur ou de l’utilisatrice aux connexions par authentification unique
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
TQID: https://experienceleague.adobe.com/2YaweRRhrf8po6RR3V64kCan8qQhDNKDrhr7TfnNNJs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 273
ht-degree: 5%

---

# Limiter la connexion de l’utilisateur ou de l’utilisatrice aux connexions par authentification unique {#restrict-user-login-to-sso-only}

Si vous [utilisez SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) et souhaitez vous assurer que les utilisateurs ne peuvent pas contourner la sécurité SSO, suivez ces instructions.

>[!IMPORTANT]
>
>Cet article ne s’applique pas aux abonnements [Adobe IMS](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo.

>[!NOTE]
>
>**Autorisations d’administration requises**

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
>Une bonne pratique consiste à inviter le(s) utilisateur(s) et à accepter l’invitation. _Une fois_ l’invitation acceptée, les administrateurs doivent la définir sur « [!UICONTROL &#x200B; Exiger une authentification unique &#x200B;]. »

>[!TIP]
>
>Si vous sélectionnez **[!UICONTROL Exiger une authentification unique]**, vous pouvez exclure un [rôle utilisateur](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) de cette restriction en cochant l’option **[!UICONTROL Contourner l’authentification unique]** lors de la configuration du rôle. Cela permet aux utilisateurs de se connecter normalement. Par exemple, les utilisateurs administrateurs peuvent toujours avoir besoin de se connecter à Marketo via l’écran de connexion. Si la connexion unique et l’identifiant universel sont activés, l’autorisation « Contourner l’authentification unique » doit être définie pour basculer entre les abonnements.

>[!CAUTION]
>
>Lorsque de nouveaux utilisateurs sont invités, ils reçoivent des e-mails d’invitation. Cependant, si l’option **[!UICONTROL Exiger une authentification unique]** est sélectionnée, ils ne reçoivent pas ces e-mails, sauf s’ils sont affectés à un rôle défini sur **[!UICONTROL Contourner l’authentification unique]**.

Désormais, tous les utilisateurs (à l’exception des utilisateurs autorisés à contourner l’authentification unique) sont limités à l’utilisation de la connexion SSO uniquement.

>[!MORELIKETHIS]
>
>* [Ajouter l&#39;authentification SSO à un portail](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Invitation d’utilisateurs Marketo à deux instances avec un ID universel](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
