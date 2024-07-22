---
unique-page-id: 7513680
description: Automatisation d’une alerte pour les personnes pouvant être dupliquées - Documents Marketo - Documentation du produit
title: Automatisation d’une alerte pour les personnes potentiellement en double
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Automatisation d’une alerte pour les personnes potentiellement en double {#automate-an-alert-for-possible-duplicate-people}

Souhaitez-vous qu’une alerte soit affichée chaque fois qu’une personne en double est créée ? Voici comment configurer une campagne dynamique pour ce faire.

1. [Créez une campagne dynamique ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}. Définissez la liste dynamique suivante :

* Déclencheur : **[!UICONTROL La personne est créée]**
* Filtre : **[!UICONTROL Champs En Double]**. Nom du champ **[!UICONTROL is] [!UICONTROL Nom complet]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >Soyez créatifs ! Testez différents champs pour obtenir de meilleurs résultats de filtrage.

1. À l’étape de flux, choisissez l’action de flux [[!UICONTROL Envoyer une alerte]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"}.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Utilisation du [jeton Send Alert Info](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"} pour inclure un lien vers la personne dans votre CRM.

   >[!CAUTION]
   >
   >Si vous importez une liste volumineuse, vous pouvez obtenir un ensemble de ces alertes en même temps !
   >
   >De plus, deux personnes portant le même nom ne signifient pas automatiquement qu&#39;elles sont la même personne.

1. Activez la campagne dans l’onglet **[!UICONTROL Planning]** .

   ![](assets/automate-an-alert-3.png)

C&#39;est tout ! Cette campagne dynamique se déclenche chaque fois qu’une nouvelle personne portant un nom complet existant est créée dans Marketo.

>[!MORELIKETHIS]
>
>[Rechercher et fusionner des personnes en double](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
