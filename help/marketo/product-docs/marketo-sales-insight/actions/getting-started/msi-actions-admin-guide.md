---
description: Guide d’administration des actions MSI - Documents Marketo - Documentation du produit
title: Guide d’administration des actions MSI
hide: true
hidefromtoc: true
source-git-commit: 55a677339f03b11ac3c2bdf58fdb83fdbd1cd4b8
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 2%

---

# Guide d’administration des actions MSI {#msi-actions-admin-guide}

>[!PREREQUISITES]
>
>* Confirmez auprès de votre gestionnaire de succès client que les actions MSI ont été activées pour votre compte Marketo (si vous ne disposez pas d’un CSM, veuillez [Contacter l’assistance](https://nation.marketo.com/t5/support/ct-p/Support)).
>* Votre synchronisation Marketo/Salesforce doit être configurée.


<table>
 <tr>
  <th>Persona</th>
  <th>Étape</th>
 </tr>
 <tr>
  <td>Administrateur Marketo</td>
  <td>Configuration du compte de ventes Marketo</td>
 </tr>
 <tr>
  <td>Administrateur Marketo ou <br/>Administration Salesforce</td>
  <td>Connexion du compte Ventes Marketo à Salesforce</td>
 </tr>
 <tr>
  <td>Administrateur Marketo</td>
  <td>Connexion du compte de ventes Marketo à Marketo</td>
 </tr>
 <tr>
  <td>Administrateur Marketo</td>
  <td>Lancer la synchronisation des données de Marketo vers le compte de vente Marketo</td>
 </tr>
 <tr>
  <td>Administrateur Marketo</td>
  <td>Invitation d’utilisateurs à des MSI-Actions</td>
 </tr>
 <tr>
  <td>Administration Salesforce</td>
  <td>Installer/mettre à niveau le package MSI dans Salesforce</td>
 </tr>
 <tr>
  <td>Administration Salesforce</td>
  <td>Configuration des MSI-Actions dans Salesforce</td>
 </tr>
</table>

## Configuration du compte de vente Marketo {#set-up-marketo-sales-account}

1. Dans Marketo, cliquez sur **Administration**.

   ![](assets/msi-actions-admin-guide-1.png)

1. Cliquez sur **Statistiques des ventes**, puis **Configuration des actions**. Sélectionnez dans la liste des administrateurs Marketo à inviter et cliquez sur **Envoyer une invitation**.

   ![](assets/msi-actions-admin-guide-2.png)

L’utilisateur recevra un e-mail lui indiquant les étapes pour accéder au compte.

>[!NOTE]
>
>D’autres utilisateurs ne seront pas ajoutés via Marketo, mais par la page Gestion des utilisateurs du compte de vente . [Cliquez ici](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md) pour en savoir plus sur l’ajout d’utilisateurs supplémentaires.

## Connexion du compte de ventes Marketo à Salesforce {#connect-marketo-sales-account-to-salesforce}

1. Dans votre compte Marketo Sales, cliquez sur l’icône représentant un engrenage et sélectionnez **Paramètres**.

   ![](assets/msi-actions-admin-guide-3.png)

1. Sous Paramètres d’administration, cliquez sur **Salesforce**.

   ![](assets/msi-actions-admin-guide-4.png)

1. Dans l’onglet Connexions et personnalisations , cliquez sur **Connexion**.

   ![](assets/msi-actions-admin-guide-5.png)

1. Cliquez sur **OK**.

   ![](assets/msi-actions-admin-guide-6.png)

Si vous êtes déjà connecté à Salesforce, vous serez connecté. Si ce n’est pas le cas, vous serez invité à vous connecter.

## Connexion de Marketo à votre compte d’applications de vente {#connect-marketo-to-your-sales-apps-account}

1. Dans votre compte Marketo Sales, cliquez sur l’icône représentant un engrenage et sélectionnez **Paramètres**.

   ![](assets/msi-actions-admin-guide-7.png)

1. Sous Paramètres d’administration, cliquez sur **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. Cliquez sur **connect**. Votre compte sera alors connecté.

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>S’il ne se connecte pas, copiez les informations d’identification de l’onglet &quot;Configuration des actions&quot; de Marketo Sales Insight et collez-les dans l’onglet Configuration .

## Lancer la synchronisation des données {#initiate-data-sync}

1. Dans Marketo, cliquez sur **Administration**.

   ![](assets/msi-actions-admin-guide-10.png)

1. Cliquez sur Sales Insight .

   ![](assets/msi-actions-admin-guide-11.png)

1. Cliquez sur l’onglet Configuration des actions . Dans la carte Synchronisation des champs d’action , cliquez sur **Synchronisation**.

   ![](assets/msi-actions-admin-guide-12.png)

1. Vous verrez un aperçu des champs qui seront synchronisés. Cliquez sur **Démarrer la synchronisation**.

   ![](assets/msi-actions-admin-guide-13.png)

Les enregistrements de personne existant dans Marketo et Salesforce seront synchronisés dans votre compte Applications commerciales Marketo.

## Invitation d’utilisateurs individuels dans des actions MSI {#invite-individual-users-to-msi-actions}

1. Dans votre compte Marketo Sales, cliquez sur l’icône représentant un engrenage et sélectionnez **Paramètres**.

   ![](assets/msi-actions-admin-guide-14.png)

1. Sous Paramètres d’administration, sélectionnez **Gestion des utilisateurs**.

   ![](assets/msi-actions-admin-guide-15.png)

1. Cliquez sur **Actions** et sélectionnez **Invitation d’utilisateurs**.

   ![](assets/msi-actions-admin-guide-16.png)

1. Saisissez la ou les adresses email et cliquez sur **Invitation**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>Par défaut, tous les nouveaux membres seront ajoutés à l’équipe Tous .

Vous recevrez un message de confirmation.

## Invitation d’utilisateurs via CSV à des actions MSI {#invite-users-via-csv-to-msi-actions}

1. Dans votre compte Marketo Sales, cliquez sur l’icône représentant un engrenage et sélectionnez **Paramètres**.

   ![](assets/msi-actions-admin-guide-18.png)

1. Sous Paramètres d’administration, sélectionnez **Gestion des utilisateurs**.

   ![](assets/msi-actions-admin-guide-19.png)

1. Cliquez sur **Actions** et sélectionnez **Invitation d’utilisateurs via CSV**.

   ![](assets/msi-actions-admin-guide-20.png)

1. Recherchez le fichier CSV sur votre ordinateur, sélectionnez-le, puis cliquez sur **Suivant**.

   ![](assets/msi-actions-admin-guide-21.png)

1. Vérifiez que les champs sont correctement mappés et cliquez sur **Invitation**.

   ![](assets/msi-actions-admin-guide-22.png)

Vous recevrez un message de confirmation une fois les invitations envoyées.

>[!NOTE]
>
>Une fois cette opération effectuée, vous pouvez soit mettre à niveau votre package MSI existant, soit en installer un nouveau et passer à [configuration des actions MSI dans Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/salesforce-configuration/msi-actions-configuration-in-salesforce.md).