---
title: Utiliser Experience Manager Assets
description: Découvrez comment utiliser des ressources d’image d’un référentiel AEM Assets connecté lors de la création de contenu dans Adobe Marketo Engage.
exl-id: c2172042-a35c-4179-bf81-6e96323bd4d4
source-git-commit: fddc2f24d9a66146f567c762305ab2825c2f29ae
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 1%

---

# Utilisation des ressources Experience Manager {#work-with-experience-manager-assets}

Connectez votre compte _Adobe Experience Manager Assets as a Cloud Service_ à votre instance Adobe Marketo Engage afin de pouvoir exploiter votre référentiel de ressources AEM dans Marketo Engage Email Designer.

>[!NOTE]
>
>Actuellement, seules les ressources d’image de _Adobe Experience Manager Assets_ sont prises en charge dans Marketo Engage. Les modifications apportées aux ressources doivent être effectuées à partir du référentiel central d’Adobe Experience Manager Assets. [En savoir plus](https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets){target="_blank"}

## Lien vers vos services cloud AEM {#link-to-your-aem-cloud-services}

Avant de pouvoir utiliser cette fonctionnalité, vous devez d’abord lier AEM Cloud Services à Adobe Marketo Engage.

+++Lier AEM Cloud Services et Marketo Engage

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Dans Marketo Engage, accédez à la zone **Admin** et sélectionnez **Adobe Experience Manager** dans l’arborescence de navigation de gauche.

   ![Sélectionnez Adobe Experience Manager dans la section Admin](assets/access-the-ai-assistant-content-accelerator-1.png){width="800" zoomable="yes"}

1. Cliquez sur **Modifier** en regard de _Services cloud Adobe Experience Manager_.

   ![Cliquez sur MODIFIER](assets/access-the-ai-assistant-content-accelerator-2.png){width="400" zoomable="yes"}

