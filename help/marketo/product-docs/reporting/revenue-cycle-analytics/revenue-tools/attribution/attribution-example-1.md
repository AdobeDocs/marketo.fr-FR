---
unique-page-id: 7514126
description: Exemple D’Attribution 1 - Documents Marketo - Documentation Du Produit
title: Exemple d’attribution 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 7%

---

# Exemple d’attribution 1 {#attribution-example}

Lisez le scénario suivant et essayez de déterminer les nombres qui doivent se trouver dans la grille.

* 11 avril | Fred est acquis par (Tradeshow)
* 15 avril | Margo assiste (Webinaire) - succès
* 22 avril | Fred est associé (rôle) à l’opportunité
* 22 avril | L’opportunité est créée pour 3 000 $

| Nom du programme | (Salon professionnel) | (Webinaire) |
|---|---|---|
| (FT) Opt Created | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Pipeline créé | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Chiffre d’affaires confirmé | `<pre>0</pre>` | `<pre>0</pre>` |

**Afficher les réponses**

>[!NOTE]
>
>**Explication**
>
>Tout d&#39;abord, il faut comprendre que certains types sont COUNTS et d&#39;autres sont CURRENCY. La valeur « Opty Created » est un nombre, un entier. Pipeline est une devise. Dans Marketo, la devise sera conforme aux paramètres régionaux d’administration.
>
>La raison pour laquelle le salon professionnel a reçu tout le crédit est que Margo n&#39;a pas été associée à un rôle dans l&#39;opportunité. Pas de rôle, pas de crédit.

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
>* [Exemple d’attribution 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Exemple d’attribution 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Exemple d’attribution 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
