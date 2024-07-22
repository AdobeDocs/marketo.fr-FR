---
unique-page-id: 11375827
description: Champs requis pour la synchronisation de Marketo avec Dynamics - Documents Marketo - Documentation du produit
title: Champs requis pour la synchronisation de Marketo avec Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 3%

---

# Champs requis pour la synchronisation de Marketo avec Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Ces champs *doivent* être synchronisés avec Marketo pour que le prospect et le contact de Sales Insight fonctionnent :

* Priorité
* Urgence
* Évaluation relative

Si l’un de ces champs est manquant, un message d’erreur s’affiche dans Marketo avec le nom des champs manquants. Pour résoudre ce problème, archivez votre instance pour vous assurer que les champs sont synchronisés pour **Lead** et **Contact**. Dans le cas contraire, ajoutez-les.

Voici comment vérifier et ajouter des champs de synchronisation.

1. Accédez à Admin et cliquez sur **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Cliquez sur **Modifier** sur Détails de la synchronisation des champs.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Sous Piste, cochez la case Priorité .

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Maintenant, faites défiler la page vers le bas et cochez la case Urgence ...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...et la case à cocher Score relatif .

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Cochez ensuite les cases Priorité, Urgence et Score relatif pour Contact.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Veillez à attendre au moins 10 minutes qu’une synchronisation s’exécute avant de vérifier que vous avez corrigé le problème.

>[!MORELIKETHIS]
>
>[Configuration des étoiles et des flammes pour les enregistrements de piste/contact](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
