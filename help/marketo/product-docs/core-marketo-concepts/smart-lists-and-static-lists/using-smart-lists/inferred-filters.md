---
unique-page-id: 2953188
description: Filtres déduits - Documents Marketo - Documentation du produit
title: Filtres automatiques
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 1%

---

# Filtres automatiques {#inferred-filters}

Lorsqu&#39;une personne visite votre site web, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} crée un cookie et le place dans le système. Nous recherchons leur IP dans une base de données spéciale et déduisons toutes sortes d&#39;informations.

>[!NOTE]
>
>Pour que les valeurs de champ déduites restent à jour, nous mettons régulièrement à jour la base de données utilisée pour les recherches d’adresses IP. Les mises à jour de la base de données peuvent introduire de nouvelles valeurs de champ déduites que vous devrez peut-être ajouter aux définitions de filtre de liste dynamique.
>
>Des mises à jour de base de données peuvent se produire au cours d&#39;une version de produit [Marketo Engage](/help/marketo/release-notes/release-schedule.md){target="_blank"}. Lorsqu&#39;une mise à jour se produit, les notes de mise à jour de [Marketo Engage](/help/marketo/release-notes/current.md){target="_blank"} contiennent une explication de toute modification apportée aux valeurs de champ déduites.

![](assets/inferred-filters-1.png)

![](assets/inferred-filters-2.png)

![](assets/inferred-filters-3.png)

![](assets/inferred-filters-4.png)

![](assets/inferred-filters-5.png)

![](assets/inferred-filters-6.png)

Lorsque vous utilisez l’un de ces filtres dans une liste dynamique, les résultats génèrent des personnes avec ces informations déduites.

>[!TIP]
>
>Utilisez ces filtres dans un rapport d’activité web. Utilisez les territoires des commerciaux et abonnez-les à un rapport quotidien personnalisé avec les visiteurs du site Web au cours des dernières 24 heures. Ils vont adorer !
>
>* Page Web visitée - Dernières 24 heures
>* L’État déduit est [sélectionner leur territoire]

Ces visiteurs anonymes sont automatiquement convertis en personnes lorsqu’ils cliquent sur un lien d’e-mail ou remplissent un formulaire. Cependant, ils conservent toutes les informations déduites.

>[!NOTE]
>
>En savoir plus sur les [activités et prospects anonymes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md){target="_blank"}.
