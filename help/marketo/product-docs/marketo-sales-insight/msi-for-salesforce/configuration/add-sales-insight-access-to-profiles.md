---
description: Ajout d’un accès Sales Insight aux profils - Documents Marketo - Documentation du produit
title: Ajouter un accès à Informations sur les ventes aux profils
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 5%

---

# Ajouter un accès [!DNL Sales Insight] aux profils {#add-sales-insight-access-to-profiles}

Voici comment créer un profil ayant accès à [!DNL Sales Insight] tout en supprimant l’accès pour vos autres profils. Ceci est destiné aux utilisateurs qui ont déjà installé le package [[!DNL Sales Insight] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Si vous avez précédemment accordé un accès [!DNL Sales Insight] à tous les profils, vous devez [supprimer l’accès au niveau du profil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} pour utiliser ce jeu d’autorisations.

## Créer un profil pour [!DNL Sales Insight] {#create-a-new-profile-for-sales-insight}

Si vous disposez d’un profil dédié pour vos utilisateurs [!DNL Sales Insight], vous pouvez ignorer cette étape.

1. Dans [!DNL Salesforce], accédez à la page Configuration .

1. Recherchez des profils dans la recherche rapide et sélectionnez l’option **[!UICONTROL Profil]**.

1. Cliquez sur le bouton **[!UICONTROL Nouveau profil]** en haut de la page.

1. Sélectionnez un profil à cloner et donnez-lui un nom (par exemple : utilisateur Sales Insight).

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

## Ajout d’autorisations [!DNL Sales Insight] {#add-sales-insight-permissions}

1. Revenez à votre liste Profils .

1. Cliquez sur le lien **[!UICONTROL Modifier]** pour le nouveau profil que vous venez de créer (ou tout autre profil existant auquel vous souhaitez accorder un accès [!DNL Sales Insight]).

1. Sur la page de modification, vous devez modifier certains paramètres.

   **Pour les profils autorisés à accéder[!DNL Sales Insight]** :

   * Dans Paramètres d’onglet, activez par défaut les onglets Marketo
   * Dans Autorisations d’objets personnalisés, cochez Lecture, Créer, Modifier et Supprimer dans [!DNL Marketo Sales Insight] configuration (si l’utilisateur doit avoir accès aux paramètres de configuration, généralement utilisés pour les administrateurs)

   **Pour les profils dont l’accès aux[!DNL Sales Insight]** n’est pas autorisé :

   * Dans Paramètres d’onglet, modifiez les onglets Marketo en Onglet masqué.
   * Dans Autorisations d’objet personnalisé, désélectionnez Lecture, Créer, Modifier et Supprimer sur [!DNL Marketo Sales Insight] configuration

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

## Créer une mise en page pour [!DNL Sales Insight] {#create-layout-for-sales-insight}

1. Accédez à la page Configuration, puis cliquez sur **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Personnaliser]** > **[!UICONTROL Leads]** > **[!UICONTROL Mises en page]**. Cliquez ensuite sur le bouton **[!UICONTROL Nouveau]**.

1. Clonez la mise en page de votre choix et donnez-lui un nom approprié (par exemple : Mise en page Sales Insight).

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

1. Répétez ces étapes pour vos mises en page [!UICONTROL Contacts], [!UICONTROL Opportunités] et [!UICONTROL Comptes].

## Attribuer un profil à la mise en page {#assign-profile-to-layout}

1. Revenez à la section Mises en page et cliquez sur le bouton **[!UICONTROL Affectation de la mise en page]**.

1. Sélectionnez **[!UICONTROL Modifier l’affectation]**.

1. Sélectionnez le profil de votre [!DNL Sales Insight] dans la liste, puis sélectionnez la mise en page de votre [!DNL Sales insight] dans le menu déroulant « [!UICONTROL  Sélectionner la mise en page ] ».

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

1. Répétez ces étapes pour vos mises en page [!UICONTROL Contacts], [!UICONTROL Opportunités] et [!UICONTROL Comptes].

## Autres modifications {#other-changes}

Voici d’autres endroits où des éléments [!DNL Sales Insight] peuvent apparaître. Vous devrez les supprimer définitivement, car vous ne pouvez pas utiliser les profils pour limiter leur accès :

* Supprimez [!DNL Sales Insight] boutons des mises en page de recherche pour [!UICONTROL Contacts], [!UICONTROL Prospects] et [!UICONTROL Comptes]
* Supprimer [!DNL Sales Insight] colonnes des listes de contacts et de leads
