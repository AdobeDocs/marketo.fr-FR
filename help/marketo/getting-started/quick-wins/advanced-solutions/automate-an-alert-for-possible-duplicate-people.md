---
unique-page-id: 7513680
description: Automatisation d'une alerte pour les personnes susceptibles d'être Duplicata - Documentation marketing - Documentation du produit
title: Automatisation d'une alerte pour les Duplicata possibles
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# Automatisation d&#39;une alerte pour les personnes Duplicata {#automate-an-alert-for-possible-duplicate-people}

Vous souhaitez qu&#39;une alerte soit créée chaque fois que possible, une personne duplicata ? Voici comment configurer une Campaign Intelligente pour le faire.

1. [Créez une campagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) intelligente. Définissez la liste intelligente suivante :

* Déclencheur : **Personne créée**
* Filtre : **Champs de Duplicata.** Nom du champ  **Nom complet**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Soyez créatifs ! Testez différents champs pour obtenir de meilleurs résultats de filtrage.

1. Dans l’étape de flux, choisissez [Envoyer l’alerte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) action de flux.

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Utilisation du [jeton d’informations d’alerte](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) pour inclure un lien vers la personne dans votre gestion de la relation client.

   >[!CAUTION]
   >
   >Si vous importez une liste volumineuse, vous pouvez obtenir un tas de ces alertes en même temps !
   >
   >De plus, deux personnes portant le même nom ne signifie pas automatiquement qu&#39;elles sont la même personne.

1. Activez la campagne dans l&#39;onglet **Planification**.

   ![](assets/image2017-3-27-8-3a24-3a37.png)

C&#39;est tout ! Cette campagne intelligente se déclenche chaque fois qu’une nouvelle personne portant un nom complet existant est créée dans Marketing Cloud.

>[!MORELIKETHIS]
>
>[Rechercher et fusionner des personnes de Duplicata](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
