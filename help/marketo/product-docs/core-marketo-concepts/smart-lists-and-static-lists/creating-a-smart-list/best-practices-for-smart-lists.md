---
unique-page-id: 7512524
description: Bonnes pratiques relatives aux listes dynamiques - Documents Marketo - Documentation du produit
title: Bonnes pratiques relatives aux listes intelligentes
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 1%

---

# Bonnes pratiques relatives aux listes intelligentes {#best-practices-for-smart-lists}

Les listes dynamiques sont l’outil de requête le plus puissant de l’univers marketing. Ils trouvent les personnes que vous recherchez avec une rapidité et une facilité magiques.

Pour faciliter leur utilisation et optimiser les performances, nous avons créé une liste des bonnes pratiques. Bon appétit !

>[!NOTE]
>
>**Chaque utilisateur de Marketo Engage est différent.** Plus la base de données est volumineuse, plus le traitement est important. Plus vous avez stocké d’activités, plus leur recherche prend du temps.
>
>Si vous ressentez une lenteur, essayez les conseils ci-dessous. Si le problème persiste, contactez l’assistance technique de [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. **Limiter l’historique -** Les filtres d’historique (ou filtres d’activité) font partie des opérations les plus gourmandes en ressources et en temps. Si vous devez les utiliser, essayez de limiter la période au plus court possible, ce qui réduirait le jeu de données pouvant faire l’objet d’une recherche. En outre, les périodes ne remplacent pas les périodes de conservation. Ex : si l’activité que vous recherchez a une période de conservation de 90 jours et que vous choisissez « 100 derniers jours », seuls les résultats des 90 derniers jours seront renvoyés. Les périodes de conservation des activités [consultez ce lien](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Limiter les listes dynamiques imbriquées -** Lors de la création d’une liste dynamique, limitez la quantité de filtres « Membre de la liste dynamique » utilisés. Cela s’appelle imbriquer des listes dynamiques et chaque liste dynamique référencée augmente le temps de traitement. Au lieu de cela, référencez des listes statiques ou utilisez [segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Utiliser des opérateurs positifs plutôt que négatifs -** Bien que des filtres « non » soient disponibles, ils doivent rechercher l’ensemble du jeu de données dans votre instance, ce qui peut prendre énormément de temps. Les filtres positifs « est » peuvent utiliser des algorithmes de recherche plus efficaces.
1. **Évitez les qualificateurs « contains » -** Si vous ne disposez que de données partielles, les qualificateurs « commence par » produiront des résultats beaucoup plus rapides que les qualificateurs « contient ». « Est » s’exécutera encore plus rapidement. Évitez d’utiliser « contains » avec des valeurs multiples, car l’association des deux peut ralentir encore davantage une campagne.
1. **Utiliser l’échantillon aléatoire en lui-même -** L’échantillon aléatoire est un filtre spécial. Utilisez-la seule pour placer vos employés dans des listes prédéfinies. Ensuite, utilisez simplement « Membre de la liste » pour rendre votre liste dynamique super rapide. Random Sample **NOT** fonctionne avec les listes dynamiques imbriquées. Le filtre Échantillon aléatoire ne fonctionne pas s’il s’agit de la liste dynamique référencée pour le filtre « Membre de la liste dynamique ».
1. **Soyez prudent avec les filtres d&#39;inactivité -** Les filtres comme « Formulaire non rempli » peuvent être très utiles, mais nécessitent beaucoup plus de puissance de traitement.
1. **Soyez économe en collant plusieurs valeurs -** la sélection multiple est conçue pour coller des dizaines, voire des centaines de valeurs. Toutefois, si on en ajoute trop, cela ralentira les choses.
1. **Soyez prudent lors de l’ajout de contraintes -** il s’agit des petits détails d’une règle et des valeurs associées. Plus vous ajoutez de contraintes, plus le temps de traitement est lent.
1. **Simplifiez vos campagnes -** plus de 100 règles indépendantes (nous l’avons vu !) vont évidemment prendre un certain temps à traiter. Restez simple et vous remarquerez les gains de vitesse - en plus, il sera plus facile pour vous de comprendre.
1. **Incluez le symbole @ avant le nom de domaine lors de l’utilisation du filtre Adresse e-mail** **-** Cela permet d’utiliser une requête plus rapide. Exemple : au lieu d’utiliser _email contient &#39;somedomain.com&#39;_, utilisez _email contient &#39;@somedomain.com_.&#39; Si vous utilisez plusieurs adresses e-mail contenant « contient », toutes doivent commencer par « @ ».

>[!TIP]
>
>Marketo Engage peut être utilisé de différentes manières et certaines techniques sont plus adaptées pour vous et votre entreprise. Contactez votre représentant commercial Adobe Professional Services si vous souhaitez obtenir de l’aide pour tirer le meilleur parti de votre investissement.
