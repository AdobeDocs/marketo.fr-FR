---
unique-page-id: 7512524
description: Bonnes pratiques pour les Listes intelligentes - Documentation marketing - Documentation du produit
title: Bonnes pratiques pour les Listes dynamiques
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---


# Bonnes pratiques pour les Listes dynamiques {#best-practices-for-smart-lists}

Les listes intelligentes sont l&#39;outil de requête le plus puissant de l&#39;univers marketing. Ils trouvent les gens que vous recherchez avec une vitesse et une facilité magiques.

Pour les rendre faciles à utiliser et à optimiser les performances, nous avons créé une liste de bonnes pratiques. Bon appétit !

>[!NOTE]
>
>**Chaque client est différent.** Plus la base de données est grande, plus le traitement est important. Plus vous avez enregistré d&#39;activités, plus il faut de temps pour les parcourir.
>
>Si vous rencontrez une lenteur, essayez les conseils ci-dessous. Si le problème persiste, contactez le [Support](http://support.marketo.com) de Marketing.

1. **Historique des limites - **Les filtres d&#39;histoire (c.-à-d. les filtres d&#39;Activité) comptent parmi les opérations les plus gourmandes en ressources et les plus chronophages. Si vous devez les utiliser, tentez de limiter la plage de dates au plus court possible, ce qui réduirait l&#39;ensemble de données pouvant faire l&#39;objet de recherches.
1. **Limiter les listes intelligentes imbriquées - **Lors de la création d’une nouvelle liste intelligente, limitez la quantité de filtres &quot;Membre de la Liste intelligente&quot; utilisés. Il s’agit de l’imbrication de listes dynamiques, et chaque liste intelligente référencée augmente le temps de traitement. Faites plutôt référence à des listes statiques ou utilisez [segmentation](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Utilisez des opérateurs positifs par rapport aux opérateurs négatifs - **Bien que des filtres &quot;non&quot; soient disponibles, ils doivent rechercher l&#39;ensemble des données de votre instance, ce qui peut prendre beaucoup de temps. Les filtres positifs &quot;est&quot; peuvent exploiter des algorithmes de recherche plus efficaces.
1. **Evitez &quot;contient&quot; -** Si vous ne disposez que de données partielles, les qualificatifs &quot;débuts avec&quot; donneront des résultats beaucoup plus rapides que &quot;contient&quot;. &quot;Est&quot; fonctionnera encore plus vite. Evitez d’utiliser &quot;contient&quot; avec plusieurs valeurs ; les deux peuvent ralentir encore davantage une campagne.
1. **Utiliser l&#39;échantillon aléatoire seul - **L&#39;échantillon aléatoire est un filtre spécial. Utilisez-le par lui-même pour mettre vos gens dans des listes préfabriquées. Puis utilisez simplement &quot;Membre de la Liste&quot; pour rendre votre liste intelligente super rapide. L’exemple aléatoire **NOT** fonctionne avec les Listes dynamiques imbriquées. Le filtre Échantillon aléatoire ne fonctionne pas s’il s’agit de la Liste dynamique référencée pour le filtre &quot;Membre de la Liste dynamique&quot;.
1. **Evitez les filtres d&#39;inactivité - **Des Filtres tels que &quot;Formulaire non rempli&quot; peuvent être très utiles, mais nécessitent beaucoup plus de puissance de traitement.
1. **Le collage de plusieurs valeurs peut être intéressant. **Le choix multiple est conçu pour coller des dizaines ou peut-être des centaines de valeurs. Mais en mettre trop, et cela ralentira.
1. **Soyez prudent lors de l&#39;ajout de contraintes - **Ce sont les détails minuscules d&#39;une règle et des valeurs associées. Plus vous ajoutez de contraintes, plus le temps de traitement est lent.
1. **Simplifiez vos campagnes - **100+ règles indépendantes (nous l&#39;avons vu !) de toute évidence, il faudra un certain temps pour les traiter. Restez simple et vous remarquerez les gains de vitesse - en plus il sera plus facile pour vous de comprendre.
1. **Insérez le symbole @ avant le nom de domaine lors de l&#39;utilisation du filtre** **Adresse électronique-** Ce qui permet d&#39;utiliser une requête plus rapide. Exemple : Au lieu d&#39;utiliser *email contient &#39;somedomain.com*&#39;, utilisez *email contient &#39;@some.com*&#39;. Si vous utilisez plusieurs adresses électroniques avec &quot;contient&quot;, elles doivent toutes être débuts avec &quot;@&quot;.

>[!TIP]
>
>Le marketing peut être utilisé de nombreuses manières et certaines techniques sont meilleures pour vous et votre entreprise. Envisagez [les services professionnels du marketing](http://pages2.marketo.com/72-hour-survival-guide.html) pour que votre investissement soit brillant.

