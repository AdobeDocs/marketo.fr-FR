---
unique-page-id: 1147066
description: Remplacer les restrictions de personne dans une Campaign intelligente - Marketo Docs - Documentation du produit
title: Remplacer les restrictions de personne dans une Campaign dynamique
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Remplacer les restrictions de personne dans une Campaign dynamique {#override-person-restrictions-in-a-smart-campaign}

Marketo vous permet de définir le nombre maximal de personnes pouvant bénéficier d’une campagne intelligente ; cela vous permet d’éviter d’envoyer par courrier électronique l’intégralité de votre base de données. Si vous souhaitez _remplacer_ cette limite, voici comment procéder.

>[!PREREQUISITES]
>
>Veillez à [activer les restrictions de personne pour les campagnes dynamiques](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) dans Marketo Admin.

1. Dans Activités marketing, accédez à votre campagne intelligente et cliquez sur **Planification**.

   ![](assets/one.png)

1. Dans Paramètres Smart Campaign, cliquez sur **Modifier**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >La limite par défaut est celle définie dans Admin.

1. Entrez une nouvelle limite, puis cliquez sur **Enregistrer.**

   ![](assets/three.png)

   La campagne intelligente ne s’exécute pas si le nombre de personnes admissibles dépasse la limite définie.

   >[!CAUTION]
   >
   >Soyez prudent avec cette fonction afin de ne pas inclure accidentellement trop de personnes.
