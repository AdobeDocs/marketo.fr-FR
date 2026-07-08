---
solution: Marketo Engage
product: marketo
title: Conformité aux directives de la CNIL - Suivi des ouvertures d’e-mails conditionnels
description: Découvrez comment configurer Marketo Engage pour la conformité CNIL à l’aide d’un champ booléen personnalisé pour acheminer le suivi des ouvertures d’e-mails en fonction du statut de consentement de chaque personne.
level: Beginner, Intermediate
feature: Email Designer
hide: true
source-git-commit: c0c8e88ae6357c4bf75437e1bbc7fe0d6bce1012
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Conformité des conseils de la CNIL : tracking conditionnel des ouvertures d&#39;emails {#cnil}

Découvrez comment configurer Marketo Engage pour honorer le consentement de l’utilisateur final pour le suivi de l’ouverture de l’e-mail (pixels), conformément aux directives de la CNIL (LIEN DE LA COMMUNAUTÉ). L’approche utilise un champ booléen personnalisé pour déterminer la variante d’e-mail qu’une personne reçoit, une dont le suivi des ouvertures est activé ou une dont le suivi est désactivé.

## Étape 1 : créer un champ booléen personnalisé {#custom-field}

1. Dans la zone **Admin**, cliquez sur **Gestion des champs** et sélectionnez **Nouveau champ personnalisé**.

   ![](assets/cnil-1.png)

1. Pour _Objet_, choisissez **Personne**. Pour _Type_, choisissez **Booléen**. Pour _Nom_, saisissez « Suivi des pixels d’e-mail » (le nom de l’API est automatiquement renseigné). Cliquez sur **Créer**.

   ![](assets/cnil-2.png)

## Étape 2 : remplir le champ de consentement {#populate}

1. Définissez la valeur du champ Suivi des pixels d’e-mail pour chaque personne via l’importation de données (synchronisation des API ou [chargement CSV](https://experienceleague.adobe.com/fr/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people){target="_blank"}).

   ![](assets/cnil-3.png)

1. Assurez-vous que le champ personnalisé est correctement mappé.

   ![](assets/cnil-4.png)

>[!NOTE]
>
>À l’avenir, vous pourrez capturer les données directement lors d’un remplissage de formulaire, ce qui permettra à la personne de s’inscrire ou de se désinscrire du suivi des ouvertures d’e-mails.

## Étape 3 : créer des variantes d’e-mail {#variants}

Créez deux e-mails. Notez que le suivi des ouvertures d’e-mail est activé par défaut pour le Designer d’e-mail et l’ancien éditeur d’e-mail.

* **Email One (suivi des ouvertures activé)** : après la création de l’e-mail, aucune autre action n’est requise. Gardez le suivi des ouvertures activé.

* **E-mail 2 (suivi des ouvertures désactivé)** : clonez l’e-mail 1 et désactivez le suivi des ouvertures.

  ![](assets/cnil-5.png)

Dans le Designer d’e-mail, la case à cocher **Désactiver le suivi des ouvertures** se trouve dans l’onglet _Détails_ du volet _Résumé_ à droite de votre e-mail. Dans l’ancien éditeur d’e-mail, la case à cocher **Désactiver le suivi des ouvertures** se trouve dans le menu _Paramètres d’e-mail_.

**Concepteur d’e-mail**

![](assets/cnil-6.png){width="800" zoomable="yes"}

**Ancien éditeur d’email**

![](assets/cnil-7.png){width="800" zoomable="yes"}

## Étape 4 : configuration de votre campagne intelligente {#smart-campaign}

[Créez une campagne intelligente](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign){target="_blank"} pour déterminer l’e-mail que chaque personne reçoit.

1. Dans l’onglet _Flux_ de votre campagne dynamique, insérez l’étape de flux **Envoyer un e-mail**.

   ![](assets/cnil-8.png){width="800" zoomable="yes"}

1. Dans l’étape de flux, cliquez sur **Ajouter un choix**. Dans Choix 1, définissez **if** sur _Suivi des pixels d’e-mail_, définissez l’opérateur sur _is_ et définissez la valeur sur _false_. Pour **E-mail**, sélectionnez _E-mail 2_.

1. Dans le choix par défaut, définissez **E-mail** sur _E-mail 1_.

   ![](assets/cnil-9.png)

Ainsi, les personnes qui n’ont pas consenti au suivi des ouvertures reçoivent l’e-mail non suivi, tandis que les personnes qui ont consenti reçoivent l’e-mail suivi standard.
