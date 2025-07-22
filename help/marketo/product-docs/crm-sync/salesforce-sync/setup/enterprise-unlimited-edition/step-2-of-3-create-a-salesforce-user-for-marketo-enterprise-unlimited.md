---
unique-page-id: 2360364
description: Étape 2 sur 3 - Création d’un utilisateur Salesforce pour Marketo (Entreprise/Illimité) - Documents Marketo - Documentation du produit
title: Étape 2 sur 3 - Création d’un utilisateur Salesforce pour Marketo (Entreprise/Illimité)
exl-id: 871f335c-7b1e-47e1-8320-a18fbf21a970
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 3%

---

# Étape 2 sur 3 : création d’un utilisateur [!DNL Salesforce] pour Marketo (Entreprise/Illimité) {#step-of-create-a-salesforce-user-for-marketo-enterprise-unlimited}

>[!NOTE]
>
>Ces étapes doivent être effectuées par un administrateur [!DNL Salesforce]

>[!PREREQUISITES]
>
>[Étape 1 de 3 : ajouter des champs Marketo à  [!DNL Salesforce] (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)

Dans cet article, vous allez configurer des autorisations d’utilisateur dans [!DNL Salesforce] profil et créer un compte d’intégration Marketo-[!DNL Salesforce].

## Création d’un profil {#create-a-profile}

1. Cliquez sur **[!UICONTROL Configurer]**.

   ![](assets/image2015-6-11-16-3a15-3a27.png)

1. Saisissez « profiles » dans la barre de recherche de navigation, puis cliquez sur le lien **[!UICONTROL Profils]**.

   ![](assets/sfdc-profiles-hands.png)

1. Cliquez sur **[!UICONTROL Nouveau]**.

   ![](assets/image2014-12-9-9-3a19-3a15.png)

1. Sélectionnez **[!UICONTROL Utilisateur standard]**, nommez le profil « Marketo-Salesforce Sync » et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-12-9-9-3a19-3a22.png)

## Définir les autorisations de profil {#set-profile-permissions}

1. Cliquez sur **[!UICONTROL Modifier]** pour définir les autorisations de sécurité.

   ![](assets/image2014-12-9-9-3a19-3a30.png)

1. Dans la section **[!UICONTROL Autorisations d’administration]**, assurez-vous que les cases suivantes sont cochées :

   * [!UICONTROL API activé]
   * [!UICONTROL Modifier les modèles HTML]
   * [!UICONTROL Gestion des documents publics]
   * [!UICONTROL Gérer les modèles publics]

   ![](assets/image2014-12-9-9-3a19-3a38.png)

   >[!TIP]
   >
   >Veillez à cocher la case **[!UICONTROL Le mot de passe n’expire jamais]**.

1. Dans la section [!UICONTROL &#x200B; Autorisations générales des utilisateurs &#x200B;] , assurez-vous que les cases suivantes sont cochées :

   * [!UICONTROL Convertir les leads]
   * [!UICONTROL Modifier les événements]
   * [!UICONTROL Modifier tâches]

   ![](assets/image2014-12-9-9-3a19-3a47.png)

1. Dans la section [!UICONTROL &#x200B; Autorisations d’objet standard &#x200B;], assurez-vous que les autorisations [!UICONTROL Lecture, Création, Modification et Suppression] sont cochées pour :

   * [!UICONTROL Comptes]
   * [!UICONTROL Campagnes]
   * [!UICONTROL Contacts]
   * [!UICONTROL Leads]
   * [!UICONTROL &#x200B; Opportunités &#x200B;]

   >[!NOTE]
   >
   >Accordez des autorisations sur les [!UICONTROL Campagnes], si vous prévoyez d’utiliser la synchronisation de la campagne.

   ![](assets/image2014-12-9-9-3a19-3a57.png)

1. Lorsque vous avez terminé, cliquez sur **[!UICONTROL Enregistrer]** au bas de la page.

   ![](assets/image2014-12-9-9-3a20-3a5.png)

## Définir les autorisations de champ {#set-field-permissions}

1. Discutez avec vos spécialistes du marketing pour savoir quels champs personnalisés sont nécessaires à la synchronisation.

   >[!NOTE]
   >
   >Cette étape permet d’éviter l’affichage des champs dont vous n’avez pas besoin dans Marketo, ce qui réduit l’encombrement et accélère la synchronisation.

1. Dans la page des détails du profil, accédez à la section **[!UICONTROL Sécurité au niveau du champ]**. Cliquez sur **[!UICONTROL Affichage]** pour modifier l’accessibilité des objets :

   * [!UICONTROL Lead]
   * [!UICONTROL Contact]
   * [!UICONTROL Compte]
   * [!UICONTROL Opportunité]

   >[!TIP]
   >
   >Vous pouvez configurer d’autres objets en fonction des besoins de votre entreprise.

   ![](assets/image2014-12-9-9-3a20-3a14.png)

1. Pour chaque objet, cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/sfdc-sync-field-edit1.png)

1. Recherchez les champs inutiles et assurez-vous que les options **[!UICONTROL Accès en lecture]** et **[!UICONTROL Accès en modification]** ne sont pas cochées. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   >[!NOTE]
   >
   >Ne modifiez que l’accessibilité des champs personnalisés.

   ![](assets/sfdc-sync-field-edit2.png)

1. Une fois que vous avez désactivé tous les champs inutiles, vous devez vérifier **[!UICONTROL Accès en lecture et Accès en modification]** pour les champs d’objet suivants. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

<table> 
 <tbody> 
  <tr> 
   <th>Objet</th> 
   <th>Champs</th> 
  </tr> 
  <tr> 
   <td>Compte</td> 
   <td>Champ de type</td> 
  </tr> 
  <tr> 
   <td>Événement</td> 
   <td>Tous les champs</td> 
  </tr> 
  <tr> 
   <td>Tâche</td> 
   <td>Tous les champs</td> 
  </tr> 
 </tbody> 
</table>

![](assets/sfdc-check-the-boxes.png)

## Créer un compte de synchronisation Marketo-Salesforce {#create-marketo-salesforce-sync-account}

>[!TIP]
>
>Créez un compte [!DNL Salesforce] dédié (par exemple, marketo@yourcompany.com) pour distinguer les modifications apportées par Marketo des autres utilisateurs [!DNL Salesforce].

1. Saisissez « Gérer les utilisateurs » dans la barre de recherche de navigation, puis cliquez sur **[!UICONTROL Utilisateurs]**. Cliquez sur **[!UICONTROL Nouvel utilisateur]**.

   ![](assets/sfdc-new-users.png)

1. Renseignez les champs obligatoires. Sélectionnez ensuite le **[!UICONTROL Licence utilisateur : Salesforce]** et le profil que vous avez précédemment créé. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   ![](assets/image2014-12-9-9-3a20-3a56.png)

L’étape 2 sur 3 est terminée.

>[!NOTE]
>
>[Étape 3 sur 3 : connecter Marketo et [!DNL Salesforce] (Entreprise/Illimité)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
