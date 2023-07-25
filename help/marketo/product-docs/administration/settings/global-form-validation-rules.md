---
description: Règles de validation de formulaire globales - Documents Marketo - Documentation du produit
title: Règles de validation de formulaire globales
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Règles de validation de formulaire globales {#global-form-validation-rules}

Cette fonctionnalité vous permet de bloquer l’envoi de domaines spécifiques à des formulaires Marketo Engage.

## Comment activer l’accès {#how-to-enable-access}

Avant de pouvoir utiliser cette fonction, vous devez activer son autorisation selon le rôle souhaité.

1. Dans Marketo, cliquez sur **[!UICONTROL Administration]**.

   ![](assets/global-form-validation-rules-1.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/global-form-validation-rules-2.png)

1. Cliquez sur le bouton **[!UICONTROL Rôles]** .

   ![](assets/global-form-validation-rules-3.png)

1. Double-cliquez sur le rôle auquel vous souhaitez accorder des autorisations.

   ![](assets/global-form-validation-rules-4.png)

1. Cliquez sur le bouton **+** Connectez-vous en regard de Accès à l’administrateur.

   ![](assets/global-form-validation-rules-5.png)

1. Faites défiler la page vers le bas et sélectionnez **[!UICONTROL Accès aux règles de validation de formulaire]** et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/global-form-validation-rules-6.png)

## Créer une règle de validation de formulaire {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Ces règles s&#39;appliqueront à tous les formulaires de votre ou vos abonnements de Marketo Engage.

1. Dans Marketo, cliquez sur **[!UICONTROL Administration]**.

   ![](assets/global-form-validation-rules-7.png)

1. Cliquez sur **[!UICONTROL Règle de validation de formulaire globale]**.

   ![](assets/global-form-validation-rules-8.png)

1. Cliquez sur **[!UICONTROL Nouvelle règle de validation de formulaire]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >La liste déroulante Actions de règle de validation de formulaire vous permet de supprimer ou de modifier des règles existantes.

1. Attribuez un nom à votre règle, fournissez-lui une description facultative, puis saisissez le message d’erreur que vous souhaitez que les visiteurs de votre formulaire voient. Saisissez le ou les domaines que vous souhaitez bloquer dans la zone Règles, puis sélectionnez **[!UICONTROL Activer la règle]**, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage dispose d’une liste bloquée définie de domaines d’e-mail de consommateur gratuits qui sont bloqués lors de l’utilisation de notre règle &quot;Liste bloquée de domaine d’e-mail de consommateur&quot; préchargée. [Afficher cette liste ici](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv).

## Comment désactiver l’accès par formulaire{#how-to-disable-access-per-form}

Une fois activées, les règles s’appliquent à tous les formulaires. Toutefois, si vous disposez d’un formulaire avec des exigences spécifiques et que vous ne souhaitez pas qu’aucun élément soit rejeté, vous pouvez désactiver la fonction [!UICONTROL Règles de validation de formulaire globales] dans les paramètres du formulaire.

1. Dans le formulaire de votre choix, cliquez sur **[!UICONTROL Paramètres de formulaire]**, puis **[!UICONTROL Paramètres]**.

   ![](assets/global-form-validation-rules-11.png)

1. Cliquez sur le bouton **[!UICONTROL Règles de validation de formulaire globales]** et choisissez **[!UICONTROL Désactivé]**.

   ![](assets/global-form-validation-rules-12.png)

Lorsque vous approuvez et publiez votre formulaire, il ignorera votre [!UICONTROL Règles de validation de formulaire globales].
