---
unique-page-id: 2359424
description: Alerte du représentant commercial - Documents Marketo - Documentation du produit
title: Prévenir un représentant commercial
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
source-git-commit: 1127928b43762086ed4d157719ff80d6c3de9ee3
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 4%

---

# Prévenir un représentant commercial {#alert-the-sales-rep}

## Mission : Alerter le représentant commercial lorsqu’une personne remplit un formulaire sur votre site web {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Pour envoyer automatiquement des emails d’alerte aux représentants commerciaux, vous avez simplement besoin d’un email d’alerte et d’une campagne par e-mail. Voici comment le faire.

>[!PREREQUISITES]
>
>[Page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}

## Étape 1 : Créer un message d’alerte {#step-create-an-alert-email}

1. Accédez au **Activités marketing** zone.

   ![](assets/alert-the-sales-rep-1.png)

1. Sélectionner **Mon programme** que vous avez créé dans le [Page d’entrée avec un formulaire](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)gagnant rapide {target=&quot;_blank&quot;}, puis sous **Nouveau** click **Nouvelle ressource locale**.

   ![](assets/alert-the-sales-rep-2.png)

1. Cliquez sur **Email**.

   ![](assets/alert-the-sales-rep-3.png)

1. **Nom** Dans l&#39;email &quot;Mon email d&#39;alerte&quot;, sélectionnez un modèle et cliquez sur **Créer**.

   ![](assets/alert-the-sales-rep-4.png)

1. Saisissez le **De nom**, **À partir du courrier électronique**, **Réponse**, et **Objet** que vous souhaitez voir votre équipe de vente.

   ![](assets/alert-the-sales-rep-5.png)

1. Faites un double-clic pour modifier le corps de l&#39;e-mail.

   ![](assets/alert-the-sales-rep-6.png)

1. Saisissez le contenu de l&#39;email.

   ![](assets/alert-the-sales-rep-7.png)

1. Positionnez-vous à l&#39;endroit où vous souhaitez insérer les coordonnées de la personne et cliquez sur le bouton **Insérer un jeton** icône .

   ![](assets/alert-the-sales-rep-8.png)

1. Recherchez et sélectionnez la variable `{{SP_Send_Alert_Info}}` **Jeton** et cliquez sur **Insérer**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} est un jeton spécial pour les emails d’alerte. Voir [Utiliser le jeton d’information d’alerte Envoyer](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;}{target=&quot;_blank&quot;} pour en savoir plus.

1. Cliquez sur **Enregistrer**.

   ![](assets/alert-the-sales-rep-10.png)

1. Cliquez sur le bouton **Actions de courrier électronique** et sélectionnez **Approuver et fermer**.

   ![](assets/alert-the-sales-rep-11.png)

## Étape 2 : Création d’une campagne de déclenchement d’alertes {#step-create-an-alert-trigger-campaign}

1. Sélectionner **Mon programme** créé précédemment, puis sous **Nouveau** click **Nouvelle campagne dynamique**.

   ![](assets/alert-the-sales-rep-12.png)

1. **Nom** dans la campagne &quot;Ma campagne d’alerte&quot;, puis cliquez sur **Créer**.

   ![](assets/alert-the-sales-rep-13.png)

1. Sous , **Liste dynamique** , recherchez et faites glisser l’objet **Remplir le formulaire** se déclenche dans la zone de travail.

   ![](assets/alert-the-sales-rep-14.png)

1. Sélectionnez le formulaire que nous avons créé précédemment.

   ![](assets/alert-the-sales-rep-15.png)

1. Sous , **Flux** , recherchez et faites glisser l’objet **Envoyer une alerte** action de flux vers la zone de travail.

   ![](assets/alert-the-sales-rep-16.png)

1. Sélectionner **Mon courriel d’alerte** créé précédemment et laissé **Envoyer à** as **Propriétaire des ventes**.

   ![](assets/alert-the-sales-rep-17.png)

1. Saisissez votre adresse électronique dans le champ **À d’autres courriers électroniques** champ .

   ![](assets/alert-the-sales-rep-18.png)

1. Accédez au **Planification** et cliquez sur l’onglet **Activer** bouton .

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >Définissez la variable **Règles de qualification** to **à chaque heure** (en modifiant la campagne dynamique) pour permettre à la même personne de déclencher des alertes plusieurs fois.

1. Cliquez sur **Activer** sur l’écran de confirmation.

   ![](assets/alert-the-sales-rep-20.png)

## Étape 3 : Testez-Le ! {#step-test-it-out}

1. Sélectionnez votre landing page et cliquez sur **Afficher la page approuvée**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >N’oubliez pas de valider les landing pages. ils ne restent pas en vie jusqu&#39;à ce qu&#39;ils soient approuvés.

1. Remplissez le formulaire et cliquez sur **Envoyer**.

   ![](assets/alert-the-sales-22.png)

1. Vous devriez recevoir votre email sous peu. Une fois que vous avez vérifié que tout fonctionne comme prévu, supprimez votre adresse électronique du flux Envoyer une alerte (voir l’étape 2.7 ci-dessus).

   >[!NOTE]
   >
   >Cliquez sur le bouton **Informations sur la personne** dans Marketo pour afficher les coordonnées.

## Mission accomplie! {#mission-complete}

<br> 

[◄ Mission 7 : Personnaliser un e-mail](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Mission 9 : Mettre à jour les ► de données de personne](/help/marketo/getting-started/quick-wins/update-person-data.md)
