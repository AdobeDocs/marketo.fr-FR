---
unique-page-id: 2953188
description: Découvrez les filtres déduits dans les listes dynamiques. Découvrez comment Marketo déduit des filtres à partir des ressources liées.
title: Filtres automatiques
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
TQID: https://experienceleague.adobe.com/-dKeAfCxfD1ErbfBzLqARUMwFY-I9RdkWGC0b-ZtNyE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 218
ht-degree: 1%

---

# Filtres automatiques {#inferred-filters}

Lorsqu&#39;une personne visite votre site web, [&#128279;](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} crée un cookie et le place dans le système. Le système recherche leur adresse IP dans une base de données spéciale et déduit toutes sortes d&#39;informations.

>[!NOTE]
>
>Pour que les valeurs de champ déduites restent à jour, la base de données utilisée pour les recherches d’adresses IP est régulièrement mise à jour. Les mises à jour de la base de données peuvent introduire de nouvelles valeurs de champ déduites que vous devrez peut-être ajouter aux définitions de filtre de liste dynamique.
>
>Des mises à jour de base de données peuvent se produire au cours d&#39;une version de produit [&#128279;](/help/marketo/release-notes/release-schedule.md){target="_blank"}. Lorsqu&#39;une mise à jour se produit, les notes de mise à jour de [&#128279;](/help/marketo/release-notes/current.md){target="_blank"} contiennent une explication de toute modification apportée aux valeurs de champ déduites.

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
