---
unique-page-id: 1147001
description: Découvrez comment utiliser la logique de règle de liste dynamique standard dans une campagne dynamique. Combinez les filtres avec la logique ET pour la qualification.
title: Utilisation de la logique standard de règle de liste intelligente
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/hRPdzjEUOeC2PZK2YlO1IPZOPoPOfo7CHJu2yUtU0qc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 10%

---

# Utilisation de la logique standard de règle de liste intelligente {#using-standard-smart-list-rule-logic}

Vous avez peut-être remarqué l’option « Utiliser des filtres » lors de la création de listes dynamiques Campaign. Ce paramètre vous permet de décider si les filtres doivent être évalués avec un opérateur AND ou OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>La modification de la logique de règle de liste dynamique s’applique uniquement aux filtres, _pas_ aux déclencheurs.

Les Triggers sont toujours évalués en tant que OU même si le paramètre ci-dessus est défini sur ALL. Par exemple :

![](assets/using-standard-smart-list-rule-logic-2.png)

La liste dynamique ci-dessus avec les mots :

```box
IF person fills out Great Form
OR
IF person visits Keith's Landing Page
AND
Industry is Energy
AND
Country is US
THEN follow the campaign's flow step(s)
```

Ainsi, si une personne remplit le formulaire _ou_ visite la page, la campagne évaluera alors cette personne en fonction de _tous_ ou _l’un_ des filtres suivants, selon le paramètre utilisé.

>[!MORELIKETHIS]
>
>[Utilisation de la logique de règle de liste dynamique avancée](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
