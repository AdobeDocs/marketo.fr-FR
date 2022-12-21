---
unique-page-id: 1147066
description: Remplacement des restrictions de personne dans une campagne dynamique - Documents Marketo - Documentation du produit
title: Remplacement des restrictions de personne dans une campagne dynamique
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Remplacement des restrictions de personne dans une campagne dynamique {#override-person-restrictions-in-a-smart-campaign}

Marketo vous permet de définir le nombre maximal de personnes qui peuvent être qualifiées pour une campagne dynamique ; vous évitez ainsi d’envoyer accidentellement par courrier électronique l’ensemble de votre base de données. Si vous voulez _override_ cette limite, voilà comment.

>[!PREREQUISITES]
>
>Veillez à [activation des restrictions de personne pour les campagnes intelligentes](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) dans l’administration Marketo.

1. Dans Activités marketing, accédez à votre campagne dynamique et cliquez sur **Planification**.

   ![](assets/one.png)

1. Dans Paramètres de campagne dynamique, cliquez sur **Modifier**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >La limite par défaut est celle définie dans Admin.

1. Saisissez une nouvelle limite, puis cliquez sur **Enregistrez.**

   ![](assets/three.png)

   La campagne dynamique ne s’exécute pas si le nombre de personnes admissibles dépasse la limite définie.

   >[!CAUTION]
   >
   >Soyez prudent avec cette fonctionnalité afin de ne pas inclure trop de personnes par inadvertance.
