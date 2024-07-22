---
unique-page-id: 12981050
description: Verrouiller le modèle de vente - Documents Marketo - Documentation du produit
title: Verrouiller le modèle de vente
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 1%

---

# Verrouiller le modèle de vente {#lock-sales-template}

Pour empêcher les utilisateurs de CRM de modifier les modèles de vente, les administrateurs peuvent activer la possibilité de verrouiller les modèles, ce qui permet ensuite aux utilisateurs de verrouiller les modèles individuellement à partir de l’éditeur d’email.

>[!CAUTION]
>
>Cette fonctionnalité fonctionne uniquement pour Salesforce et n’est pas compatible avec Microsoft Dynamics ou d’autres CRM. Les modèles accessibles à partir des modules externes Outlook ou Gmail ne seront pas verrouillés, car l’éditeur n’est pas contrôlé par Marketo.

## Activer le modèle de verrouillage {#enable-lock-template}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à **Admin**, puis cliquez sur **Sales Insight**.

   ![](assets/1.png)

1. Sous **Settings**, cliquez sur **Edit**.

   ![](assets/2.png)

1. Cochez **Activer la possibilité de verrouiller des modèles**. Cliquez sur **Enregistrer**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Par défaut, cette case est cochée et la possibilité de verrouiller des modèles est activée. Si vous la décochez, la fonction de modèle de verrouillage sera désactivée dans l’éditeur d’email.

>[!NOTE]
>
>Si vous modifiez ce paramètre en tant qu’administrateur, **et non**, les modèles existants seront affectés rétroactivement ; en d’autres termes, ils ne seront pas verrouillés automatiquement.

## Verrouillage d’un modèle dans l’éditeur de courrier électronique {#lock-template-in-the-email-editor}

1. Sélectionnez l&#39;email que vous souhaitez verrouiller, puis cliquez sur **Modifier le brouillon**.

   ![](assets/5.png)

1. Dans l’éditeur de courrier électronique, cliquez sur **Paramètres de courrier électronique**.

   ![](assets/6.png)

1. Vérifiez **Publish to Marketo Sales Insight** si ce n’est pas déjà fait. Vous pouvez désormais décocher la case **Autoriser l&#39;utilisateur CRM à modifier l&#39;email** afin de verrouiller le modèle. Cliquez sur **Enregistrer**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Cette case est cochée par défaut et les utilisateurs CRM sont autorisés à modifier les emails.
