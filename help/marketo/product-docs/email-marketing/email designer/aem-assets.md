---
title: Utiliser Experience Manager Assets
description: Découvrez comment utiliser des ressources d’image d’un référentiel AEM Assets connecté lors de la création de contenu dans Adobe Marketo Engage.
hide: true
hidefromtoc: true
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# Utilisation de ressources Experience Manager

Lorsqu’Adobe Experience Manager Assets as a Cloud Service est intégré à Adobe Marketo Engage, vous pouvez facilement découvrir et accéder aux ressources numériques à utiliser dans votre contenu marketing. Lorsque vous créez votre contenu, les ressources sont accessibles à partir de l’élément _[!UICONTROL Assets]_ sur la navigation de gauche, ainsi que lors de la création de contenu d’e-mail pour un parcours de compte. Vous pouvez également charger des ressources vers le référentiel AEM Assets as a Cloud Service connecté directement depuis Adobe Journey Optimizer B2B edition.

>[!NOTE]
>
>Actuellement, seules les ressources d’image d’Adobe Experience Manager Assets sont prises en charge dans Adobe Journey Optimizer B2B edition. Les modifications apportées aux ressources doivent être effectuées à partir du référentiel central d’Adobe Experience Manager Assets. [En savoir plus](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets)

Lorsque vous utilisez ces ressources numériques, les dernières modifications apportées à Assets as a Cloud Service se propagent automatiquement aux campagnes par e-mail actives par le biais de références liées. Si des images sont supprimées dans Adobe Experience Manager Assets as a Cloud Service, elles apparaissent avec une référence rompue dans les emails. Lorsque des ressources actuellement utilisées dans les parcours de compte sont modifiées ou supprimées, les auteurs de parcours sont informés des modifications apportées à l’image et de la liste des parcours qui utilisent l’image. Toutes les modifications apportées aux ressources doivent être effectuées dans le référentiel central d’Adobe Experience Manager Assets.

## Utiliser AEM Assets comme source d’images

Si votre environnement comporte une ou plusieurs connexions au référentiel Assets, vous pouvez désigner AEM Assets comme source des ressources lorsque vous créez ou affichez les détails d’un e-mail, d’un modèle d’e-mail ou d’un fragment visuel.

* Lorsque vous créez un contenu, choisissez `AEM Assets` comme élément **[!UICONTROL Image Source]** dans la boîte de dialogue.

CAPTURE D’ÉCRAN

* Lorsque vous ouvrez une ressource de contenu existante, choisissez `AEM Assets` dans le panneau _[!UICONTROL Corps]_ à droite.

CAPTURE D’ÉCRAN

## Accès aux ressources pour la création

>[!IMPORTANT]
>
>Un administrateur doit ajouter les utilisateurs qui doivent accéder à Assets aux profils de produit Utilisateurs consommateurs d’Assets et/ou Utilisateurs Assets . [En savoir plus](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

Dans l’éditeur de contenu visuel, cliquez sur l’icône _Sélecteur de ressources_ dans la barre latérale gauche. Le panneau Outils devient alors une liste des ressources disponibles dans le référentiel sélectionné.

CAPTURE D’ÉCRAN

Si plusieurs référentiels AEM sont connectés, cliquez sur la flèche de menu correspondant à **[!UICONTROL Référentiel]** pour choisir le référentiel à utiliser.

CAPTURE D’ÉCRAN

Il existe plusieurs méthodes pour ajouter une ressource d’image à la zone de travail visuelle :

* Glissez-déposez une miniature d’image à partir du volet de navigation de gauche.

CAPTURE D’ÉCRAN

* Ajoutez un composant d’image à la zone de travail, puis cliquez sur **[!UICONTROL Parcourir]** pour afficher la boîte de dialogue _[!UICONTROL Sélectionner Assets]_.

  Dans la boîte de dialogue, vous pouvez choisir une image dans le référentiel sélectionné.

  Plusieurs outils sont disponibles pour vous aider à localiser la ressource dont vous avez besoin.

CAPTURE D’ÉCRAN

* Modifiez le **[!UICONTROL Référentiel]** en haut à droite.

* Cliquez sur **[!UICONTROL Gérer les ressources]** en haut à droite pour ouvrir le référentiel Assets dans un autre onglet du navigateur et utiliser les outils de gestion d’AEM Assets.

* Cliquez sur le sélecteur _Type de vue_ en haut à droite pour remplacer l’affichage par **[!UICONTROL Vue Liste]**, **[!UICONTROL Vue Grille]**, **[!UICONTROL Vue Galerie]** ou **[!UICONTROL Vue Cascade]**.

* Cliquez sur l’icône _Ordre de tri_ pour modifier l’ordre de tri entre croissant et décroissant.

* Cliquez sur la flèche du menu **[!UICONTROL Trier par]** pour remplacer les critères de tri par **[!UICONTROL Nom]**, **[!UICONTROL Taille]** ou **[!UICONTROL Modifié]**.

* Cliquez sur l’icône _Filtrer_ en haut à gauche pour filtrer les éléments affichés en fonction de vos critères.

* Saisissez du texte dans le champ Rechercher pour filtrer les éléments affichés afin qu’ils correspondent au nom de la ressource.

CAPTURE D’ÉCRAN
