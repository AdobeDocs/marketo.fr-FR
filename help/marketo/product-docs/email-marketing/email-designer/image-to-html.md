---
title: Convertir des images en modèles HTML
description: Utilisez cet outil sans code pour transformer une image en modèle d’e-mail modifiable.
solution: Marketo Engage
product: marketo
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 74c8b1597bed7e2ac827bea444200dacfe4b29a5
workflow-type: tm+mt
source-wordcount: '1287'
ht-degree: 1%

---

# Convertir des images en modèles HTML {#image-to-html}

## Vue d’ensemble {#overview}

Le convertisseur d’images vers HTML accélère considérablement la création d’e-mails en convertissant des images statiques en modèles de contenu d’e-mail HTML entièrement personnalisables et modulaires. Cet outil sans code vous permet de transformer des conceptions visuelles de concepteurs graphiques ou d’outils de conception en modèles d’e-mail réactifs et modifiables, pouvant être réutilisés à maintes reprises.

Grâce à la technologie d’IA générative, le convertisseur image en HTML analyse la disposition, la typographie, les couleurs et les éléments visuels de votre image et génère un code HTML propre et modulaire qui conserve la fidélité de la conception tout en garantissant une modifiabilité et une compatibilité complètes avec le Designer Email.

>[!PREREQUISITES]
>
>* Vous devez d’abord accepter les conditions générales [Core Gen-AI et les conditions supplémentaires](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} relatives à l’utilisation de la fonctionnalité Gen-AI dans le Designer d’e-mail. Pour plus d’informations, contactez l’équipe du compte Adobe (votre gestionnaire de compte).
>* Votre rôle Marketo doit disposer des autorisations _Accéder au modèle d’e-mail_ et _Modifier/générer le modèle d’e-mail_ activées [&#128279;](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#edit-a-role).

## Convertir une image {#convert-an-image}

Pour convertir une image en modèle d’e-mail HTML entièrement personnalisable, procédez comme suit.

>[!NOTE]
>
>Pour de meilleurs résultats, utilisez des images de haute qualité avec des éléments visuels clairs et du texte lisible. La largeur des images doit idéalement être comprise entre 600 et 800 pixels pour correspondre aux dimensions d’e-mail standard.

1. Dans _Design Studio_, cliquez sur **Modèles d’e-mail**, puis **Modèles d’e-mail (nouveau)**.

   ![](assets/image-to-html-1.png)

1. Cliquez sur **[!UICONTROL Convertir l’image en modèle]**.

   ![](assets/image-to-html-2.png)

1. Saisissez un _Nom du modèle_ et une description facultative. Vous pouvez également choisir le style de votre marque. Chargez ou faites glisser et déposez l’image souhaitée.

   ![](assets/image-to-html-3.png)

1. Faites défiler vers le bas et cochez la case _Le fichier de chargement ne contient pas..._ . Cliquez sur **Convertir**.

   ![](assets/image-to-html-4.png)

   >[!NOTE]
   >
   >Le processus de génération peut prendre jusqu’à cinq minutes selon la complexité et la taille de votre conception d’image. Le traitement de l’IA se produit en arrière-plan. Vous pouvez donc quitter cet écran et travailler sur d’autres tâches pendant que la conversion est en cours. Vous devrez peut-être actualiser l’écran de la bibliothèque _Modèle d’e-mail_ pour afficher le changement de statut.

1. Une fois la conversion terminée, votre modèle est automatiquement enregistré en tant que brouillon. Cliquez sur son nom pour l’afficher/le modifier.

   ![](assets/image-to-html-5.png)

1. Le modèle converti s’ouvre dans le Designer d’e-mail avec des fonctionnalités de modification complètes. Vous pouvez maintenant :

   * Modifier le contenu textuel et appliquer une personnalisation
   * Modification des images et ajout de liens
   * Ajuster les couleurs, les polices et le style
   * Ajouter, supprimer ou réorganiser des composants de contenu
   * Tirez parti de toutes les fonctionnalités de Designer par e-mail comme pour tout autre modèle

   ![](assets/image-to-html-6.png){width="800" zoomable="yes"}

1. Vous pouvez effectuer les ajustements souhaités pour affiner le modèle et respecter les directives de votre marque.

1. Une fois satisfait de votre modèle, cliquez sur **[!UICONTROL Enregistrer et fermer]** puis **Publier**.

Votre modèle est maintenant disponible dans la bibliothèque _Modèles d’e-mail_ et peut être utilisé lors de la création d’e-mails.

## Cas d&#39;utilisation courants {#use-cases}

Le convertisseur d’images en HTML est idéal pour :

* **Migration de plateforme** : vous effectuez une migration depuis une autre plateforme de marketing par e-mail ? Convertissez vos conceptions d’e-mail existantes en modèles HTML prêts pour Marketo Engage sans devoir reconstruire à partir de zéro
* **Conversion de maquettes de conception** : transformez des maquettes de conception d’outils tels que Photoshop, Figma ou d’autres logiciels de conception en modèles d’e-mail fonctionnels
* **Création rapide de modèles** : générez rapidement des modèles d’e-mail pour les campagnes sensibles au facteur temps, sans attendre les ressources de développement.
* **Création de bibliothèques de modèles** : créez une bibliothèque complète de modèles cohérents avec la marque que les membres de l’équipe non techniques peuvent personnaliser et déployer

## Bonnes pratiques {#best-practices}

**Avant de commencer**

* **Enregistrer le contenu existant** : la conversion d’une image vers HTML remplacera tout le contenu existant de votre e-mail. Enregistrez toujours votre travail actuel avant d’utiliser cette fonctionnalité.
* **Planifier votre workflow** : utilisez le convertisseur image vers HTML au début du processus de création d’e-mail ou assurez-vous que vous êtes prêt à remplacer tout le contenu actuel.

**Préparation des images**

* **Résolution** : utilisez des images haute résolution pour une meilleure reconnaissance du texte et une meilleure détection des éléments.
* **Clarté** : assurez-vous que le texte est clairement lisible et que les éléments visuels sont bien définis.
* **Largeur** : concevez des images aux largeurs d’e-mail standard (600 à 800 px) pour répondre aux exigences standard des clients de messagerie.
* **Format de fichier** : utilisez le format JPEG ou PNG pour éviter les images compressées ou de faible qualité.
* **Conception complète** : incluez la conception complète d’e-mail dans une seule image, de l’en-tête au pied de page.

**Considérations de conception**

* **Dispositions simples** : les dispositions simples et bien structurées se convertissent avec plus de précision que les conceptions très complexes.
* **Éléments standard** : utilisez des modèles de conception d’e-mail courants (en-tête, sections de corps, CTA, pied de page).
* **Lisibilité du texte** : assurez-vous que le contraste entre le texte et l’arrière-plan est suffisant.
* **Polices sécurisées pour le web** : les conceptions qui utilisent des polices sécurisées pour le web courantes auront une meilleure fidélité.
* **Évitez le chevauchement des éléments** : conservez des éléments de conception clairement séparés pour une meilleure reconnaissance de la structure.

**Après la conversion**

* **Vérifier votre brouillon** : une fois la conversion terminée, votre modèle est automatiquement enregistré en tant que brouillon. Prenez le temps d’examiner attentivement l’HTML générée pour en vérifier la précision.
* **Tester minutieusement** : tester l’e-mail sur différents clients de messagerie et appareils. Pour des résultats plus rapides, tirez parti de l’intégration [Litmus](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).
* **Affiner manuellement** : effectuez les ajustements nécessaires à l’aide des fonctionnalités d’édition complète du Designer Email.
* **Alignement de la marque** : vérifiez que les couleurs, les polices et le style correspondent à vos directives de marque.
* **Personalization** : ajoutez du contenu dynamique et des jetons de personnalisation selon vos besoins.
* **Accessibilité** : passez en revue et améliorez les fonctionnalités d’accessibilité si nécessaire.

## Restrictions et considérations {#limitations}

Gardez à l’esprit les restrictions suivantes lorsque vous utilisez le convertisseur Image vers HTML.

* **Interprétation de l’IA** : l’IA génère HTML en fonction d’une interprétation visuelle de votre image. Les conceptions complexes ou inhabituelles peuvent nécessiter des réglages manuels après la conversion.

* **Précision du texte** : bien que l’IA tente de reconnaître et de reproduire le texte avec précision, vérifiez toujours le contenu du texte et apportez les corrections nécessaires.

* **Contenu dynamique** : le processus de conversion crée une HTML statique en fonction de votre image. Vous devrez ajouter manuellement la personnalisation, le contenu dynamique et le suivi après la conversion.

* **Dispositions complexes** : les conceptions très complexes avec des superpositions complexes, des formes inhabituelles ou des éléments non standard peuvent ne pas se convertir parfaitement. Des conceptions plus simples donnent généralement de meilleurs résultats.

* **Temps de traitement** : le processus de conversion peut prendre jusqu’à cinq minutes selon la complexité et la taille de votre image. Le traitement par l’IA se produit en arrière-plan, ce qui vous permet de travailler sur d’autres tâches sans garder l’écran ouvert. Le modèle est automatiquement enregistré en tant que brouillon une fois la conversion terminée.

>[!NOTE]
>
>Le convertisseur d’images en HTML est conçu pour fournir un point de départ solide pour la création d’e-mails. L’HTML générée doit être examinée et affinée à l’aide du Designer d’e-mail afin de s’assurer qu’elle répond à vos besoins.

## Questions fréquentes {#faq}

+++Qu’advient-il de mon contenu d’e-mail existant lorsque j’utilise le convertisseur Image vers HTML ?

Tout le contenu existant de votre e-mail sera supprimé et remplacé par le modèle nouvellement généré lorsque vous chargez une image à des fins de conversion. Veillez à enregistrer tout contenu important avant d’utiliser cette fonctionnalité. Il est préférable d’utiliser le convertisseur image vers HTML au début de votre processus de création d’e-mail.

+++

+++Quels formats de fichier sont pris en charge ?

Le convertisseur image vers HTML prend en charge les formats d’image JPEG (.jpg, .jpeg) et PNG (.png).

+++

+++Combien de temps dure le processus de conversion ?

La conversion peut prendre jusqu’à cinq minutes, selon la complexité et la taille de votre conception d’image. Le traitement de l’IA s’effectue en arrière-plan, ce qui vous permet de quitter l’application et d’effectuer d’autres tâches ; il n’est pas nécessaire de garder l’écran ouvert. Une fois la conversion terminée, votre fichier est automatiquement enregistré en tant que brouillon pour que vous puissiez le réviser et le modifier.

+++

+++Puis-je modifier le modèle généré ?

Oui! Le modèle HTML généré s’ouvre dans le Designer d’e-mail avec des fonctionnalités d’édition complètes. Vous pouvez modifier tous les aspects du modèle, notamment le texte, les images, le style, la disposition et la structure.

+++

+++Que se passe-t-il si la conversion ne correspond pas exactement à ma conception ?

L’IA fait de son mieux pour interpréter avec précision votre conception, mais un certain raffinement manuel peut être nécessaire. Utilisez le Designer d’e-mail pour ajuster tous les éléments qui nécessitent des ajustements.

+++

+++Puis-je utiliser cette fonctionnalité pour les landing pages ou d’autres types de contenu ?

Le convertisseur image en HTML est actuellement conçu spécifiquement pour les modèles d’e-mail. Pour les autres types de contenu, utilisez les options de conception et d’importation standard disponibles dans le Designer d’e-mail.

+++

+++Puis-je réutiliser des modèles convertis dans plusieurs campagnes par e-mail ?

Oui! Les modèles créés avec le convertisseur image vers HTML sont automatiquement enregistrés dans votre bibliothèque _Modèles d’e-mail_. Vous pouvez désormais y accéder et les réutiliser dans n’importe quel e-mail.

+++
