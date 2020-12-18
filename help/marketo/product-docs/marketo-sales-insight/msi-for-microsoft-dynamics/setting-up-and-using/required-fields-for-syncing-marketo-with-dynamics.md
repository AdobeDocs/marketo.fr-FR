---
unique-page-id: 11375827
description: Champs requis pour la synchronisation du marché avec Dynamics - Marketo Docs - Documentation sur les produits
title: Champs requis pour synchroniser le marketing avec Dynamics
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---


# Champs requis pour synchroniser le marketing avec Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Ces champs *doivent* être synchronisés avec Marketo pour que le prospect et le contact pour que Sales Insight fonctionnent :

* Priorité
* Urgence
* Note relative

Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour corriger ce problème, archivez votre instance pour vous assurer que les champs sont synchronisés pour **Lead** et **Contact**. Sinon, ajoutez-les.

Voici comment vérifier et ajouter des champs de synchronisation.

1. Accédez à Admin et cliquez sur Microsoft Dynamics.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur Modifier dans Détails de synchronisation des champs.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Sous Piste, cochez la case Priorité.

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Défilez maintenant et cochez la case Urgence...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...et la case à cocher Note relative.

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Cochez ensuite les cases Priorité, Urgence et Score relatif pour le contact.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Cliquez sur Enregistrer.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Veillez à patienter au moins 10 minutes pour qu’une synchronisation s’exécute avant de vérifier que vous avez corrigé le problème.

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de piste/contact](http://docs.marketo.com/x/BICMAg)

