---
unique-page-id: 7514126
description: Exemple d’attribution 1 - Documents Marketo - Documentation du produit
title: Exemple d’attribution 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 4%

---

# Exemple d’attribution 1 {#attribution-example}

Lisez le scénario suivant et essayez de déterminer les nombres qui doivent se trouver dans la grille.

* 11 avril | Fred est acquis par (Tradeshow)
* 15 avril | Margo attend (webinaire) - succès
* 22 avril | Fred est associé (rôle) à l’opportunité.
* 22 avril | L’opportunité est créée pour 3 000 $

| Nom du programme | (Tradeshow) | (Webinaire) |
|---|---|---|
| (FT) Opty Created | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Pipeline créé | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Chiffre d’affaires confirmé | `<pre>0</pre>` | `<pre>0</pre>` |

**Afficher les réponses**

>[!NOTE]
>
>**Explication**
>
>Tout d&#39;abord, il faut comprendre que certains types sont COMPTES et d&#39;autres sont DEVISE. Opty Created est un nombre, un entier. Le pipeline est une devise. Dans Marketo, la devise est conforme aux paramètres régionaux de votre administrateur.
>
>La raison pour laquelle le Commerce a reçu tout le crédit est que Margo n&#39;a pas été associé à un rôle dans l&#39;opportunité. Pas de rôle, pas de crédit.

>[!NOTE]
>
>**Règles d’attribution**
>
>1. Le crédit est réparti uniformément.
>1. Tu ne peux pas donner plus de crédit que tu n&#39;as gagné.
>1. On ne peut pas créditer quelque chose qui s&#39;est passé dans le passé.

Essayez tous les exemples et vous serez en faveur de l’attribution !

>[!MORELIKETHIS]
>
>* [Exemple d’attribution 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Exemple d’attribution 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Exemple d’attribution 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
