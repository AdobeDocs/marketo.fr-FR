---
unique-page-id: 2359424
description: Alerte le représentant commercial - Documents Marketo - Documentation du produit
title: Prévenir un représentant commercial
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 2%

---

# Prévenir un représentant commercial {#alert-the-sales-rep}

## Mission : alerter le représentant commercial lorsqu’une personne remplit un formulaire sur votre site web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Pour envoyer automatiquement des emails d’alerte aux représentants commerciaux, vous avez simplement besoin d’un email d’alerte et d’une campagne par e-mail. Voici comment le faire.

>[!PREREQUISITES]
>
>[Page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Étape 1 : création d’un email d’alerte {#step-create-an-alert-email}

1. Accédez à la zone **[!UICONTROL Activités marketing]**.

   ![](assets/alert-the-sales-rep-1.png)

1. Sélectionnez **Mon programme** que vous avez créé dans la [Landing Page with a Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} quick win, puis, sous **[!UICONTROL New]**, cliquez sur **[!UICONTROL New Local Asset]**.

   ![](assets/alert-the-sales-rep-2.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/alert-the-sales-rep-3.png)

1. **Nommez** l’e-mail &quot;My Email Alert&quot;, sélectionnez un modèle et cliquez sur **[!UICONTROL Create]**.

   ![](assets/alert-the-sales-rep-4.png)

1. Saisissez les **From Name**, **From Email**, **[!UICONTROL Reply-to]** et **[!UICONTROL Subject]** que votre équipe de vente doit voir.

   ![](assets/alert-the-sales-rep-5.png)

1. Double-cliquez pour éditer le texte de l&#39;email.

   ![](assets/alert-the-sales-rep-6.png)

1. Saisissez le contenu de l&#39;email.

   ![](assets/alert-the-sales-rep-7.png)

1. Placez le curseur à l’endroit où vous souhaitez insérer les coordonnées de la personne et cliquez sur l’icône **Insérer un jeton** .

   ![](assets/alert-the-sales-rep-8.png)

1. Recherchez et sélectionnez le `{{SP_Send_Alert_Info}}` **[!UICONTROL Jeton]** et cliquez sur **[!UICONTROL Insérer]**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} est un jeton spécial pour les emails d’alerte. Pour en savoir plus, voir [Utilisation du jeton d’informations sur les alertes d’envoi](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"} .

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/alert-the-sales-rep-10.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Actions de courrier électronique]** et sélectionnez **[!UICONTROL Approuver et fermer]**.

   ![](assets/alert-the-sales-rep-11.png)

## Etape 2 : création d&#39;une campagne de déclenchement d&#39;alertes {#step-create-an-alert-trigger-campaign}

1. Sélectionnez **Mon programme** créé précédemment, puis, sous **[!UICONTROL Nouveau]**, cliquez sur **[!UICONTROL Nouvelle campagne dynamique]**.

   ![](assets/alert-the-sales-rep-12.png)

1. **Nommez** la campagne &quot;Ma campagne d’alerte&quot; et cliquez sur **[!UICONTROL Créer]**.

   ![](assets/alert-the-sales-rep-13.png)

1. Sous l’onglet **[!UICONTROL Liste dynamique]**, recherchez et faites glisser le déclencheur **[!UICONTROL Remplit le formulaire]** sur la zone de travail.

   ![](assets/alert-the-sales-rep-14.png)

1. Sélectionnez le formulaire que nous avons créé précédemment.

   ![](assets/alert-the-sales-rep-15.png)

1. Sous l’onglet **[!UICONTROL Flux]** , recherchez et faites glisser l’action de flux **[!UICONTROL Envoyer l’alerte]** vers la zone de travail.

   ![](assets/alert-the-sales-rep-16.png)

1. Sélectionnez **[!UICONTROL Mon e-mail d’alerte]** créé précédemment et laissez **[!UICONTROL Envoyer à]** comme **[!UICONTROL propriétaire des ventes]**.

   ![](assets/alert-the-sales-rep-17.png)

1. Saisissez votre adresse électronique dans le champ **[!UICONTROL À d’autres messages électroniques]** .

   ![](assets/alert-the-sales-rep-18.png)

1. Accédez à l’onglet **[!UICONTROL Schedule]** et cliquez sur le bouton **[!UICONTROL Activer]** .

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >Définissez les **[!UICONTROL règles de qualification]** sur **[!UICONTROL chaque fois]** (en modifiant la campagne dynamique) pour permettre à la même personne de déclencher des alertes plusieurs fois.

1. Cliquez sur **[!UICONTROL Activer]** dans l’écran de confirmation.

   ![](assets/alert-the-sales-rep-20.png)

## Étape 3 : Testez-Le ! {#step-test-it-out}

1. Sélectionnez votre landing page et cliquez sur **[!UICONTROL Afficher la page approuvée]**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >N&#39;oubliez pas d&#39;approuver les landing pages ; elles ne sont pas mises en ligne avant approbation.

1. Remplissez le formulaire et cliquez sur **[!UICONTROL Submit]**.

   ![](assets/alert-the-sales-22.png)

1. Vous devriez recevoir votre email sous peu. Une fois que vous avez vérifié que tout fonctionne comme prévu, supprimez votre adresse électronique du flux Envoyer une alerte (voir l’étape 2.7 ci-dessus).

   >[!NOTE]
   >
   >Cliquez sur l’onglet **[!UICONTROL Informations sur la personne]** de Marketo pour afficher les informations de contact.

## Mission terminée ! {#mission-complete}

<br> 

[◄ Mission 7 : personnaliser un email](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Mission 9 : mise à jour des données de personne ►](/help/marketo/getting-started/quick-wins/update-person-data.md)
