---
description: Mode Sombre - Documents Marketo - Documentation Du Produit
title: Mode Sombre
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: f960d7918d97a2c5e3d16673bc4c5c592004ff1e
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 62%

---

# Mode Sombre {#dark-mode}

Lors de la conception de vos e-mails, le Designer d’e-mail vous permet de passer à la vue **[!UICONTROL Mode sombre]**.

En **[!UICONTROL mode sombre]**, vous pouvez définir des paramètres personnalisés spécifiques à afficher par la prise en charge des clients de messagerie lorsque leur mode sombre est activé.

## Présentation du mode sombre {#what-is-dark-mode}

Le mode sombre permet aux clients de messagerie et aux applications de messagerie de s’afficher avec des arrière-plans plus sombres et des couleurs plus claires pour le texte, les boutons et d’autres éléments de l’interface utilisateur. Cela permet de réduire la fatigue visuelle, d’économiser l’autonomie de la batterie et d’améliorer la lisibilité dans les environnements à faible luminosité pour une expérience de visionnage plus confortable.

## Mécanismes de sécurisation {#guardrails}

Le rendu en mode sombre peut varier considérablement selon les clients de messagerie.

Avant d’utiliser le mode sombre, il est important de comprendre comment les principaux clients de messagerie le gèrent. Il existe trois cas à distinguer :

### Clients ne prenant pas en charge le mode sombre {#not-supporting}

Certains clients de messagerie ne prennent pas du tout en charge cette fonctionnalité, tels que :

* Yahoo!Mail
* AOL

Que vous définissiez ou non des paramètres personnalisés de mode sombre, ces clients de messagerie n’affichent jamais de rendu en mode sombre.

### Clients appliquant leur propre mode sombre {#default-support}

Certains clients de messagerie appliquent systématiquement leur propre mode sombre par défaut pour tous les e-mails reçus. Les couleurs, les arrière-plans, les images, etc., sont automatiquement ajustés avec les paramètres de mode sombre spécifiques à ce client de messagerie. Aucune modification externe n’est possible.

Ces clients, par exemple :

* Gmail (client de messagerie web de bureau, iOS, Android, client de messagerie web mobile)
* Outlook Windows
* Outlook Windows Mail

Dans ce cas, si vous définissez des paramètres de mode sombre personnalisés dans le Designer Email, ces paramètres sont remplacés par les paramètres du client de messagerie.

Ainsi, bien que ces clients de messagerie gèrent le mode sombre, votre conception de mode sombre spécifique ne sera pas rendue.

### Clients prenant en charge le mode sombre personnalisé {#custom-support}

D’autres clients de messagerie offrent la possibilité de rendre le mode sombre personnalisé avec la requête `@media (prefers-color-scheme: dark)`, qui est la méthode utilisée par le Designer de messagerie [!DNL Marketo Engage].

Voici une liste des principaux clients gérant cette option :

* Apple Mail macOS
* Apple Mail iOS
* Outlook macOS
* Outlook.com
* Outlook iOS
* Outlook Android

Dans ce cas, les paramètres que vous définissez dans le Designer Email doivent être affichés.

