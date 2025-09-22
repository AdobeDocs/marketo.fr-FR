---
unique-page-id: 1147001
description: Utilisation De La Logique De Règle De Liste Dynamique Standard - Documents Marketo - Documentation Du Produit
title: Utilisation de la logique standard de règle de liste intelligente
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 9%

---

# Utilisation de la logique standard de règle de liste intelligente {#using-standard-smart-list-rule-logic}

Vous avez peut-être remarqué l’option « Utiliser des filtres » lors de la création de listes dynamiques Campaign. Ce paramètre vous permet de décider si les filtres doivent être évalués avec un opérateur AND ou OR.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>La modification de la logique de règle de liste dynamique s’applique uniquement aux filtres, _pas_ aux déclencheurs.

Les Triggers sont toujours évalués en tant que OU même si le paramètre ci-dessus est défini sur ALL. Voici un exemple :

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
