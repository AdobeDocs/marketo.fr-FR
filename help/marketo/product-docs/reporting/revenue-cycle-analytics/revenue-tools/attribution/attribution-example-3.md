---
unique-page-id: 7514149
description: Exemple d’attribution 3 - Documents Marketo - Documentation du produit
title: Exemple d’attribution 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 3%

---

# Exemple d’attribution 3 {#attribution-example}

Lisez le scénario suivant et essayez de déterminer les nombres qui doivent se trouver dans la grille.

* 11 avril | Téléchargements Steve (Content) - succès
* 22 avril | L’opportunité est créée pour 3 000 $ (Steve et Jason ont tous deux des rôles).
* 25 avril | Jason participe (webinaire) - succès
* 30 avril | L&#39;opportunité se ferme

| Mesure d’attribution | (Contenu) | (Webinaire) |
|---|---|---|
| (MT) Option créée | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Pipeline créé | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Chiffre d’affaires confirmé | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Afficher les réponses**

>[!NOTE]
>
>**Explication**
>
>Souvenez-vous de la règle d’attribution #3. Jason a réussi le programme APRÈS la création de l’opération. Par conséquent, le webinaire ne peut pas recevoir de crédit pour la création de l&#39;opportunité. Seul le crédit pour l&#39;Opty a gagné.
>
>Par conséquent, (contenu) dispose de 100 % du crédit pour la création et le pipeline de l’Opty, mais seulement 50 % du crédit pour l’Opty a été gagné.

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
>* [Exemple d’attribution 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
