---
description: Règles de validation de formulaire globales - Documents Marketo - Documentation du produit
title: Règles de validation de formulaire globales
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
source-git-commit: 2736e8a0456de76b9894312c26f6ba9c0345daee
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Règles de validation de formulaire globales {#global-form-validation-rules}

Cette fonctionnalité vous permet de bloquer l’envoi de domaines spécifiques à des formulaires Marketo Engage.

## Comment activer l’accès {#how-to-enable-access}

Avant de pouvoir utiliser cette fonction, vous devez activer son autorisation selon le rôle souhaité.

1. Dans Marketo, cliquez sur **Administration**.

   ![](assets/global-form-validation-rules-1.png)

1. Cliquez sur **Utilisateurs et rôles**.

   ![](assets/global-form-validation-rules-2.png)

1. Cliquez sur le bouton **Rôles** .

   ![](assets/global-form-validation-rules-3.png)

1. Double-cliquez sur le rôle auquel vous souhaitez accorder des autorisations.

   ![](assets/global-form-validation-rules-4.png)

1. Cliquez sur le bouton **+** Connectez-vous en regard de Accès à l’administrateur.

   ![](assets/global-form-validation-rules-5.png)

1. Faites défiler la page vers le bas et sélectionnez **Accès aux règles de validation de formulaire** et cliquez sur **Enregistrer**.

   ![](assets/global-form-validation-rules-6.png)

## Créer une règle de validation de formulaire {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Ces règles s’appliqueront à tous les formulaires de vos abonnements de Marketo Engage.

1. Dans Marketo, cliquez sur **Administration**.

   ![](assets/global-form-validation-rules-7.png)

1. Cliquez sur **Règle de validation de formulaire globale**.

   ![](assets/global-form-validation-rules-8.png)

1. Cliquez sur **Nouvelle règle de validation de formulaire**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >La liste déroulante Actions de règle de validation de formulaire vous permet de supprimer ou de modifier des règles existantes.

1. Attribuez un nom à votre règle, fournissez-lui une description facultative, puis saisissez le message d’erreur que vous souhaitez que les visiteurs de votre formulaire voient. Saisissez le ou les domaines que vous souhaitez bloquer dans la zone Règles, puis sélectionnez **Activer la règle**, puis cliquez sur **Créer**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage dispose d’une liste bloquée définie de domaines d’e-mail de consommateur gratuits qui sont bloqués lors de l’utilisation de notre règle &quot;Liste bloquée de domaine d’e-mail de consommateur&quot; préchargée. [Afficher cette liste ici](/help/marketo/product-docs/administration/settings/assets/freemaildomains_2023.csv).

## Comment désactiver l’accès par formulaire{#how-to-disable-access-per-form}

Une fois activées, les règles s’appliquent à tous les formulaires. Toutefois, si vous disposez d’un formulaire avec des exigences spécifiques et que vous ne souhaitez rien refuser, vous pouvez désactiver les règles de validation de formulaire globales dans les paramètres du formulaire.

1. Dans le formulaire de votre choix, cliquez sur **Paramètres de formulaire**, puis **Paramètres**.

   ![](assets/global-form-validation-rules-11.png)

1. Cliquez sur la liste déroulante Règles de validation de formulaire globales , puis sélectionnez **Désactivé**.

   ![](assets/global-form-validation-rules-12.png)

Lorsque vous approuvez et publiez votre formulaire, il ignorera vos règles de validation de formulaire globales.
