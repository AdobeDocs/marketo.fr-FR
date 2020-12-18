---
unique-page-id: 12981050
description: Verrouiller le modèle de ventes - Documents marketing - Documentation du produit
title: Verrouiller le modèle de vente
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Verrouiller le modèle de vente {#lock-sales-template}

Pour empêcher les utilisateurs de la gestion de la relation client de modifier les modèles de vente, les administrateurs peuvent activer la possibilité de verrouiller les modèles, ce qui permet ensuite aux utilisateurs de verrouiller les modèles individuellement dans l’éditeur de courrier électronique.

>[!CAUTION]
>
>Cette fonctionnalité fonctionne uniquement pour Salesforce et n&#39;est pas compatible avec Microsoft Dynamics ou d&#39;autres CRM. Les modèles accessibles à partir des modules externes Outlook ou Gmail ne seront pas verrouillés, car l&#39;éditeur n&#39;est pas contrôlé par Marketo.

## Activer le modèle de verrouillage {#enable-lock-template}

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à **Admin**, puis cliquez sur **Sales Insight**.

   ![](assets/1.png)

1. Sous **Paramètres**, cliquez sur **Modifier**.

   ![](assets/2.png)

1. Cochez **Activer la possibilité de verrouiller les modèles**. Cliquez sur **Enregistrer**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Par défaut, cette case est cochée et la possibilité de verrouiller les modèles est activée. La désactivation de cette fonction désactive la fonction de verrouillage du modèle dans l’éditeur de courrier électronique.

>[!NOTE]
>
>La modification de ce paramètre en tant qu’administrateur **n’affecte pas** rétroactivement les modèles existants ; c&#39;est-à-dire qu&#39;il ne les verrouillera pas automatiquement.

## Verrouiller le modèle dans l’éditeur de courriel {#lock-template-in-the-email-editor}

1. Sélectionnez le courrier électronique à verrouiller, puis cliquez sur **Modifier le brouillon**.

   ![](assets/5.png)

1. Dans l’éditeur de courrier électronique, cliquez sur **Paramètres de courrier électronique**.

   ![](assets/6.png)

1. Vérifiez **Publier sur Marketing Sales Insight** si ce n&#39;est pas déjà fait. Vous pouvez désormais désélectionner **Autoriser l’utilisateur CRM à modifier le courrier électronique** afin de verrouiller le modèle. Cliquez sur **Enregistrer**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Par défaut, cette case est cochée et les utilisateurs de CRM sont autorisés à modifier les courriers électroniques.

