---
solution: Marketo Engage
product: marketo
title: TITLE
description: Découvrez comment rationaliser la création d’e-mails avec des thèmes et des modules réutilisables, en garantissant la cohérence et l’efficacité de la conception.
feature: Email Designer
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
exl-id: 349ee021-7341-40e0-8d8c-d041f1a8f343
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 74%

---

# Appliquer des thèmes au contenu de votre e-mail {#apply-email-themes}

>[!AVAILABILITY]
>
>Cette fonctionnalité est actuellement en version Beta et disponible uniquement pour les clientes et clients Beta. Pour rejoindre le programme Beta, contactez votre représentant ou représentante Adobe.

Grâce aux thèmes, les utilisateurs et les utilisatrices non techniques ont la possibilité de créer du contenu réutilisable adapté à une marque et une langue de conception spécifiques en ajoutant un style personnalisé aux modèles standard<!-- to achieve brand specific results-->.

Cette fonctionnalité permet aux spécialistes du marketing d’utiliser plus rapidement et à moindre effort des e-mails visuellement attrayants et conformes à la marque, tout en fournissant des options de personnalisation avancées pour des besoins de conception uniques.

<!--What is the Enhanced Email Authoring Experience?

This feature introduces two key components to simplify and enhance email creation:

* **Theme Management System**: A centralized system for creating, customizing, and applying reusable themes to emails. Themes ensure consistent styling across campaigns and eliminate the need for repetitive manual styling.

* **Modules**: Pre-designed, reusable content blocks that abstract common email elements (e.g., titles, descriptions, images, and links). Modules are built using customizable low-level components, offering flexibility while maintaining design standards.

Key Benefits:

- **Consistency**: Ensure all emails align with your brand's design guidelines.
- **Efficiency**: Save time by reusing themes and modules across campaigns.
- **Customization**: Add custom CSS and mobile-specific styles for advanced designs.
- **Scalability**: Eliminate repetitive styling tasks, enabling faster email creation.-->

## Mécanismes de sécurisation et limitations {#themes-guardrails}

* Lors de la création d’un e-mail en partant de zéro, vous pouvez choisir de commencer à créer votre contenu à l’aide d’un thème afin d’appliquer rapidement un style spécifique adapté à votre marque et à votre conception.

  Si vous choisissez le mode _Style manuel_, vous ne pourrez appliquer aucun thème, sauf si vous réinitialisez l’e-mail.

* Les [fragments](/help/marketo/product-docs/email-marketing/email-designer/fragments.md) ne sont pas compatibles entre les modes _Utiliser des thèmes_ et _Style manuel_.

  Pour pouvoir utiliser un fragment dans un contenu auquel un thème est appliqué, ce fragment doit être créé en mode _Utiliser des thèmes_.

* Si vous utilisez du contenu créé dans HTML, vous serez en [mode de compatibilité](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html) et vous ne pourrez pas appliquer de thèmes à ce contenu.

  Pour tirer pleinement parti de toutes les fonctionnalités du Designer d’e-mail, y compris les thèmes, vous devez créer du contenu en mode _Utiliser des thèmes_ ou convertir le [contenu HTML importé](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html).

<!--If using a content created in Manual Styling mode or HTML, you cannot apply themes to this content. You must create a new content in Use Themes mode.

If you apply a theme to a content using a [fragment](../content-management/fragments.md) created in Manual Styling mode, the rendering may not be optimal.-->

## Créer un thème {#create-and-edit-themes}

Pour définir un thème que vous pouvez utiliser dans les futurs contenus d’e-mail, procédez comme suit.

1. Pour commencer, créez un [modèle d’e-mail](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template).

1. Sélectionnez l’option **[!UICONTROL Créer ou modifier des thèmes]**.

   `![](assets/theme-create.png)`

1. Vous pouvez sélectionner le thème par défaut ou utiliser un modèle Adobe ou personnalisé. Dans cet exemple, sélectionnez le thème par défaut et cliquez sur **[!UICONTROL Créer]**.

   `![](assets/theme-select.png)`

1. Dans l’onglet **[!UICONTROL Paramètres généraux]**, commencez à définir votre thème en lui donnant un nom spécifique pour votre marque. Vous pouvez ajuster la largeur par défaut de vos e-mails et exporter le thème actuel pour le partager dans les sandbox.

   `<!--![](assets/theme-general-settings.png)-->`

1. Utilisez le rail à droite pour parcourir les différents onglets et mettre à jour vos paramètres de conception.

   `![](assets/theme-right-pane.png)`