>[!NOTE]
>
>Découvrez comment définir des paramètres de mode sombre personnalisés avec le Designer Email dans [cette section](#define-custom-dark-mode).

Cependant, certaines restrictions peuvent s’appliquer en fonction de chaque client de messagerie. Par exemple, certains clients tels qu’Apple Mail 16 (macOs 13) ne généreront pas de mode sombre si des images sont présentes.

Pour des résultats optimaux, testez votre contenu dans les clients de messagerie ciblés. Pour voir une simulation qui se rapproche le plus possible du résultat final pour chaque client, utilisez la fonctionnalité [Rendu des emails](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) de la Designer Email.

## Mode sombre dans le Concepteur d’e-mail {#dark-mode-email-designer}

En ce qui concerne le mode sombre dans le Concepteur d’e-mail, deux aspects doivent être pris en compte :

* Vous pouvez prévisualiser la manière dont le mode sombre par défaut s’affichera dans la plupart des clients de messagerie pris en charge. [En savoir plus](#preview-dark-mode)

* Si vous souhaitez remplacer les paramètres par défaut des clients de messagerie de prise en charge, vous pouvez définir des paramètres de mode sombre personnalisés dans l’e-mail que vous modifiez. [En savoir plus](#define-custom-dark-mode)

### Prévisualiser le mode sombre par défaut {#preview-dark-mode}

Pour accéder au mode sombre dans le Concepteur d’e-mail et prévisualiser les paramètres par défaut du mode sombre, procédez comme suit.

1. Dans la page d’accueil du concepteur d’e-mail, cliquez sur le bouton **[!UICONTROL Créer en partant de zéro]**.

1. Ajoutez [structures et contenu](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-structure-and-content) à votre e-mail.

1. En haut à droite, activez le bouton (bascule) **[!UICONTROL Mode sombre]**.

   CAPTURE D’ÉCRAN

1. La prévisualisation du mode sombre par défaut s’affiche.

   CAPTURE D’ÉCRAN

Par défaut, l’aperçu en mode sombre du Concepteur d’e-mail applique le modèle de couleurs « inversion complète des couleurs » à tous les éléments, à l’exception des images et des icônes.

Cela signifie qu’il détecte les zones comportant des éléments clairs et sombres et les inverse, de sorte que les arrière-plans clairs deviennent sombres et que le texte sombre devient clair, tandis que les arrière-plans sombres deviennent clairs et que le texte clair devient sombre.

>[!CAUTION]
>
>Le rendu final peut varier en fonction du client de messagerie de la personne destinataire. Pour visualiser une simulation qui se rapproche le plus possible du résultat final pour chaque client de messagerie, utilisez l’option [Rendu des e-mails](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).

### Définir le mode sombre personnalisé {#define-custom-dark-mode}

Après avoir activé le **[!UICONTROL mode sombre]**, vous pouvez choisir de modifier des éléments de style spécifiques dans votre contenu qui s’afficheront uniquement si le mode sombre est activé dans le client de messagerie de la personne destinataire, à condition que le client prenne en charge cette fonctionnalité.

>[!WARNING]
>
>Le rendu final en mode sombre dépend de chaque client de messagerie. Le résultat peut donc varier d’un client à l’autre. [En savoir plus](#guardrails)

Pour tirer parti du style du mode sombre personnalisé d’Email Designer, Journey Optimizer utilise la requête CSS `@media (prefers-color-scheme: dark)`, qui détecte si le client de messagerie de l’utilisateur est en mode sombre et applique la conception avec thème sombre définie dans votre e-mail.

Pour définir les paramètres du mode sombre personnalisé, procédez comme suit.

1. Veillez à basculer vers l’aperçu en **[!UICONTROL mode sombre]** dans le Concepteur d’e-mail. [Voici comment procéder](#preview-dark-mode)

1. Modifiez les attributs de couleurs du style, tels que le texte, les arrière-plans, les boutons, etc.

1. Vous ne pouvez pas modifier les couleurs des images et des icônes, mais vous pouvez définir des ressources spécifiques au mode sombre. Pour ce faire, sélectionnez une image. Passez en **[!UICONTROL mode sombre]** à l’aide du bouton dédié dans le volet **[!UICONTROL Paramètres]** et sélectionnez une autre ressource.

   CAPTURE D’ÉCRAN

1. Vous pouvez à tout moment **[!UICONTROL Passer en mode en direct]** afin de vérifier comment votre contenu s’affiche sur les différentes tailles d’appareils. Dans cette vue, cliquez sur le bouton Mode sombre en haut de l’écran pour prévisualiser la version en mode sombre de votre contenu sur les différents appareils.

   CAPTURE D’ÉCRAN

   >[!CAUTION]
   >
   >Le mode en direct est une prévisualisation générique conçue pour comparer l’aspect du rendu sur différentes tailles d’appareils. Le rendu final peut varier en fonction du client de messagerie de la personne destinataire.

1. Une fois que vous avez apporté les modifications souhaitées pour le mode sombre, cliquez sur **[!UICONTROL Simuler le contenu]**.

   ![](assets/dark-mode-simulate.png)

1. Sélectionnez **[!UICONTROL Rendu d’e-mail]** et connectez-vous à votre compte Litmus. Vous pouvez voir le rendu final en mode sombre pour divers clients de messagerie. En savoir plus sur le [Rendu des emails](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).

   >[!WARNING]
   >
   >Bien que la simulation se rapproche beaucoup de la façon dont les e-mails s’afficheront en mode sombre, le rendu réel peut être différent en raison de variations au niveau des paramètres des fournisseurs de services de messagerie ou au niveau des paramètres des appareils.

## Bonnes pratiques {#best-practices}

À mesure que l’adoption du mode sombre augmente dans les principaux clients de messagerie, il est essentiel d’examiner le rendu de vos e-mails à la fois dans les environnements clairs et sombres, que vous utilisiez le [mode sombre personnalisé](#define-custom-dark-mode) ou non.

Le mode sombre peut modifier les couleurs, les arrière-plans et les images, parfois en remplaçant les choix définis lors de la conception. Pour garantir la cohérence visuelle, l’accessibilité et l’intégrité de la marque, suivez les bonnes pratiques répertoriées ci-dessous.

**Optimiser vos images et vos logos**

* Enregistrez les logos et les icônes au format PNG avec des arrière-plans transparents pour éviter la présence de zones blanches visibles en mode sombre.

* Évitez les images avec des fonds blancs ou clairs codés en dur.

* Si vous ne pouvez pas utiliser la transparence, placez les images sur un arrière-plan uni dans votre conception pour éviter des inversions de couleurs inappropriées.

**Vérifier vos arrière-plans**

* Vérifiez que le contraste entre le texte et les couleurs d’arrière-plan est suffisant pour garantir une bonne lisibilité en mode clair et en mode sombre.

* Évitez de vous fier uniquement aux couleurs d’arrière-plan pour du contenu important. Certains clients remplacent les couleurs d’arrière-plan en mode sombre ; veillez donc à ce que les informations clés soient toujours visibles.

**Concevoir du contenu accessible en mode sombre**

* Utilisez des combinaisons de couleurs faciles à distinguer pour les personnes atteintes de daltonisme.

* Utilisez une palette de tons moyens pour garantir un contraste adéquat par rapport à des arrière-plans clairs et sombres.

* Utilisez des combinaisons de couleurs accessibles à fort contraste pour améliorer la lisibilité et respecter les normes WCAG. Utilisez des outils tels que le vérificateur de contraste de WebAIM pour vérifier le contraste des couleurs.

* Évitez les polices de caractères fines, car elles peuvent affecter la lisibilité. Si votre marque nécessite l’utilisation d’une police fine, mettez-la en gras en mode sombre.

* N’utilisez pas de blanc pur sur du noir pur, car cela peut entraîner une fatigue oculaire et peut être automatiquement inversé par certains clients de messagerie.

* Fournissez un style de secours accessible si le mode sombre n’est pas pris en charge.

**Tester vos e-mails dans un environnement en mode sombre**

* Utilisez la [prévisualisation du mode sombre](#preview-dark-mode) du Concepteur d’e-mail, qui utilise des modèles de couleurs inversées, pour repérer les problèmes en amont.

* Utilisez l’option [Rendu d’e-mail](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) qui tire parti de Litmus pour simuler vos conceptions sur les principaux clients de messagerie (Apple Mail, Gmail, Outlook) et voir comment les couleurs et les images se comportent en mode sombre.
