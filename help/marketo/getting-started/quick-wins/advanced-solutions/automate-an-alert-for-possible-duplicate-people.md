---
unique-page-id: 7513680
description: Automatiser une alerte pour les personnes potentiellement en double - Documents Marketo - Documentation du produit
title: Automatiser une alerte de personnes potentiellement en double
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 9%

---

# Automatiser une alerte de personnes potentiellement en double {#automate-an-alert-for-possible-duplicate-people}

Vous souhaitez recevoir une alerte chaque fois qu’un doublon est créé ? Voici comment configurer une campagne intelligente pour y parvenir.

1. [Créer une campagne intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}. Définissez la liste dynamique suivante :

* Déclencheur : **[!UICONTROL Personne créée]**
* Filtre : **[!UICONTROL champs en double]**. Nom du champ **[!UICONTROL is] [!UICONTROL Nom complet]**

  ![](assets/automate-an-alert-1.png)

  >[!TIP]
  >
  >Faites preuve de créativité. Testez différents champs pour obtenir de meilleurs résultats de filtrage.

1. À l’étape de flux, choisissez l’action de flux [[!UICONTROL Envoyer l’alerte]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md){target="_blank"}.

   ![](assets/automate-an-alert-2.png)

   >[!TIP]
   >
   >Utilisation du [jeton Envoyer les informations d’alerte](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"} pour inclure un lien vers la personne dans votre CRM.

   >[!CAUTION]
   >
   >Si vous importez une liste volumineuse, vous risquez de recevoir un grand nombre de ces alertes en même temps.
   >
   >De plus, deux personnes portant le même nom ne signifient pas automatiquement qu’elles sont la même personne.

1. Activez la campagne dans l&#39;onglet **[!UICONTROL Planning]**.

   ![](assets/automate-an-alert-3.png)

Vous avez terminé. Cette campagne dynamique se déclenche chaque fois qu’une nouvelle personne portant un nom complet existant est créée dans Marketo.

>[!MORELIKETHIS]
>
>[Rechercher et fusionner des personnes en double](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}
