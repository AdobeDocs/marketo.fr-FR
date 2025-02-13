---
solution: Marketo Engage
product: marketo
title: Fragments paramétrés
description: Découvrez comment personnaliser des fragments en rendant certains de leurs champs modifiables.
feature: Email Editor
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
source-git-commit: ec442823dde75f071220208a7e8edd24355d063f
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 62%

---

# Fragments paramétrés {#parameterized-fragments}

Lorsque des fragments sont utilisés dans un e-mail ou un modèle d’e-mail, ils sont verrouillés par défaut en raison de l’héritage. Cela signifie que toutes les modifications apportées à un fragment sont automatiquement propagées à toutes les ressources où le fragment est utilisé. Grâce aux fragments personnalisables, les champs spécifiques d’un fragment peuvent être définis comme modifiables lorsque le fragment est ajouté à un e-mail ou à un modèle d’e-mail. Supposons, par exemple, que vous ayez un fragment avec une bannière, du texte et un bouton. Vous pouvez désigner comme modifiables certains champs, tels que l’image ou l’URL cible du bouton. Cela permet aux utilisateurs et utilisatrices de modifier ces éléments lorsqu’ils incorporent le fragment dans leur modèle d’e-mail ou d’e-mail, offrant ainsi une expérience personnalisée sans affecter le fragment d’origine.

En utilisant des fragments paramétrés, vous pouvez gérer et personnaliser efficacement votre contenu sans créer de blocs de contenu entièrement nouveaux ou interrompre l’héritage du fragment d’origine. Cela permet de s’assurer que les modifications apportées au niveau du fragment sont toujours propagées, tout en permettant la personnalisation nécessaire au niveau du modèle d’e-mail/e-mail.

Les fragments visuels et d’expression peuvent être marqués comme personnalisables. Pour obtenir des instructions détaillées sur la manière de procéder pour chaque type de fragment, reportez-vous aux sections ci-dessous.

## Ajouter des champs modifiables dans des fragments visuels {#visual}

Pour rendre des parties d’un fragment visuel modifiables, procédez comme suit :

>[!NOTE]
>
>Des champs modifiables peuvent être ajoutés aux composants **image**, **texte** et **bouton**. Pour les composants **HTML**, les champs modifiables sont ajoutés à l’aide de l’éditeur de personnalisation, comme pour les fragments d’expression. [Découvrir comment ajouter un champ modifiable dans les composants HTML et les fragments d’expression](#expression)

1. Ouvrez l’écran d’édition du contenu du fragment.

1. Sélectionnez le composant de votre fragment dans lequel vous souhaitez configurer des champs modifiables.

1. Le volet des propriétés du composant s’ouvre sur le côté droit. Sélectionnez l’onglet **[!UICONTROL Champs modifiables]**, puis activez l’option **[!UICONTROL Activer l’édition]**.

1. Tous les champs pouvant être modifiés pour le composant sélectionné sont répertoriés dans le volet. Les champs disponibles pour la modification dépendent du type de composant sélectionné.

   Dans l’exemple ci-dessous, nous autorisons la modification de l’URL du bouton « Cliquez ici ».

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Cliquez sur **[!UICONTROL Aperçu]** pour vérifier tous les champs modifiables et leurs valeurs par défaut.

   Dans cet exemple, le champ URL du bouton s’affiche avec la valeur par défaut définie dans le composant. Cette valeur sera personnalisable par les utilisateurs et utilisatrices après l’ajout du fragment à leur contenu.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Enregistrez vos modifications lorsque vous avez terminé.

Après avoir ajouté le fragment dans un e-mail, les utilisateurs et utilisatrices pourront personnaliser tous les champs modifiables configurés dans le fragment.

## Ajouter des champs modifiables dans les composants HTML et les fragments d’expression {#expression}

Pour rendre modifiables des parties d’un composant HTML ou d’un fragment d’expression, vous devez utiliser une syntaxe spécifique dans l’éditeur d’expression. Cela implique de déclarer une _variable_ avec une valeur par défaut que les utilisateurs et utilisatrices peuvent remplacer après l’ajout du fragment à leur contenu.

Supposons, par exemple, que vous souhaitiez créer un fragment à ajouter à vos e-mails et permettre aux utilisateurs et utilisatrices de personnaliser une couleur spécifique utilisée à différents emplacements, tels que les cadres ou les couleurs d’arrière-plan des boutons. Lors de la création de votre fragment, vous devez déclarer une variable avec un _ID unique_ (par exemple, « couleur ») et l’appeler aux emplacements souhaités dans le contenu du fragment auquel vous souhaitez appliquer cette couleur. Lors de l’ajout du fragment à leur contenu, les utilisateurs et utilisatrices peuvent personnaliser la couleur utilisée partout où la variable est référencée.

Pour les composants HTML, seuls des éléments spécifiques peuvent devenir des champs modifiables. Pour plus d’informations, développez la section ci-dessous.

+++Éléments modifiables dans les composants HTML :

Les éléments ci-dessous peuvent devenir des champs modifiables dans un composant HTML :

* Partie de texte
* URL complète pour un lien ou une image (ne fonctionne pas avec une partie d’une URL)
* Propriété CSS entière (ne fonctionne pas avec la propriété partielle)

Par exemple, dans le code ci-dessous, chaque élément surligné en rouge peut devenir une propriété :

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++

>[!MORELIKETHIS]
>
>[Fragments](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
