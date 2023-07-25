---
unique-page-id: 1147001
description: Utilisation de la logique de règle de liste dynamique standard - Documents Marketo - Documentation du produit
title: Utilisation de la logique de règle de liste dynamique standard
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Utilisation de la logique de règle de liste dynamique standard {#using-standard-smart-list-rule-logic}

Vous avez peut-être remarqué l’option &quot;Utiliser des filtres&quot; lors de la création de listes dynamiques de campagne. Ce paramètre vous permet de décider si les filtres doivent être évalués avec un opérateur ET ou OU.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>La modification de la logique des règles de liste dynamique s’applique uniquement aux filtres, **not** déclencheurs.

Les déclencheurs sont toujours évalués en tant que OU même si le paramètre ci-dessus est défini sur ALL.  Voici un exemple :

![](assets/image2014-9-22-14-3a12-3a57.png)

La liste dynamique ci-dessus en termes :

```box
IF person fills out My Form
OR
IF person visits My Page 
AND 
Industry is Marketing 
AND 
Country is USA 
THEN follow the campaign's flow step(s)
```

Ainsi, si une personne remplit le formulaire **ou** visite la page, la campagne évalue ensuite cette personne en fonction de **all** ou **any** des filtres suivants, selon le paramètre utilisé.

>[!MORELIKETHIS]
>
>[Utilisation de la logique de règle de liste dynamique avancée](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
