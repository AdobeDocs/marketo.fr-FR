---
unique-page-id: 7514151
description: Exemple D’Attribution 4 - Documents Marketo - Documentation Du Produit
title: Exemple d’attribution 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 6%

---

# Exemple d’attribution 4 {#attribution-example}

Lisez le scénario suivant et essayez de déterminer les nombres qui doivent se trouver dans la grille.

* 11 avril | Michelle télécharge e-Book (Content) - Success
* 15 avril | John assiste (webinaire) - Succès
* 22 avril | (Opportunité 1) créée pour 3 000 $
* 24 avril | (Opportunité 2) créée pour 5 000 $
* 25 avril | John et Michelle sont associés à **les deux** Optys
* 29 avril | [Opty 1] est conclu

| Nom du programme | (Contenu) | (Webinaire) |
|---|---|---|
|   | (Opty 1) | (Opty 2) | (Opty 1) | (Opty 2) |
| (MT) Opt créé | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Pipeline créé | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Chiffre d’affaires confirmé | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Afficher les réponses**

>[!NOTE]
>
>**Explication**
>
>Lorsque vous avez plusieurs possibilités et plusieurs personnes qui réussissent le programme, vous devez répartir le crédit entre les personnes et les programmes. Notez toutefois que le crédit pour les opportunités 1 et 2 n’est pas combiné. Chacune d&#39;elles est une évaluation de crédit distincte.
>
>Lorsque de nombreuses personnes sont impliquées, Marketo calcule automatiquement les fractions d’une opportunité de donner du crédit.

>[!NOTE]
>
>**Règles d’attribution**
>
>1. Le crédit est partagé également
>1. On ne peut pas accorder plus de crédit que ce qu&#39;on a gagné
>1. On ne peut pas attribuer le mérite de quelque chose qui s&#39;est produit dans le passé

Essayez tous les exemples et vous serez un pro de l’attribution !

>[!MORELIKETHIS]
>
>* [Exemple d’attribution 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Exemple d’attribution 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Exemple d’attribution 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
