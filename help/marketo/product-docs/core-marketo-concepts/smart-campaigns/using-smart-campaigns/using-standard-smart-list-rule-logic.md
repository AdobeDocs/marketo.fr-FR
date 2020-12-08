---
unique-page-id: 1147001
description: Utilisation de la logique de règle de Liste intelligente standard - Documentation sur le marketing - Documentation du produit
title: Utilisation de la logique de règle de Liste intelligente standard
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---


# Utilisation de la logique de règle de Liste intelligente standard {#using-standard-smart-list-rule-logic}

Vous avez peut-être remarqué l’option &quot;Utiliser les filtres&quot; lors de la création de listes dynamiques de campagne. Ce paramètre vous permet de décider si les filtres doivent être évalués avec un opérateur ET ou OU.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>La modification de la logique des règles de liste intelligente s’applique uniquement aux filtres, **pas** aux déclencheurs.

Les déclencheurs sont toujours évalués comme OU, même si le paramètre ci-dessus est défini sur ALL.  Voici un exemple :

![](assets/image2014-9-22-14-3a12-3a57.png)

La liste intelligente ci-dessus, en termes :
`<pre data-theme="Confluence">IF person fills out My Form OR IF person visits My Page AND Industry is Marketing AND Country is USA THEN follow the campaign's flow step(s)</pre>` Ainsi, si une personne remplit le formulaire **ou visite** la page, la campagne évalue cette personne en fonction de **tous **ou **n*importe quel **des filtres suivants, selon le paramètre utilisé.

>[!NOTE]
>
>**Articles connexes**
>
>* [Utilisation de la logique avancée des règles de Liste intelligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)

>



