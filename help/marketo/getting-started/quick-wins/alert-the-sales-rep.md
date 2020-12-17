---
unique-page-id: 2359424
description: Alerte au représentant commercial - Documents marketing - Documentation du produit
title: Alerter le représentant commercial
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---


# Alerter le représentant commercial {#alert-the-sales-rep}

## Mission : Alerter le représentant commercial lorsqu&#39;une personne remplit un formulaire sur votre site Web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Pour envoyer automatiquement des e-mails d&#39;alerte aux représentants commerciaux, il vous suffit d&#39;envoyer un courriel d&#39;alerte et une campagne par courriel. Voici comment le faire.

>[!PREREQUISITES]
>
>[landing page avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

## Étape 1 : Créer un courriel d&#39;alerte {#step-create-an-alert-email}

1. Accédez à la zone **Activités marketing**.

   ![](assets/one-5.png)

1. Sélectionnez **Mon Programme** que vous avez créé dans le [Landing page avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) gagner rapidement, puis sous **Nouveau** cliquez sur **Nouveau fichier local**.

   ![](assets/two-6.png)

1. Cliquez sur **Courriel**.

   ![](assets/three-5.png)

1. **** Nommez l’adresse électronique &quot;My Email Alert&quot;, sélectionnez un modèle et cliquez sur  **Créer**.

   ![](assets/four-4.png)

1. Entrez **Du nom**, **Du courriel**, **Répondre à** et **Objet** que votre équipe commerciale doit voir.

   ![](assets/five-5.png)

1. Cliquez sur le doublon pour modifier le texte du courrier électronique.

   ![](assets/six-5.png)

1. Tapez le contenu du message.

   ![](assets/seven-6.png)

1. Placez le curseur à l’endroit où vous souhaitez insérer les coordonnées de la personne et cliquez sur l’icône **Insérer un jeton**.

   ![](assets/eight-4.png)

1. Recherchez et sélectionnez le `{{SP_Send_Alert_Info}}` **jeton** et cliquez sur **Insérer**.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} est un jeton spécial pour les messages d&#39;alerte. Voir [Utiliser le jeton d’informations d’alerte ](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) pour en savoir plus.

1. Cliquez sur **Enregistrer**.

   ![](assets/ten-5.png)

1. Fermez l’onglet/la fenêtre de l’éditeur de courrier électronique.

   ![](assets/eleven-5.png)

1. Sous **Actions de courriel**, cliquez sur **Approuver**.

   ![](assets/twelve-4.png)

## Étape 2 : Créer un déclencheur d&#39;alerte Campaign {#step-create-an-alert-trigger-campaign}

1. Sélectionnez **Mon Programme** créé précédemment, puis sous **New** cliquez sur **New Smart Campaign**.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **** Nommez la campagne &quot;My Alert Campaign&quot; et cliquez sur  **Create**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Sous l&#39;onglet **Liste intelligente**, recherchez et faites glisser le déclencheur **Remplit le formulaire** sur la trame.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Sélectionnez le formulaire que nous avons créé précédemment.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Sous l&#39;onglet **Flux**, recherchez et faites glisser l&#39;action de flux **Envoyer l&#39;alerte** vers le canevas.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Sélectionnez **Mon courriel d&#39;alerte** créé précédemment et laissez **Envoyer à** comme **propriétaire commercial**.

   ![](assets/eighteen-1.png)

1. Tapez votre adresse électronique dans le champ **À d’autres adresses électroniques**.

   ![](assets/nineteen-2.png)

1. Accédez à l&#39;onglet **Planification** et cliquez sur le bouton **Activer**.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >Définissez les **Règles de qualification** sur **à chaque fois** (en modifiant la Campaign dynamique) pour permettre à la même personne de déclencher des alertes à plusieurs reprises.

1. Cliquez sur **Activer** dans l’écran de confirmation.

   ![](assets/twenty-one-1.png)

## Étape 3 : Testez-Le ! {#step-test-it-out}

1. Sélectionnez votre landing page et cliquez sur **Vue Page approuvée**.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >N&#39;oubliez pas d&#39;approuver les landings page ; ils ne sont pas en direct avant d&#39;être approuvés.

1. Remplissez le formulaire et cliquez sur **Envoyer**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Vous devriez recevoir votre courriel sous peu. Une fois que vous avez vérifié que tout fonctionne comme il se doit, supprimez votre adresse électronique du flux Envoyer l&#39;alerte (voir l&#39;étape 2.7 ci-dessus).

   >[!NOTE]
   >
   >Cliquez sur l&#39;onglet **Informations sur la personne** dans Marketo pour afficher les informations de contact.

## Mission terminée ! {#mission-complete}

<br> 

[Mission 7 : Personnaliser un courriel](personalize-an-email.md)

[Mission 9 : Mettre à jour les données de piste ►](update-person-data.md)
