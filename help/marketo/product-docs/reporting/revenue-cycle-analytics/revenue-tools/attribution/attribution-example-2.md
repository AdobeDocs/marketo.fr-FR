---
unique-page-id: 7514146
description: Exemple d’attribution 2 - Documents Marketo - Documentation du produit
title: Exemple d’attribution 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 4%

---

# Exemple d’attribution 2 {#attribution-example}

Lisez le scénario suivant et essayez de déterminer les nombres qui doivent se trouver dans la grille.

* 11 avril | La facturation est acquise par (commerce)
* 15 avril | Joan est acquis par (webinaire)
* 22 avril | (Opportunité 1) créée pour 6 000 $
* 24 avril | (Opportunité 2) créée pour 10 000 $
* 25 avril | Bill et Joan sont associés à des rôles aux types **BOTH**
* 29 avril | (Opportunité 1) est terminée

| Nom du programme | (Tradeshow) | (Webinaire) |
|---|---|---|
| (FT) Opty Created | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT) Pipeline créé | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Chiffre d’affaires confirmé | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Afficher les réponses**

>[!NOTE]
>
>**Explication**
>
>Comme Bill et Joan étaient tous deux associés à des rôles pour les opportunités **BOTH** , le système (selon les règles) partageait le crédit uniformément entre eux.
>
>Le pipeline créé pour chaque programme (8 000 $) représente la moitié du total (16 000 $) disponible pour donner en tant que crédit.

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
>* [Exemple d’attribution 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Exemple d’attribution 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
