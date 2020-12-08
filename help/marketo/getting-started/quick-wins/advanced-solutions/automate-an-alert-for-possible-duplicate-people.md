---
unique-page-id: 7513680
description: Automatisation d'une alerte pour les personnes susceptibles d'être Duplicata - Documentation marketing - Documentation du produit
title: Automatisation d'une alerte pour les Duplicata possibles
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# Automatisation d&#39;une alerte pour les Duplicata possibles {#automate-an-alert-for-possible-duplicate-people}

Vous souhaitez qu&#39;une alerte soit créée chaque fois que possible, une personne duplicata ? Voici comment configurer une Campaign Intelligente pour le faire.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

1. [Créez une campagne](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)intelligente. Définissez la liste intelligente suivante :

   * Déclencheur : **Personne créée**
   * Filtre : **Champs du Duplicata. **Nom du champ **est** **plein nom**.

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Soyez créatifs ! Testez différents champs pour obtenir de meilleurs résultats de filtrage.

1. Dans l’étape de flux, choisissez [Envoyer l’alerte](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) comme action de flux.

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Utilisation du jeton [](../../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) Envoyer les informations d’alertepour inclure un lien vers la personne dans votre gestion de la relation client.

   >[!CAUTION]
   >
   >Si vous importez une liste volumineuse, vous pouvez obtenir un tas de ces alertes en même temps !
   >
   >
   >De plus, deux personnes portant le même nom ne signifie pas automatiquement qu&#39;elles sont la même personne.

1. Activez la campagne dans l’onglet **Planification** .

   ![](assets/image2017-3-27-8-3a24-3a37.png)

C&#39;est tout ! Cette campagne intelligente se déclenche chaque fois qu’une nouvelle personne portant un nom complet existant est créée dans Marketing Cloud.

>[!MORELIKETHIS]
>
>* [Rechercher et fusionner des personnes de Duplicata](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)

