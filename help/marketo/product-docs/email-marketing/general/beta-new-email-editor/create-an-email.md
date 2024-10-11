---
description: Création d’un courrier électronique - Documents Marketo - Documentation du produit
title: Créer un email
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 2d69e52883d141e3976c6d4fc1de6038675af602
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 7%

---

# Créer un email {#create-an-email}

Texte d&#39;introduction ici.

>[!IMPORTANT]
>
>Cet article est destiné aux membres du nouvel éditeur de messagerie du Marketo Engage fermé en version bêta uniquement. S&#39;il vous plaît, ne diffusez pas.

1. Connectez-vous à Marketo Engage via [Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"}.

1. Dans My Marketo, sélectionnez **Design Studio**.

   ![](assets/create-an-email-1.png)

1. Dans l’arborescence, sélectionnez **Emails (New Editor)**.

   ![](assets/create-an-email-2.png)

1. Cliquez sur le bouton **Créer un email** .

   ![](assets/create-an-email-3.png)

1. Saisissez un nom d’email et un objet. Cliquez sur **Créer**.

   ![](assets/create-an-email-4.png)

C&#39;est tout. Il est maintenant temps de concevoir votre email.

## Choisissez votre type de contenu {#choose-your-content-type}

1. Dans l&#39;email que vous venez de créer, cliquez sur **+ Ajouter le contenu de l&#39;email**.

   CAPTURE D’ÉCRAN

1. La page &quot;Créer votre email&quot; se charge. Vous pouvez choisir parmi plusieurs options :

* [Concevoir à partir de zéro](#design-from-scratch) à l’aide de l’éditeur de courrier électronique

* [Importez votre propre HTML](#import-html) via un HTML ou un fichier zip

* [Sélectionnez un modèle existant](#choose-a-template) (un de nos échantillons ou un que vous avez déjà enregistré)

### Créer en partant de zéro {#design-from-scratch}

Lorsque vous partez de zéro dans l&#39;éditeur d&#39;email, utilisez les options ci-dessous pour définir votre contenu.

1. Dans la page d’accueil Concevoir votre modèle, sélectionnez **Concevoir à partir de zéro**.

Ajoutez la structure et le contenu à votre email.

Ajoutez des images.

Personnalisez votre contenu.

Vérifier et mettre à jour les liens.

### Importer du contenu HTML {#import-html}

Vous pouvez importer du contenu d’HTML existant pour concevoir vos modèles d’email. Le contenu peut être :

* Un fichier d’HTML avec une feuille de style intégrée

* Fichier .zip contenant un fichier d’HTML, la feuille de style (.css) et les images

>[!NOTE]
>
>Il n’existe aucune contrainte sur la structure des fichiers .zip. Cependant, les références doivent être relatives et s’ajuster à l’arborescence du dossier .zip.

1. Dans la page Concevoir votre modèle, sélectionnez **Importer l&#39;HTML**.

   CAPTURE D’ÉCRAN

1. Faites glisser et déposez le fichier d’HTML ou .zip de votre choix, puis cliquez sur **Importer**.

   CAPTURE D’ÉCRAN

>[!NOTE]
>
>Lorsque le contenu de l’HTML est chargé, votre contenu est en mode de compatibilité. Dans ce mode, vous pouvez uniquement personnaliser votre texte, ajouter des liens ou inclure des ressources à votre contenu.

Vous pouvez apporter les modifications souhaitées au contenu importé à l’aide des [ outils de l’éditeur de courrier électronique](#add-structure-and-content).

### Choisir un modèle {#choose-a-template}

Deux types de modèles sont proposés.

* Exemples de modèles : Marketo Engage propose quatre modèles d&#39;email d&#39;usine.

* Modèles enregistrés : il s’agit de modèles entièrement créés à l’aide du menu Modèles ou d’un email que vous avez créé et que vous avez choisi d’enregistrer en tant que modèle.

>[!BEGINTABS]

>[!TAB Exemples de modèles]

Choisissez l&#39;un de nos modèles d&#39;usine pour démarrer rapidement votre conception d&#39;email.

1. Dans la page Créer votre email, sélectionnez **Exemples de modèles**.

   CAPTURE D’ÉCRAN

1. Sélectionnez le modèle de votre choix.

   CAPTURE D’ÉCRAN

1. Un aperçu s’affiche. Pour confirmer votre sélection, cliquez sur **Utiliser ce modèle**.

   CAPTURE D’ÉCRAN

>[!TAB Modèles enregistrés]

Sélectionnez l’un de vos modèles créés précédemment.

1. Dans la page Créer votre email , sélectionnez Modèles enregistrés .

   CAPTURE D’ÉCRAN

1. Sélectionnez le modèle de votre choix.

   CAPTURE D’ÉCRAN

1. Un aperçu s’affiche. Pour confirmer votre sélection, cliquez sur **Utiliser ce modèle**.

   CAPTURE D’ÉCRAN

>[!ENDTABS]

## Ajouter la structure et le contenu {#add-structure-and-content}

1. Pour commencer à créer ou modifier du contenu, faites glisser et déposez un élément de Structures sur la zone de travail. Modifiez ses paramètres dans le volet de droite.

   >[!TIP]
   >
   >Sélectionnez le composant n:n colonne pour définir le nombre de colonnes de votre choix (entre trois et dix). Vous pouvez également définir la largeur de chaque colonne en déplaçant les flèches sous la colonne.

   CAPTURE D’ÉCRAN

   >[!NOTE]
   >
   >La taille de chaque colonne ne peut pas être inférieure à 10 % de la largeur totale du composant de structure. Seules les colonnes vides peuvent être supprimées.

1. Dans la section Contenu , faites glisser les éléments de votre choix sur un ou plusieurs composants de structure.

   CAPTURE D’ÉCRAN

1. Chaque composant peut être personnalisé à partir des onglets Paramètres ou Style . Modifiez la police, le style de texte, la marge, etc.

CAPTURE D’ÉCRAN

### Ajout d’Assets {#add-assets}

Dans le sélecteur de ressources, vous pouvez sélectionner directement des ressources stockées dans la bibliothèque Assets. Double-cliquez sur le dossier contenant vos ressources. Glissez et déposez-les dans un composant de structure.

Insérez des champs de personnalisation pour personnaliser votre contenu à partir des attributs de profil, des appartenances à l’audience, des attributs contextuels, etc.

Cliquez sur Activer le contenu des conditions pour ajouter du contenu dynamique et adapter le contenu aux profils ciblés selon des règles conditionnelles.

Cliquez sur l’onglet Liens du volet de gauche pour afficher toutes les URL de votre contenu qui seront suivies. Vous pouvez modifier leur type de suivi ou libellé et ajouter des balises si nécessaire.

Si nécessaire, vous pouvez personnaliser davantage votre email en cliquant sur Passer à l’éditeur de code dans le menu avancé. Vous pouvez ainsi modifier le code source de l’email, par exemple pour ajouter des balises d’HTML personnalisées ou de suivi.

ATTENTION
Vous ne pouvez pas revenir au concepteur visuel de cet email après avoir basculé vers l’éditeur de code.

Une fois votre contenu prêt, cliquez sur le bouton Simuler le contenu pour vérifier le rendu. Vous pouvez choisir la vue bureau ou la vue mobile.

Une fois prêt, cliquez sur Enregistrer .





## Vérification des alertes {#check-alerts}

Lorsque vous concevez votre contenu, des alertes s’affichent dans l’interface (en haut à droite de l’écran) lorsque des paramètres clés sont manquants.

Il existe deux types d’alertes :

**Avertissements**

Les avertissements se rapportent aux recommandations et aux bonnes pratiques, telles que :

* **Le lien d’exclusion n’est pas présent dans le corps de l’email** : bien que les liens de désabonnement soient obligatoires, l’ajout de ces liens au corps de votre email est une bonne pratique.

>[!NOTE]
>
>L’ajout d’une option de désabonnement n’est pas nécessaire pour les [emails opérationnels](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md) (hors marketing).

* **La version texte de l’HTML est vide** : vous devez définir une version texte du corps de votre email lorsque le contenu de l’HTML ne peut pas être affiché.

* **Le lien vide est présent dans le corps de l’email** : vérifiez que tous les liens de votre email sont corrects.

* **La taille de l&#39;email a dépassé la limite de 100 Ko** : pour une diffusion optimale, assurez-vous que la taille de l&#39;email ne dépasse pas 100 Ko.

**Erreurs**

Les erreurs vous empêchent d’envoyer ou de tester l’email jusqu’à ce qu’il soit résolu :

* **Objet manquant** : une ligne d’objet d’email est requise.

* **La version email du message est vide** : cette erreur se produit lorsque le contenu de l&#39;email n&#39;a pas été configuré.

## Tester votre email

Lorsque le contenu de votre message est défini, vous pouvez utiliser des profils de test pour le prévisualiser, envoyer des bons à tirer et contrôler le rendu de votre message sur les clients courants de bureau, de mobile et web. Si vous avez inséré du contenu personnalisé, vous pouvez vérifier son affichage dans le message à l’aide des données de profil de test.

Pour prévisualiser le contenu de votre email, cliquez sur **Simuler le contenu**, puis ajoutez un profil de test pour vérifier votre message à l’aide des données de profil de test.

CAPTURE D’ÉCRAN

## Référencer un email {#reference-an-email}

Après avoir créé un email dans le nouvel éditeur, vous pouvez le référencer dans les campagnes dynamiques ou les listes dynamiques comme vous le feriez avec tout autre email.

* Référencez-le dans une liste dynamique en [ suivant les étapes habituelles](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md).

* Référencez-la dans une campagne dynamique en [ suivant les étapes habituelles](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

>[!NOTE]
>
>Seuls les emails enregistrés peuvent être référencés. Il n’existe pas d’état &quot;approuvé&quot; dans le nouvel éditeur de messagerie.
