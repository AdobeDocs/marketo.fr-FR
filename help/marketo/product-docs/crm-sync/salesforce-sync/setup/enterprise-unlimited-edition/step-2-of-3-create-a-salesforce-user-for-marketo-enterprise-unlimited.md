---
unique-page-id: 2360364
description: Étape 2 sur 3 - Création d’un utilisateur Salesforce pour Marketo (Enterprise/Unlimited) - Documents Marketo - Documentation du produit
title: Étape 2 sur 3 - Création d’un utilisateur Salesforce pour Marketo (Enterprise/Unlimited)
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 4%

---

# Étape 2 sur 3 : Création d’un utilisateur Salesforce pour Marketo (Enterprise/Unlimited) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Ces étapes doivent être effectuées par un administrateur Salesforce

>[!PREREQUISITES]
>
>[Étape 1 sur 3 : Ajout de champs Marketo à Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

Dans cet article, vous allez configurer des autorisations utilisateur dans le profil Salesforce et créer un compte d’intégration Marketo-Salesforce.

## Création d’un profil {#create-a-profile}

1. Cliquez sur **Configuration**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Saisissez &quot;profils&quot; dans la barre de recherche de navigation, puis cliquez sur le **Profils** lien.

   ![](assets/sfdc-profiles-hands.png)

1. Cliquez sur **Nouveau**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Sélectionner **Utilisateur standard**, nommez le profil &quot;Marketo-Salesforce Sync&quot; et cliquez sur **Enregistrer**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Définition des autorisations de profil {#set-profile-permissions}

1. Cliquez sur **Modifier** pour définir les autorisations de sécurité.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Sous , **Autorisations administratives** , vérifiez que les cases suivantes sont cochées :

   * API activée
   * Modifier les modèles de HTML
   * Gérer les documents publics
   * Gérer les modèles publics

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Veillez à vérifier la variable **Le mot de passe n’expire jamais** de la boîte.

1. Dans la section Autorisations des utilisateurs générales , assurez-vous que les cases suivantes sont cochées :

   * Convertir les pistes
   * Modifier des événements
   * Modifier les tâches

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Dans la section Autorisations d’objet standard , assurez-vous que les autorisations de lecture, de création, de modification et de suppression sont cochées pour :

   * Comptes
   * Campagnes
   * Contacts
   * Leads
   * Opportunités

   >[!NOTE]
   >
   >Octroyez des autorisations aux campagnes si vous envisagez d’utiliser la synchronisation des campagnes.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Lorsque vous avez terminé, cliquez sur **Enregistrer** au bas de la page.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Définition des autorisations de champ {#set-field-permissions}

1. Discutez avec vos spécialistes du marketing pour déterminer les champs personnalisés à synchroniser.

   >[!NOTE]
   >
   >Cette étape permet d’éviter que les champs dont vous n’avez pas besoin ne s’affichent dans Marketo, ce qui réduit l’encombrement et accélère la synchronisation.

1. Dans la page des détails du profil, accédez à **Sécurité au niveau du champ** . Cliquez sur **Affichage** pour modifier l’accessibilité des objets :

   * Lead
   * Contact
   * Compte
   * Opportunité

   >[!TIP]
   >
   >Vous pouvez configurer d’autres objets en fonction des besoins de votre entreprise.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Pour chaque objet, cliquez sur **Modifier**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Recherchez les champs inutiles, assurez-vous que la variable **Accès en lecture** et **Modifier l’accès** ne sont pas cochées. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   >[!NOTE]
   >
   >Modifiez uniquement l’accessibilité pour les champs personnalisés.

   ![](assets/sfdc-sync-field-edit2.png)

1. Après avoir désactivé tous les champs superflus, vous devez cocher la case **Accès en lecture et accès en modification** pour les champs d’objet suivants. Cliquez sur **Enregistrer** lorsque vous avez terminé.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1"><p>Objet</p></th> 
   <th colspan="1" rowspan="1"><p>Champs</p></th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Compte</p></td> 
   <td colspan="1" rowspan="1"><p>Champ de type</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Événement</p></td> 
   <td colspan="1" rowspan="1"><p>Tous les champs</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Tâche</p></td> 
   <td colspan="1" rowspan="1"><p>Tous les champs</p></td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## Créer un compte de synchronisation Marketo-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Créez un compte Salesforce dédié (marketo@yourcompany.com, par exemple) pour distinguer les modifications effectuées par Marketo des autres utilisateurs Salesforce.

1. Saisissez &quot;Gérer les utilisateurs&quot; dans la barre de recherche de navigation, puis cliquez sur **Utilisateurs**. Cliquez sur **Nouvel utilisateur**.

   ![](assets/sfdc-new-users.png)

1. Renseignez les champs requis. Sélectionnez ensuite le **Licence utilisateur : Salesforce** et le profil que vous avez créé précédemment. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

Les étapes 2 sur 2 sont terminées.

>[!NOTE]
>
>[Étape 3 sur 3 : Connexion de Marketo et de Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
