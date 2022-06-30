---
unique-page-id: 7513680
description: Automatisation d’une alerte pour les personnes pouvant être dupliquées - Documents Marketo - Documentation du produit
title: Automatisation d’une alerte pour les personnes pouvant être dupliquées
exl-id: 596c03f4-7a84-4564-bbe1-e7bc0d22a616
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Automatisation d’une alerte pour les personnes pouvant être dupliquées {#automate-an-alert-for-possible-duplicate-people}

Souhaitez-vous qu’une alerte soit affichée chaque fois qu’une personne en double est créée ? Voici comment configurer une campagne dynamique pour ce faire.

1. [Création d’une campagne dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target=&quot;_blank&quot;}. Définissez la liste dynamique suivante :

* Déclencheur : **Personne créée**
* Filtre : **Dupliquer les champs.** Nom du champ **est Nom complet**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Soyez créatifs ! Testez différents champs pour obtenir de meilleurs résultats de filtrage.

1. Dans l’étape de flux, choisissez [Envoyer une alerte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md)Action de flux {target=&quot;_blank&quot;}.

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >En utilisant la variable [Envoyer le jeton Informations d’alerte](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;} pour inclure un lien vers la personne dans votre CRM.

   >[!CAUTION]
   >
   >Si vous importez une liste volumineuse, vous pouvez obtenir un ensemble de ces alertes en même temps !
   >
   >De plus, deux personnes portant le même nom ne signifient pas automatiquement qu&#39;elles sont la même personne.

1. Activez l’opération dans la variable **Planification** .

   ![](assets/image2017-3-27-8-3a24-3a37.png)

C&#39;est tout ! Cette campagne dynamique se déclenche chaque fois qu’une nouvelle personne portant un nom complet existant est créée dans Marketo.

>[!MORELIKETHIS]
>
>[Rechercher et fusionner des personnes en double](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target=&quot;_blank&quot;}
