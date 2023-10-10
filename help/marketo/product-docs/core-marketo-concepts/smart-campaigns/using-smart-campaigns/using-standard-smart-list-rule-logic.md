---
unique-page-id: 1147001
description: Utilisation de la logique de règle de liste dynamique standard - Documents Marketo - Documentation du produit
title: Utilisation de la logique de règle de liste dynamique standard
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 3916413a90e52a3423a8d7f78ad1c9eb45c2a219
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Utilisation de la logique de règle de liste dynamique standard {#using-standard-smart-list-rule-logic}

Vous avez peut-être remarqué l’option &quot;Utiliser des filtres&quot; lors de la création de listes dynamiques de campagne. Ce paramètre vous permet de décider si les filtres doivent être évalués avec un opérateur ET ou OU.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>La modification de la logique des règles de liste dynamique s’applique uniquement aux filtres, **not** déclencheurs.

Les déclencheurs sont toujours évalués en tant que OU même si le paramètre ci-dessus est défini sur ALL. Voici un exemple :

![](assets/using-standard-smart-list-rule-logic-2.png)

La liste dynamique ci-dessus en mots :

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

Ainsi, si une personne remplit le formulaire **ou** visite la page, la campagne évalue ensuite cette personne en fonction de **all** ou **any** des filtres suivants, en fonction du paramètre utilisé.

>[!MORELIKETHIS]
>
>[Utilisation de la logique de règle de liste dynamique avancée](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
