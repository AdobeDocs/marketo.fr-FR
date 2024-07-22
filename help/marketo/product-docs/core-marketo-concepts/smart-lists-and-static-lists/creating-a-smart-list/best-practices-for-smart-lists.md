---
unique-page-id: 7512524
description: Bonnes pratiques pour les listes dynamiques - Documents Marketo - Documentation du produit
title: Bonnes pratiques relatives aux listes intelligentes
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Bonnes pratiques relatives aux listes intelligentes {#best-practices-for-smart-lists}

Les listes dynamiques sont l’outil de requête le plus puissant de l’univers marketing. Ils trouvent les gens que vous cherchez avec une vitesse magique et facilité.

Pour les rendre faciles à utiliser et optimiser les performances, nous avons créé une liste de bonnes pratiques. Bon appétit !

>[!NOTE]
>
>**Chaque utilisateur de Marketo Engage est différent.** Plus la base de données est grande, plus le traitement est important. Plus vous avez d’activités stockées, plus la recherche prend du temps.
>
>Si vous rencontrez une lenteur, essayez les conseils ci-dessous. Si le problème persiste, contactez le [support Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. **Historique des limites -** Les filtres d’historique (également appelés filtres d’activité) comptent parmi les opérations les plus gourmandes en ressources et chronophages. Si vous devez les utiliser, essayez de limiter la plage de dates au plus court possible, ce qui réduirait le jeu de données pouvant faire l’objet de recherches. En outre, les périodes ne remplaceront pas les périodes de rétention. Ex : si l’activité que vous interrogez a une période de conservation de 90 jours et que vous choisissez &quot;100 derniers jours&quot;, seuls les résultats des 90 derniers jours seront renvoyés. Les périodes de rétention des activités [se trouvent ici](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Limiter les listes dynamiques imbriquées -** Lors de la création d’une liste dynamique, limitez la quantité de filtres &quot;Membre de la liste dynamique&quot; utilisés. Cela s’appelle l’imbrication de listes dynamiques, et chaque liste dynamique référencée augmente le temps de traitement. À la place, référencez des listes statiques ou utilisez [segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Utilisez des opérateurs positifs plutôt que négatifs -** Bien que des filtres &quot;non&quot; soient disponibles, ils doivent rechercher l’ensemble des données de votre instance, ce qui peut prendre beaucoup de temps. Les filtres &quot;is&quot; positifs peuvent utiliser des algorithmes de recherche plus efficaces.
1. **Évitez &quot;contains&quot; -** Si vous ne disposez que de données partielles, les qualificateurs &quot;commence par&quot; donneront des résultats beaucoup plus rapides que &quot;contains&quot;. &quot;Is&quot; s’exécute encore plus rapidement. Évitez d’utiliser &quot;contains&quot; avec plusieurs valeurs ; les deux ensembles peuvent ralentir encore plus une campagne.
1. **Utiliser l’exemple aléatoire en lui-même -** L’exemple aléatoire est un filtre spécial. Utilisez-le seul pour mettre vos gens dans des listes préfabriquées. Ensuite, utilisez simplement &quot;Membre de la liste&quot; pour rendre votre liste dynamique très rapide. L’exemple aléatoire **NOT** fonctionne avec les listes dynamiques imbriquées. Le filtre Exemple aléatoire ne fonctionne pas s’il s’agit de la liste dynamique référencée pour le filtre &quot;Membre de la liste dynamique&quot;.
1. **Soyez riche en filtres d’inactivité -** Les filtres tels que &quot;Formulaire non rempli&quot; peuvent être très utiles, mais nécessitent beaucoup plus de puissance de traitement.
1. **Le collage de plusieurs valeurs est une bonne chose.** Le choix multiple est conçu pour coller des dizaines ou peut-être des centaines de valeurs. En y mettre trop, cependant, et cela ralentira.
1. **Soyez prudent lors de l’ajout de contraintes -** Il s’agit des détails minuscules d’une règle et des valeurs associées. Plus vous ajoutez de contraintes, plus le temps de traitement est lent.
1. **Simplifiez vos campagnes -** 100+ règles indépendantes (nous l’avons vu !) sont évidemment sur le point de prendre du temps pour les traiter. Restez simple et vous remarquerez les gains de vitesse - et il vous sera plus facile de comprendre.
1. **Incluez le symbole @ avant le nom de domaine lors de l’utilisation du filtre Adresse électronique** **-** Cela permet d’utiliser une requête plus rapide. Exemple : au lieu d&#39;utiliser _email contient &#39;some domain.com&#39;_, utilisez _email contenant &#39;@somedomain.com_&#39;. Si vous utilisez plusieurs adresses électroniques avec &quot;contient&quot;, toutes doivent commencer par &quot;@&quot;.

>[!TIP]
>
>Le Marketo Engage peut être utilisé de différentes manières et certaines techniques sont meilleures pour vous et votre entreprise. Contactez votre représentant commercial Adobe Professional Services si vous souhaitez obtenir de l’aide pour tirer le meilleur parti de votre investissement.
