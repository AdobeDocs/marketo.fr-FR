---
unique-page-id: 12981050
description: Verrouiller le modèle de vente - Documents Marketo - Documentation du produit
title: Verrouiller le modèle de vente
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

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

1. Accédez à **Administration**, puis cliquez sur **Statistiques des ventes**.

   ![](assets/1.png)

1. Sous **Paramètres**, cliquez sur **Modifier**.

   ![](assets/2.png)

1. Vérifier **Activer la possibilité de verrouiller des modèles**. Cliquez sur **Enregistrer**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Par défaut, cette case est cochée et la possibilité de verrouiller des modèles est activée. Si vous la décochez, la fonction de modèle de verrouillage sera désactivée dans l’éditeur d’email.

>[!NOTE]
>
>Si vous modifiez ce paramètre en tant qu’administrateur, **not** affecte rétroactivement les modèles existants ; En d’autres termes, il ne les verrouillera pas automatiquement.

## Verrouillage d’un modèle dans l’éditeur de courrier électronique {#lock-template-in-the-email-editor}

1. Sélectionnez l&#39;email que vous souhaitez verrouiller, puis cliquez sur **Modifier le brouillon**.

   ![](assets/5.png)

1. Dans l’éditeur d’email, cliquez sur **Paramètres de messagerie électronique**.

   ![](assets/6.png)

1. Vérifier **Publication sur Marketo Sales Insight** s’il n’est pas déjà vérifié. Vous pouvez désormais décocher la case **Autoriser un utilisateur CRM à modifier un email** afin de verrouiller le modèle. Cliquez sur **Enregistrer**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Cette case est cochée par défaut et les utilisateurs CRM sont autorisés à modifier les emails.
