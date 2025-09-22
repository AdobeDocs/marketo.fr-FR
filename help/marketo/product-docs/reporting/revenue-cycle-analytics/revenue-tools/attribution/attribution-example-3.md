---
unique-page-id: 7514149
description: Exemple D’Attribution 3 - Documents Marketo - Documentation Du Produit
title: Exemple d’attribution 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 6%

---

# Exemple d’attribution 3 {#attribution-example}

Lisez le scénario suivant et essayez de déterminer les nombres qui doivent se trouver dans la grille.

* 11 avril | Téléchargements Steve (Contenu) - succès
* 22 avril | L’opportunité est créée pour 3 000 $ (Steve et Jason ont tous deux des rôles).
* 25 avril | Jason assiste (Webinaire) - Succès
* 30 avril | L’opportunité est close-confirmée

| Mesure d’attribution | (Contenu) | (Webinaire) |
|---|---|---|
| (MT) Opt créé | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Pipeline créé | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Chiffre d’affaires confirmé | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Afficher les réponses**

>[!NOTE]
>
>**Explication**
>
>Mémoriser les #3 de règles d’attribution. Jason a eu un succès de programme APRÈS la création de la copie. Par conséquent, le webinaire ne peut pas être crédité pour la création de l’opportunité . Seul le crédit pour l’option a été gagné.
>
>Par conséquent, (Contenu) a 100 % de crédit pour la création et le pipeline de l’option, mais seulement 50 % de crédit pour l’option gagnée.

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
>* [Exemple d’attribution 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
