---
unique-page-id: 7514898
description: Configuration d'une Campaign intelligente Trigger pour les ventes à l'aide de "Campaign is Requested" - Docs marketing - Documentation du produit
title: Configuration d'une Campaign dynamique de déclenchement pour les ventes à l'aide de "Campaign is Requested"
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Configuration d&#39;une Campaign intelligente déclencheuse pour les ventes à l&#39;aide de &quot;Campaign is Requested&quot; {#setting-up-a-trigger-smart-campaign-for-sales-using-campaign-is-requested}

L&#39;une des caractéristiques les plus cool de Marketo est la possibilité de permettre aux vendeurs de participer à l&#39;effort marketing. Ils sont en première ligne, interagissant avec les gens. Les vendeurs devraient avoir la capacité d&#39;orienter le marketing dans la bonne direction.

>[!NOTE]
>
>Exemples de campagnes dynamiques à demander :
>
>1. **Entretien**  à long terme - quand ils n&#39;ont pas de budget cette année et que vous voulez simplement rester sur le radar
>1. **Principal cycle**  de vente - lorsque le vendeur ne veut pas de message à la personne sauf le sien. (utilisez l&#39;indicateur de suspension marketing pour les désabonner temporairement)

>
>
Soyez créatifs ! Qu&#39;est-ce que le vendeur aimerait automatiser ? Demandez-leur et branchez-le !

1. Créer une **Campaign intelligente.**

   ![](assets/image2015-5-20-16-3a3-3a25.png)

1. Recherchez **Campaign est demandé** et faites-le glisser sur le canevas.

   ![](assets/campaignfilterdrag.png)

1. Les choix de la source indiquent le type de demande qui sera satisfaite. Pour la fonctionnalité Salesforce, veillez à choisir **Sales** **Insight**.

   >[!TIP]
   >
   >Les opérateurs source sont pour la sécurité. Vous pouvez limiter la campagne aux requêtes effectuées uniquement par des sources spécifiques, comme d’autres campagnes ou développeurs dynamiques. Sélectionnez **Est n’importe lequel** dans la première zone si vous souhaitez autoriser les requêtes provenant de toutes les sources.
   >
   >**N&#39;oubliez** pas qu&#39;en choisissant Sales Insight, il apparaîtra comme par magie dans la boîte pour les ventes. Ne le fais pas trop ! Trop d&#39;entre eux seront ignorés.

   ![](assets/image2015-5-20-17-3a56-3a56.png)

C&#39;est un excellent moyen d&#39;étendre votre portée marketing à d&#39;autres services. Configurez tous les types de campagnes à automatiser.

>[!TIP]
>
>N&#39;oubliez pas de nommer clairement vos campagnes intelligentes. Ils s&#39;affichent dans Sales Insight exactement comme vous les nommez.
