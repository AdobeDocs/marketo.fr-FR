---
description: Guide de configuration des actions Sales Insight - Documents Marketo - Documentation du produit
title: Guide de configuration des actions Sales Insight
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 1%

---

# Guide de configuration des actions Sales Insight {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>Marketo Sales Insight Actions est une application web qui s’intègre à l’interface utilisateur de Salesforce via le [package Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. On parle parfois de &quot;ventes Marketo&quot; ou simplement de &quot;actions&quot;.

>[!PREREQUISITES]
>
>* Confirmez auprès de l’équipe du compte d’Adobe (votre gestionnaire de compte) que les actions MSI ont été activées pour votre compte de Marketo Engage (si vous n’avez pas de gestionnaire de compte, contactez l’[assistance Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}).
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
  <td>Administrateur Marketo ou <br/> administrateur Salesforce</td>
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

1. Dans Marketo, cliquez sur **Admin**.

   ![](assets/msi-actions-admin-guide-1.png)

   >[!NOTE]
   >
   >Si vous ne voyez pas d’ID de client et de secret de client sur la carte Informations sur l’intégration, activez votre instance Actions en invitant le premier utilisateur. L’ID de client et le secret de client s’affichent alors.

1. Cliquez sur **Sales Insight**, puis sur **Actions Config**. Sélectionnez dans la liste des administrateurs Marketo à inviter et cliquez sur **Envoyer l’invitation**.

   ![](assets/msi-actions-admin-guide-2.png)

L’utilisateur recevra un e-mail lui indiquant les étapes pour accéder au compte.

>[!NOTE]
>
>D’autres utilisateurs ne seront pas ajoutés via Marketo, mais par la page Gestion des utilisateurs du compte de vente . [Cliquez ici](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"} pour en savoir plus sur l’ajout d’utilisateurs supplémentaires.

## Connexion du compte de ventes Marketo à Salesforce {#connect-marketo-sales-account-to-salesforce}

1. Dans votre compte Marketo Sales, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/msi-actions-admin-guide-3.png)

1. Sous Paramètres d’administration, cliquez sur **Salesforce**.

   ![](assets/msi-actions-admin-guide-4.png)

1. Dans l’onglet Connexions et personnalisations , cliquez sur **Se connecter**.

   ![](assets/msi-actions-admin-guide-5.png)

1. Cliquez sur **OK**.

   ![](assets/msi-actions-admin-guide-6.png)

Si vous êtes déjà connecté à Salesforce, vous serez connecté. Si ce n&#39;est pas le cas, on vous demandera de vous connecter.

## Connexion de Marketo à votre compte d’applications de vente {#connect-marketo-to-your-sales-apps-account}

1. Dans votre compte Marketo Sales, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/msi-actions-admin-guide-7.png)

1. Sous Paramètres d’administration, cliquez sur **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. Cliquez sur **connect**. Votre compte sera alors connecté.

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>S’il ne se connecte pas, copiez les informations d’identification de l’onglet &quot;Configuration des actions&quot; de Marketo Sales Insight et collez-les dans l’onglet Configuration .

## Lancer la synchronisation des données {#initiate-data-sync}

La synchronisation des champs d’unification des données pour les actions d’aperçu des ventes permet au système d’extraire des informations sur les personnes de votre base de données de Marketo Engage dans votre base de données d’actions d’aperçu des ventes, de mettre à jour les données de vos personnes et de s’assurer que les activités sont consignées dans les bons enregistrements dans Marketo et Salesforce.

>[!CAUTION]
>
>Une fois que vous avez lancé la synchronisation des données, vous devez **et non** supprimer l’utilisateur d’origine sur votre instance d’actions Sales Insight. Il s’agit de l’utilisateur auquel la première invitation a été envoyée.

1. Dans Marketo, cliquez sur **Admin**.

   ![](assets/msi-actions-admin-guide-10.png)

1. Cliquez sur **Sales Insight**.

   ![](assets/msi-actions-admin-guide-11.png)

1. Cliquez sur l’onglet **Configuration des actions** . Dans la carte Synchronisation des champs d’action , cliquez sur **Synchroniser**.

   ![](assets/msi-actions-admin-guide-12.png)

1. Vous verrez un aperçu des champs qui seront synchronisés. Cliquez sur **Démarrer la synchronisation**.

   ![](assets/msi-actions-admin-guide-13.png)

Les enregistrements de personne existant dans Marketo et Salesforce seront synchronisés dans votre compte Applications commerciales Marketo.

>[!NOTE]
>
>Pour en savoir plus sur la façon dont les personnes et les données d’activité se synchronisent entre les actions Sales Insight, Marketo et Salesforce, [ cliquez ici](/help/marketo/product-docs/marketo-sales-insight/actions/admin/sync-sales-action-data-with-marketo-and-salesforce.md){target="_blank"}.

## Invitation d’utilisateurs individuels dans des actions MSI {#invite-individual-users-to-msi-actions}

1. Dans votre compte Marketo Sales, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/msi-actions-admin-guide-14.png)

1. Sous Paramètres d’administration, sélectionnez **Gestion utilisateur**.

   ![](assets/msi-actions-admin-guide-15.png)

1. Cliquez sur **Actions** et sélectionnez **Inviter des utilisateurs**.

   ![](assets/msi-actions-admin-guide-16.png)

1. Saisissez la ou les adresses email et cliquez sur **Inviter**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>Par défaut, tous les nouveaux membres seront ajoutés à l’équipe Tous .

Vous recevrez un message de confirmation.

## Invitation d’utilisateurs via CSV à des actions MSI {#invite-users-via-csv-to-msi-actions}

1. Dans votre compte Marketo Sales, cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/msi-actions-admin-guide-18.png)

1. Sous Paramètres d’administration, sélectionnez **Gestion utilisateur**.

   ![](assets/msi-actions-admin-guide-19.png)

1. Cliquez sur **Actions** et sélectionnez **Inviter des utilisateurs via CSV**.

   ![](assets/msi-actions-admin-guide-20.png)

1. Recherchez le fichier CSV sur votre ordinateur, sélectionnez-le, puis cliquez sur **Suivant**.

   ![](assets/msi-actions-admin-guide-21.png)

1. Vérifiez que les champs sont correctement mappés et cliquez sur **Invite**.

   ![](assets/msi-actions-admin-guide-22.png)

Vous recevrez un message de confirmation une fois que les invitations seront envoyées.

>[!NOTE]
>
>Une fois cela fait, vous pouvez soit mettre à niveau votre package MSI existant, soit en installer un nouveau et passer à la [configuration des actions MSI dans Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"}.
