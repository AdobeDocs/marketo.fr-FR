---
description: Comment activer l’autorisation Accès aux règles de validation des formulaires et créer des règles globales pour bloquer l’envoi de domaines spécifiques à Marketo Engage forms.
title: Règles générales de validation du formulaire
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
TQID: https://experienceleague.adobe.com/uGwgB0vL3we5uWah5BxAa1YxcXbshilehIGoocbIEpg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 2%

---

# Règles générales de validation du formulaire {#global-form-validation-rules}

Cette fonctionnalité vous permet de bloquer l’envoi de formulaires Marketo Engage à des domaines spécifiques.

## Activation de l’accès {#how-to-enable-access}

Avant de pouvoir utiliser cette fonctionnalité, vous devez activer son autorisation pour le rôle souhaité.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-1.png)

1. Cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![](assets/global-form-validation-rules-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Rôles]**.

   ![](assets/global-form-validation-rules-3.png)

1. Double-cliquez sur le rôle pour lequel vous souhaitez accorder des autorisations.

   ![](assets/global-form-validation-rules-4.png)

1. Cliquez sur le signe **+** en regard de **Accéder à l’administrateur**.

   ![](assets/global-form-validation-rules-5.png)

1. Faites défiler vers le bas et sélectionnez **[!UICONTROL Accéder aux règles de validation de formulaire]** puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/global-form-validation-rules-6.png)

## Créer une règle de validation de formulaire {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Ces règles s’appliqueront à tous les formulaires de vos abonnements Marketo Engage.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-7.png)

1. Cliquez sur **[!UICONTROL Règle de validation de formulaire globale]**.

   ![](assets/global-form-validation-rules-8.png)

1. Cliquez sur **[!UICONTROL Nouvelle règle de validation de formulaire]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >La liste déroulante [!UICONTROL  Actions de règle de validation du formulaire ] vous permet de supprimer ou de modifier des règles existantes.

1. Nommez votre règle, donnez-lui une description facultative et saisissez le message d’erreur que vous souhaitez que les visiteurs de votre formulaire voient. Saisissez un ou plusieurs domaines à bloquer dans la zone des règles, sélectionnez **[!UICONTROL Activer la règle]**, puis cliquez sur **[!UICONTROL Créer]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage a défini une place sur la liste bloquée de domaines d’e-mail gratuits qui sont bloqués lors de l’utilisation de la règle « Domaine d’e-mail consommateur » préchargée. [Consultez cette liste ici](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv) (pour télécharger, vérifiez que votre navigateur est à jour et qu’il peut accepter les téléchargements).

## Comment désactiver l’accès par formulaire{#how-to-disable-access-per-form}

Une fois activées, les règles s’appliquent à tous les formulaires. Cependant, si vous disposez d’un formulaire avec des exigences spécifiques et que vous ne souhaitez rien rejeter, vous pouvez désactiver [!UICONTROL Règles de validation globale des formulaires] dans les paramètres du formulaire.

1. Dans le formulaire souhaité, cliquez sur **[!UICONTROL Paramètres du formulaire]**, puis **[!UICONTROL Paramètres]**.

   ![](assets/global-form-validation-rules-11.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Règles de validation globales des formulaires]** et choisissez **[!UICONTROL Désactivé]**.

   ![](assets/global-form-validation-rules-12.png)

Lorsque vous approuvez et publiez votre formulaire, il ignore vos [!UICONTROL règles globales de validation des formulaires].
