---
unique-page-id: 8159286
description: Filtres d’opportunité et Triggers - Documents Marketo - Documentation du produit
title: Filtres d’opportunité et Triggers
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
feature: Smart Lists
source-git-commit: 8a5903fa5313e34f448f833f20ab8e3624cf23e6
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 5%

---

# Filtres d’opportunité et Triggers {#opportunity-filters-and-triggers}

Les filtres et déclencheurs d’opportunité vous permettent de suivre les événements d’opportunité de Salesforce. Ils sont légèrement différents des autres filtres et déclencheurs.

## Filtres d’opportunités {#opportunity-filters}

Les filtres d’opportunités vous permettent d’analyser les prospects Salesforce qui disposent d’opportunités. Vous pouvez les trouver dans le dossier Opportunités de la palette lors de la modification d’une liste dynamique. Elles sont en quelques sortes.

* Nombre d&#39;opportunités
* Montant total de l&#39;opportunité
* Total du chiffre d&#39;affaires souhaité de l&#39;opportunité
* A une opportunité
* Ajout de l’opportunité
* Suppression de l’opportunité
* Opportunité mise à jour

Si vous recherchez vos champs d’opportunité (personnalisés ou standard), utilisez la variable **A une opportunité** filtrer ou **L&#39;occasion était`[Added/Removed/Updated]`** filtres ou déclencheurs.

**Nombre d’Oppositions, Montant total d’opposition, Chiffre d’affaires total d’opposition attendu**

Grâce à ces filtres, vous pouvez rechercher des pistes en fonction du nombre total, du montant ou des recettes attendues de toutes leurs opportunités.

![](assets/image2015-6-11-12-3a29-3a34.png)

**L’opportunité a été ajoutée à l’opportunité, a été supprimée de l’opportunité**

Si vous recherchez des prospects qui disposent d’opportunités en fonction d’une combinaison de critères, utilisez la variable **A une opportunité**, **A été ajouté à l’opportunité**, ou **A été supprimé de l’opportunité** filtre. Ils vous disent :

* **A une opportunité**: si cette piste présente actuellement une opportunité correspondante
* **A été ajouté à l’opportunité**: si cette piste a jamais été ajoutée à une opportunité correspondante
* **A été supprimé de l’opportunité**: si cette piste a été supprimée d’une opportunité correspondante

Ajoutez les critères de recherche comme **Contrainte** sur le filtre. Les contraintes incluent vos champs standard et personnalisés d’opportunité :

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Par exemple, supposons que vous souhaitiez trouver des pistes ayant des opportunités ouvertes d’au moins 5 000 $. Faites glisser le **A une opportunité** filtrer et utiliser la variable **Est fermé** et **Quantité** contraintes :

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Lorsque vous utilisez plusieurs filtres d’opportunité, vous pouvez obtenir des réponses incorrectes. Si vous avez créé l’exemple ci-dessus avec deux filtres d’opportunité, vous obtenez une liste de prospects qui disposent d’une opportunité d’au moins 5 000 € et de toute opportunité qui est fermée, même s’il s’agit d’opportunités distinctes.

**Opportunité mise à jour**

La variable **Mise à jour de l’opportunité** filtre recherche les opportunités lorsqu’un champ d’opportunité spécifique a été mis à jour. Sélectionnez le champ à vérifier avec le menu déroulant Attribut de déclenchement, puis utilisez les contraintes pour réduire l’ensemble de modifications.

Par exemple, ce filtre vous montrera tous les prospects dont la date de clôture a été modifiée au cours des 30 derniers jours :

![](assets/image2015-6-11-12-3a33-3a7.png)

## Déclencheurs d’opportunité {#opportunity-triggers}

Les déclencheurs d’opportunité suivants sont disponibles. Ils fonctionnent comme les filtres correspondants (décrits précédemment), sauf qu’ils peuvent déclencher des campagnes directement lorsque l’événement se produit :

* Mise à jour de l&#39;opportunité
* Ajouté à l&#39;opportunité
* Supprimé de l&#39;opportunité

Vous pouvez, par exemple, utiliser cette liste dynamique pour déclencher lorsqu’une piste est ajoutée à une opportunité. Dans le flux, vous pouvez les ajouter à la liste Marketing suspendu ou leur envoyer un email ciblé.

![](assets/image2015-6-11-12-3a33-3a48.png)

Pour déclencher vos champs personnalisés d’opportunité, utilisez la variable **Opportunité mise à jour** déclenchez et sélectionnez le champ dans la liste déroulante :

![](assets/image2015-6-11-12-3a33-3a34.png)
