---
unique-page-id: 7514151
description: Exemple d’attribution 4 - Documents Marketo - Documentation du produit
title: Exemple d’attribution 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 3%

---

# Exemple d’attribution 4 {#attribution-example}

Lisez le scénario suivant et essayez de déterminer les nombres qui doivent se trouver dans la grille.

* 11 avril | Michelle télécharge eBook (Content) - Succès
* 15 avril | John assiste (webinaire) - Réussite
* 22 avril | (Opportunité 1) créée pour 3 000 $
* 24 avril | (Opportunité 2) créée pour 5 000 $
* 25 avril | John et Michelle sont associés à **deux** Optys
* 29 avril | [Opty 1] is Closed-Won

| Nom du programme | (Contenu) | (Webinaire) |
|---|---|---|
|   | (Opty 1) | (Opty 2) | (Opty 1) | (Opty 2) |
| (MT) Option créée | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Pipeline créé | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Chiffre d’affaires confirmé | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Afficher les réponses**

>[!NOTE]
>
>**Explication**
>
>Lorsque vous avez plusieurs opportunités et plusieurs personnes avec succès de programme, vous devez répartir le crédit entre les personnes et les programmes. Toutefois, notez que le crédit pour l’opportunité 1 et 2 n’est pas combiné. Chacun d&#39;eux constitue une évaluation du crédit distincte.
>
>Lorsque de nombreuses personnes sont impliquées, Marketo calcule automatiquement les fractions d’une opportunité pour laquelle donner du crédit.

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
>* [Exemple d’attribution 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Exemple d’attribution 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Exemple d’attribution 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
