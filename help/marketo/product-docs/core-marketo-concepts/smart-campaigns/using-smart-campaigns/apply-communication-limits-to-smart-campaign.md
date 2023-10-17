---
unique-page-id: 1147064
description: Application de limites de communication à la campagne dynamique - Documents Marketo - Documentation du produit
title: Application de limites de communication à une campagne dynamique
exl-id: b33885ba-6811-47ab-9db9-099d35ca49df
feature: Smart Campaigns
source-git-commit: fec5219c599c805328d77797d2636e549e489ca5
workflow-type: tm+mt
source-wordcount: '132'
ht-degree: 0%

---

# Application de limites de communication à une campagne dynamique {#apply-communication-limits-to-smart-campaign}

>[!PREREQUISITES]
>
>[Activer les limites de communication](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md){target="_blank"}

Ce n&#39;est pas une bonne idée d&#39;envoyer des emails à quelqu&#39;un plusieurs fois par jour, ou trop de fois par semaine, n&#39;est-ce pas ? Heureusement, le Marketo Engage a des limites de communication pour aider.

>[!NOTE]
>
>Lorsqu’une personne dépasse les limites de communication définies, Marketo bloque les emails non opérationnels (les emails opérationnels sont toujours envoyés).

1. Dans votre campagne dynamique, cliquez sur le bouton **[!UICONTROL Planification]** puis **[!UICONTROL Modifier les paramètres]**.

   ![](assets/apply-communication-limits-to-smart-campaign-1.png)

1. Vérifiez les **[!UICONTROL Bloquer les emails non opérationnels]** , puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/apply-communication-limits-to-smart-campaign-2.png)

>[!NOTE]
>
>La limite fait référence au nombre de personnes qualifiées qu’une campagne dynamique peut affecter.

>[!TIP]
>
>Pour définir cette valeur par défaut, modifiez la variable [limites de communication](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md){target="_blank"} dans la section Admin .

Maintenant, vous pouvez être certain que vous n&#39;envoyez pas accidentellement trop d&#39;emails à votre audience.
