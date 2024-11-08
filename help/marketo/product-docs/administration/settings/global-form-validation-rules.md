---
description: Règles de validation de formulaire globales - Documents Marketo - Documentation du produit
title: Règles générales de validation du formulaire
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 8958bbd03c3c6b1c6ac4769c229ad28590191fb3
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 2%

---

# Règles générales de validation du formulaire {#global-form-validation-rules}

Cette fonctionnalité vous permet de bloquer l’envoi de domaines spécifiques à des formulaires Marketo Engage.

## Comment activer l’accès {#how-to-enable-access}

Avant de pouvoir utiliser cette fonction, vous devez activer son autorisation en fonction du rôle souhaité.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-1.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/global-form-validation-rules-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Rôles]** .

   ![](assets/global-form-validation-rules-3.png)

1. Double-cliquez sur le rôle auquel vous souhaitez accorder des autorisations.

   ![](assets/global-form-validation-rules-4.png)

1. Cliquez sur le signe **+** en regard de l’option Accéder à l’administrateur.

   ![](assets/global-form-validation-rules-5.png)

1. Faites défiler l’écran vers le bas et sélectionnez **[!UICONTROL Accéder aux règles de validation de formulaire]** et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/global-form-validation-rules-6.png)

## Créer une règle de validation de formulaire {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Ces règles s&#39;appliqueront à tous les formulaires de votre ou vos abonnements de Marketo Engage.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-7.png)

1. Cliquez sur **[!UICONTROL Règle de validation de formulaire globale]**.

   ![](assets/global-form-validation-rules-8.png)

1. Cliquez sur **[!UICONTROL Nouvelle règle de validation de formulaire]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >La liste déroulante Actions de règle de validation de formulaire vous permet de supprimer ou de modifier des règles existantes.

1. Attribuez un nom à votre règle, fournissez-lui une description facultative, puis saisissez le message d’erreur que vous souhaitez que les visiteurs de votre formulaire voient. Saisissez le ou les domaines que vous souhaitez bloquer dans la zone des règles, sélectionnez **[!UICONTROL Activer la règle]**, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage dispose d’une liste bloquée définie de domaines d’e-mail de consommateur gratuits qui sont bloqués lors de l’utilisation de notre règle &quot;Liste bloquée de domaine d’e-mail de consommateur&quot; préchargée. [Affichez cette liste ici](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv) (pour télécharger, vérifiez que votre navigateur est à jour et qu’il peut accepter les téléchargements).

## Comment désactiver l’accès par formulaire{#how-to-disable-access-per-form}

Une fois activées, les règles s’appliquent à tous les formulaires. Toutefois, si vous disposez d’un formulaire avec des exigences spécifiques et que vous ne souhaitez rien refuser, vous pouvez désactiver les [!UICONTROL Règles de validation de formulaire globales] dans les paramètres du formulaire.

1. Dans le formulaire de votre choix, cliquez sur **[!UICONTROL Paramètres de formulaire]**, puis sur **[!UICONTROL Paramètres]**.

   ![](assets/global-form-validation-rules-11.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Règles de validation de formulaire globales]** et sélectionnez **[!UICONTROL Désactivé]**.

   ![](assets/global-form-validation-rules-12.png)

Lorsque vous approuvez et publiez votre formulaire, il ignorera vos [!UICONTROL Règles de validation de formulaire globales].
