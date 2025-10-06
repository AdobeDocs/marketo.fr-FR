---
solution: Marketo Engage
product: marketo
title: Fragments personnalisables
description: Découvrez comment personnaliser des fragments en rendant certains de leurs champs modifiables.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
source-git-commit: cc6c04ca8a72f6efb0bec93cba084fe2993f53f0
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 64%

---

# Fragments personnalisables {#customizable-fragments}

Lorsque des fragments sont utilisés dans un e-mail ou un modèle d’e-mail, ils sont verrouillés par défaut en raison de l’héritage. Cela signifie que toutes les modifications apportées à un fragment sont automatiquement propagées à toutes les ressources où le fragment est utilisé. Grâce aux fragments personnalisables, les champs spécifiques d’un fragment peuvent être définis comme modifiables lorsque le fragment est ajouté à un e-mail ou à un modèle d’e-mail. Supposons, par exemple, que vous ayez un fragment avec une bannière, du texte et un bouton. Vous pouvez désigner comme modifiables certains champs, tels que l’image ou l’URL cible du bouton. Cela permet aux utilisateurs et utilisatrices de modifier ces éléments lorsqu’ils incorporent le fragment dans leur modèle d’e-mail ou d’e-mail, offrant ainsi une expérience personnalisée sans affecter le fragment d’origine.

En exploitant des fragments personnalisables, vous pouvez gérer et personnaliser efficacement votre contenu sans créer de blocs de contenu entièrement nouveaux ni interrompre l’héritage du fragment d’origine. Cela permet de s’assurer que les modifications apportées au niveau du fragment sont toujours propagées, tout en permettant la personnalisation nécessaire au niveau du modèle d’e-mail/e-mail.

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
<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->
>[!MORELIKETHIS]
>
>[Fragments](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