1. Sélectionnez un ou plusieurs référentiels.

   ![Sélectionner un référentiel](assets/access-the-ai-assistant-content-accelerator-3.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Seuls les référentiels qui ont été associés dans la même organisation IMS que votre abonnement Marketo Engage sont répertoriés.

1. Vous devez ajouter un [certificat d’identification de service](https://experienceleague.adobe.com/fr/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) pour configurer le référentiel. Cliquez sur le bouton **+ Ajouter un certificat**.

   ![Ajouter un certificat](assets/access-the-ai-assistant-content-accelerator-4.png){width="800" zoomable="yes"}

1. Effectuez un glisser-déposer de votre certificat (fichier JSON uniquement) ou sélectionnez-le depuis votre ordinateur. Cliquez sur **Ajouter** lorsque vous avez terminé.

   ![Recherchez le certificat sur votre ordinateur](assets/access-the-ai-assistant-content-accelerator-5.png){width="600" zoomable="yes"}

1. Le référentiel configuré est affiché ci-dessous, ainsi que le statut et l’expiration. Cliquez sur le bouton représentant des points de suspension (**...**) pour afficher le certificat. Sinon, c&#39;est fini.

   ![Le certificat a été ajouté](assets/access-the-ai-assistant-content-accelerator-6.png){width="700" zoomable="yes"}

Désormais, toutes les images de la bibliothèque de gestion des ressources numériques de ce référentiel sont accessibles à partir du Designer de messagerie Marketo Engage.

+++

## Utilisation des ressources AEM {#working-with-aem-assets}

Lorsque vous utilisez ces ressources numériques, les dernières modifications apportées à _Assets as a Cloud Service_ se propagent automatiquement aux campagnes par e-mail actives par le biais de références liées. Si des images sont supprimées dans _Adobe Experience Manager Assets as a Cloud Service_, les images s’affichent avec une référence rompue dans vos e-mails. Lorsque des ressources actuellement utilisées dans Marketo Engage sont modifiées ou supprimées, les auteurs d’e-mails sont avertis des modifications de l’image. Toutes les modifications apportées aux ressources doivent être effectuées dans le référentiel central d’Adobe Experience Manager Assets.

### Utiliser AEM Assets comme source d’images {#use-aem-assets-as-the-image-source}

Si votre environnement comporte une ou plusieurs connexions au référentiel de ressources, vous pouvez désigner AEM Assets comme source des ressources lorsque vous créez ou affichez les détails d’un e-mail, d’un modèle d’e-mail ou d’un fragment visuel.

* Lors de la création de contenu, choisissez `AEM Assets` comme élément **[!UICONTROL Image Source]** dans la boîte de dialogue.

![Sélectionnez AEM Assets comme source d’image dans la boîte de dialogue de création](assets/work-with-experience-manager-assets-1.png){width="400" zoomable="yes"}

* Lors de l’ouverture d’une ressource de contenu existante, choisissez `AEM Assets` dans la section _[!UICONTROL Corps]_ à droite.

![Sélectionnez AEM Assets comme source d’image dans les propriétés](assets/work-with-experience-manager-assets-2.png){width="700" zoomable="yes"}

### Accès aux ressources pour la création {#access-assets-for-authoring}

>[!IMPORTANT]
>
>Un administrateur doit ajouter des utilisateurs qui doivent accéder aux ressources aux profils de produit Utilisateurs consommateurs Assets et/ou Utilisateurs Assets . [En savoir plus](https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

Dans l’éditeur de contenu visuel, cliquez sur l’icône _Sélecteur de ressources Experience Manager_ dans la barre latérale gauche. Le panneau Outils devient alors une liste des ressources disponibles dans le référentiel sélectionné.

![Cliquez sur l’icône du sélecteur Assets pour accéder aux ressources d’image](assets/work-with-experience-manager-assets-3.png){width="700" zoomable="yes"}

Si plusieurs référentiels AEM sont connectés, cliquez sur le bouton **[!UICONTROL Gérer en tant que]** pour choisir le référentiel à utiliser.

![Choisissez un référentiel AEM Assets pour accéder aux ressources d’image](assets/work-with-experience-manager-assets-4.png){width="700" zoomable="yes"}

Choisissez le référentiel de votre choix.

![Choisissez un référentiel AEM Assets pour accéder aux ressources d’image](assets/work-with-experience-manager-assets-5.png){width="500" zoomable="yes"}

Il existe plusieurs méthodes pour ajouter une ressource d’image à la zone de travail visuelle :

* Glissez-déposez une miniature d’image à partir du volet de navigation de gauche.

![Choisissez un référentiel AEM Assets pour accéder aux ressources d’image](assets/work-with-experience-manager-assets-6.png){width="700" zoomable="yes"}

* Ajoutez un composant d’image à la zone de travail, puis cliquez sur **[!UICONTROL Parcourir]** pour afficher la boîte de dialogue _[!UICONTROL Sélectionner Assets]_.

  Dans la boîte de dialogue, vous pouvez choisir une image dans le référentiel sélectionné.

  Plusieurs outils sont disponibles pour vous aider à localiser la ressource dont vous avez besoin.

![Utilisez l’outil dans la boîte de dialogue Sélectionner Assets pour rechercher et sélectionner une ressource image](assets/work-with-experience-manager-assets-7.png){width="700" zoomable="yes"}

* Modifiez le **[!UICONTROL Référentiel]** en haut à droite.

* Cliquez sur **[!UICONTROL Gérer les ressources]** en haut à droite pour ouvrir le référentiel Assets dans un autre onglet du navigateur et utiliser les outils de gestion d’AEM Assets.

* Cliquez sur le sélecteur _Type de vue_ en haut à droite pour remplacer l’affichage par **[!UICONTROL Vue Liste]**, **[!UICONTROL Vue Grille]**, **[!UICONTROL Vue Galerie]** ou **[!UICONTROL Vue Cascade]**.

* Cliquez sur l’icône _Ordre de tri_ pour modifier l’ordre de tri entre croissant et décroissant.

* Cliquez sur la flèche du menu **[!UICONTROL Trier par]** pour remplacer les critères de tri par **[!UICONTROL Nom]**, **[!UICONTROL Taille]** ou **[!UICONTROL Modifié]**.

* Cliquez sur l’icône _Filtrer_ en haut à gauche pour filtrer les éléments affichés en fonction de vos critères.

* Saisissez du texte dans le champ Rechercher pour filtrer les éléments affichés afin qu’ils correspondent au nom de la ressource.

![Utilisez les filtres et le champ de recherche pour localiser la ressource](assets/work-with-experience-manager-assets-8.png){width="700" zoomable="yes"}
