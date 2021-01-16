---
unique-page-id: 1147001
description: Utilisation de la logique de règle de Liste intelligente standard - Documentation sur le marketing - Documentation du produit
title: Utilisation de la logique de règle de Liste intelligente standard
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---


# Utilisation de la logique de règle de Liste intelligente standard {#using-standard-smart-list-rule-logic}

Vous avez peut-être remarqué l’option &quot;Utiliser les filtres&quot; lors de la création de listes dynamiques de campagne. Ce paramètre vous permet de décider si les filtres doivent être évalués avec un opérateur ET ou OU.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>La modification de la logique de règle de liste intelligente s’applique uniquement aux filtres, **et non** déclencheurs.

Les déclencheurs sont toujours évalués comme OU, même si le paramètre ci-dessus est défini sur ALL.  Voici un exemple :

![](assets/image2014-9-22-14-3a12-3a57.png)

La liste intelligente ci-dessus, en termes :

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

Ainsi, si une personne remplit le formulaire **ou** visite la page, la campagne évalue cette personne en fonction de **all** ou **any** des filtres suivants, selon le paramètre utilisé.

>[!MORELIKETHIS]
>
>[Utilisation de la logique avancée des règles de Liste intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
