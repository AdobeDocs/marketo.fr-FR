---
unique-page-id: 8159286
description: Filtres d'opportunité et déclencheurs - Docs marketing - Documentation du produit
title: Filtres d'opportunité et déclencheurs
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Filtres d&#39;opportunité et déclencheurs {#opportunity-filters-and-triggers}

Les filtres et déclencheurs d&#39;opportunité vous permettent de suivre les événements d&#39;opportunité de Salesforce. Ils sont un peu différents des autres filtres et déclencheurs.

## Filtres d&#39;opportunité {#opportunity-filters}

Les filtres d&#39;opportunité vous permettent d&#39;analyser vos prospects de Salesforce qui ont des opportunités. Vous pouvez les trouver dans le dossier Opportunités de la palette lors de la modification d’une liste dynamique. Ils sont en quelques saveurs.

* Nombre d’options
* Montant total d&#39;opacité
* Total des recettes prévues de l&#39;Optimisation
* A une opportunité
* L&#39;opportunité a été Ajoutée
* L&#39;opportunité a été supprimée
* L&#39;opportunité a été mise à jour

Si vous recherchez vos champs Opportunité (personnalisé ou standard), utilisez le filtre **Avec opportunité** ou **L&#39;opportunité était`[Added/Removed/Updated]`** filtres ou déclencheurs.

**Nombre d’options, Montant total de l’opacité, Recettes totales prévues de l’opacité**

Avec ces filtres, vous pouvez trouver des pistes en fonction du nombre total, du montant ou des recettes attendues de toutes leurs opportunités.

![](assets/image2015-6-11-12-3a29-3a34.png)

**L&#39;opportunité a été Ajoutée à l&#39;opportunité, a été supprimée de l&#39;opportunité**

Si vous recherchez des pistes qui ont des opportunités en fonction d&#39;une combinaison de critères, utilisez le filtre **Avec opportunité**, **A été Ajouté à Opportunité** ou **A été supprimé de Opportunité**. Ils vous disent :

* **A une opportunité** : Si cette piste a actuellement une opportunité correspondante
* **A été Ajouté à Opportunité** : Si cette piste a déjà été ajoutée à une opportunité correspondante
* **A été supprimé de l&#39;opportunité** : Si cette piste a été supprimée d&#39;une opportunité correspondante

Ajoutez les critères de recherche sous la forme **Contraintes** sur le filtre. Les contraintes incluent vos champs standard et personnalisés d’opportunité :

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Supposons, par exemple, que vous souhaitiez trouver des pistes ayant des opportunités ouvertes d’au moins 5 000 $. Faites glisser le filtre **Avec opportunité** et utilisez les contraintes **Est fermé** et **Montant** :

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Lorsque vous utilisez plusieurs filtres d&#39;opportunité, il se peut que vous obteniez des réponses incorrectes. Si vous avez créé l&#39;exemple ci-dessus avec deux filtres d&#39;opportunité, vous obtiendriez une liste de pistes qui ont une opportunité d&#39;au moins 5 000 $ et toute opportunité fermée, même si ce sont des opportunités distinctes.

**L&#39;opportunité a été mise à jour**

Le filtre **Opportunité a été mis à jour** recherche toute opportunité lorsqu&#39;un champ opportunité spécifique a été mis à jour. Sélectionnez le champ à vérifier avec la liste déroulante Attribut de déclenchement, puis utilisez les contraintes pour restreindre l’ensemble de modifications.

Par exemple, ce filtre vous montre tous les prospects dont la date de clôture a été modifiée au cours des 30 derniers jours :

![](assets/image2015-6-11-12-3a33-3a7.png)

## Déclencheurs d&#39;opportunité {#opportunity-triggers}

Les déclencheurs d&#39;opportunité suivants sont disponibles. Ils fonctionnent de la même manière que leurs filtres correspondants (décrits plus haut), sauf qu’ils peuvent déclencher des campagnes correctement lorsque le événement se produit :

* L&#39;opportunité est mise à jour
* Ajouté à l&#39;opportunité
* Supprimé de l&#39;opportunité

Par exemple, vous pouvez utiliser cette Liste dynamique pour déclencher une piste lorsqu&#39;une piste est ajoutée à une opportunité. Dans le flux, vous pouvez les ajouter à la liste Suspendue du marketing ou leur envoyer un courriel ciblé.

![](assets/image2015-6-11-12-3a33-3a48.png)

Pour déclencher vos champs personnalisés d&#39;opportunité, utilisez le déclencheur **Opportunité mise à jour** et sélectionnez le champ dans la liste déroulante :

![](assets/image2015-6-11-12-3a33-3a34.png)

