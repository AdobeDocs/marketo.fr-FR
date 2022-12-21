---
unique-page-id: 1147064
description: Application de limites de communication à la campagne dynamique - Documents Marketo - Documentation du produit
title: Application de limites de communication à une campagne dynamique
exl-id: b33885ba-6811-47ab-9db9-099d35ca49df
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# Application de limites de communication à une campagne dynamique {#apply-communication-limits-to-smart-campaign}

>[!PREREQUISITES]
>
>[Activer les limites de communication](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)

Ce n&#39;est pas une bonne idée d&#39;envoyer des emails à quelqu&#39;un plusieurs fois par jour ou trop de fois par semaine, n&#39;est-ce pas ? Heureusement, Marketo a des limites de communication pour aider. Voici comment ils fonctionnent.

>[!NOTE]
>
>Lorsqu’une personne dépasse les limites de communication définies, Marketo bloque les emails non opérationnels (les emails opérationnels sont toujours envoyés).

1. Dans votre campagne dynamique, cliquez sur le bouton **Planification** puis **Modifier les paramètres**.

   ![](assets/programeditsettings-hands-1.png)

1. Vérifiez les **Bloquer les emails non opérationnels** , puis cliquez sur **Enregistrer**.

   ![](assets/apply-communication-limits-to-smart-campaign.png)

>[!NOTE]
>
>La limite fait référence au nombre de personnes qualifiées qu’une campagne dynamique peut affecter.

>[!TIP]
>
>Pour définir cette valeur par défaut, modifiez la variable  [limites de communication](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md) dans la section Admin .

Doux. Maintenant, vous pouvez être certain que vous n&#39;envoyez pas accidentellement trop d&#39;emails à votre audience.