1. Dans l’onglet **[!UICONTROL Couleurs]** :

   * Utilisez le bouton **[!UICONTROL Modifier]** pour configurer une **[!UICONTROL palette de couleurs]** avec les couleurs par défaut de votre marque. Sélectionnez un **[!UICONTROL préréglage]** pour créer rapidement un jeu de couleurs ou ajuster chaque couleur de votre thème individuellement. Vous pouvez également utiliser une combinaison des deux.

     `![](assets/theme-colors.gif)`

   * Cliquez sur **[!UICONTROL Ajouter une variante]** pour créer plusieurs variantes de couleurs, telles que le mode clair et le mode sombre, où chaque variante a sa propre palette de couleurs et ses propres commandes de nuances.

     `![](assets/theme-colors-variant.png)`

   * Pour chaque variante, cliquez sur l’icône Modifier pour modifier un élément individuel. Vous pouvez utiliser la palette par défaut que vous avez créée ou n’importe quelle couleur personnalisée.

     `![](assets/theme-colors-edit-variant.gif)`

1. Dans les **[!UICONTROL Paramètres de texte]**, vous pouvez définir la police globale que vous souhaitez utiliser pour l’ensemble du thème. Pour un contrôle plus granulaire, vous pouvez également modifier chaque en-tête et type de paragraphe pour ajuster la police, la taille, le style, etc.

   `![](assets/theme-text.png)`

1. Dans l’onglet **[!UICONTROL Espacement]**, sélectionnez un élément dans la liste pour l’espacer correctement entre les différents composants.

   `<!--![](assets/theme-spacing.png)-->`

1. En utilisant les autres onglets sur la droite, vous pouvez gérer séparément chaque élément de bouton, séparateur, mise en forme d’image supplémentaire et espacement de la disposition de la grille pour ce thème.

   `<!--![](assets/theme-buttons.png)-->`

1. Cliquez sur **[!UICONTROL Enregistrer]** pour stocker ce thème en vue d’une utilisation ultérieure.

## Appliquer des thèmes à un e-mail {#apply-themes}

Pour appliquer des thèmes de style par défaut ou personnalisés à un e-mail, procédez comme suit.

1. `In [!DNL Marketo Engage], [add an email](create-email.md) action to a journey or campaign, and [edit your email body](get-started-email-design.md#key-steps).`

1. Vous pouvez sélectionner l’une des actions suivantes :

   * `Select a built-in [email template](use-email-templates.md) to open the Email Designer. A default theme specific to each template is automatically applied.`

   * `Design a [new content from scratch](content-from-scratch.md) and select **[!UICONTROL Use Themes]** to start with a predefined styling theme.`

     `![](assets/theme-from-scratch.png)`

     >[!CAUTION]
     >
     >Si vous choisissez le mode _Style manuel_, vous ne pourrez appliquer aucun thème, sauf si vous réinitialisez l’e-mail.
     >
     >Pour utiliser un [fragment](/help/marketo/product-docs/email-marketing/email-designer/fragments.md) en mode _Utiliser des thèmes_, ce fragment doit avoir été créé lui-même à l’aide du mode _Utiliser des thèmes_.

1. Une fois dans le Concepteur d’e-mail, cliquez sur le bouton **[!UICONTROL Thèmes]** sur le rail de droite. Le thème par défaut ou le thème du modèle s’affiche. Vous pouvez basculer entre les deux variantes de couleur de ce thème.

   `![](assets/theme-default-hero.png)`

1. Cliquez sur la flèche en regard du thème actuellement utilisé. La liste des thèmes personnalisés et Adobe disponibles s’affiche.

   `![](assets/theme-hero-change.png)`

1. Cliquez sur **[!UICONTROL Thèmes personnalisés]** et sélectionnez le thème que vous avez créé.

   `![](assets/theme-select-custom.png)`

1. Cliquez en dehors de la liste déroulante. Le thème personnalisé nouvellement sélectionné applique automatiquement ses styles à tous les composants d’e-mail. Vous pouvez basculer entre les deux variantes de couleur.

1. Lorsqu’un composant est sélectionné, vous pouvez toujours déverrouiller son style à l’aide de l’icône dédiée.

   `![](assets/theme-unlock-style.png)`

Vous pouvez baculer entre les thèmes à tout moment. Le contenu de l’e-mail reste inchangé, mais les styles sont mis à jour pour refléter le nouveau thème.

<!--
>[!NOTE]
> - Themes apply styles globally. Ensure your theme is finalized before applying it to multiple emails.
> - Switching themes may override custom styles applied to individual components.

>[!CAUTION]
> - When using fragments, the email's theme will override the fragment's styles. A warning will be displayed in the editor if there is a conflict.

## Example Use Cases {#example-use-cases}

### 1. Creating a New Theme
- A marketer creates a theme with their brand's colors, fonts, and button styles.
- The theme is saved and reused across multiple email campaigns.

### 2. Switching Themes
- A marketer applies a holiday-themed design to an existing email by switching to a pre-designed holiday theme.-->
