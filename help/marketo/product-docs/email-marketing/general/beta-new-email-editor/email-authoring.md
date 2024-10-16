---
description: Création d’emails - Documents Marketo - Documentation du produit
title: Création d’emails
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 43a0d32c2bc6a5f72a13cb6022b00c058d9c3269
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 4%

---

# Création d’emails {#email-authoring}

Découvrez comment créer, personnaliser et prévisualiser des emails dans le nouveau Designer Marketo Engage Email.

>[!IMPORTANT]
>
>Cet article est destiné uniquement aux membres de la version bêta de l’éditeur de messagerie du nouveau Marketo Engage. S&#39;il vous plaît, ne diffusez pas.

## Création d’un e-mail {#create-an-email}

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

1. Dans l&#39;email que vous venez de créer, cliquez sur **Ajouter le contenu de l&#39;email**.

   ![](assets/choose-your-content-type-1.png)

1. La page _Créer votre email_ se charge. Vous pouvez choisir parmi plusieurs options :

* [Concevoir à partir de zéro](#design-from-scratch) à l’aide de l’éditeur visuel de courrier électronique

* [Importez votre propre HTML](#import-html) via un HTML ou un fichier zip

* [Sélectionnez un modèle existant](#choose-a-template) (un de nos échantillons ou un que vous avez déjà enregistré)

### Créer en partant de zéro {#design-from-scratch}

Lorsque vous partez de zéro dans l&#39;éditeur d&#39;email, utilisez les options ci-dessous pour définir votre contenu.

1. Sur la page _Créer votre email_, sélectionnez **Concevoir à partir de zéro**.

1. Ajoutez [structure et contenu](#add-structure-and-content) à votre email.

1. Ajoutez [images](#add-assets).

1. [Personnalisez](#personalize-content) votre contenu.

1. Vérifiez les liens et [modifiez le suivi](#edit-url-tracking).

### Importer du contenu HTML {#import-html}

Vous pouvez importer du contenu d&#39;HTML existant pour concevoir votre email. Le contenu peut être :

* Un fichier d’HTML avec une feuille de style intégrée

* Fichier .zip contenant un fichier d’HTML, la feuille de style (.css) et les images

>[!NOTE]
>
>Il n’existe aucune contrainte sur la structure des fichiers .zip. Cependant, les références doivent être relatives et s’ajuster à l’arborescence du dossier .zip.

1. Dans la page Concevoir votre modèle, sélectionnez **Importer l&#39;HTML**.

1. Faites glisser et déposez le fichier d’HTML ou .zip souhaité (ou sélectionnez un fichier sur votre ordinateur) et cliquez sur **Importer**.

   ![](assets/authoring-import-your-html-1.png)

>[!NOTE]
>
>Lorsque le contenu de l’HTML est chargé, votre contenu est en mode de compatibilité. Dans ce mode, vous pouvez uniquement personnaliser votre texte, ajouter des liens ou ajouter des ressources à votre contenu.

Vous pouvez apporter les modifications souhaitées au contenu importé à l’aide des [outils visuels de l’éditeur d’email](#add-structure-and-content).

### Choisir un modèle {#choose-a-template}

Deux types de modèles sont proposés.

* Exemples de modèles : Marketo Engage propose quatre modèles d&#39;email d&#39;usine.

* Modèles enregistrés : il s’agit de modèles entièrement créés à l’aide du menu Modèles ou d’un email que vous avez créé et que vous avez choisi d’enregistrer en tant que modèle.

>[!BEGINTABS]

>[!TAB Exemples de modèles]

Choisissez l&#39;un des modèles d&#39;usine pour démarrer la conception de votre modèle d&#39;email.

1. L’onglet Exemples de modèles est ouvert par défaut.

1. Sélectionnez le modèle à utiliser.

   ![](assets/authoring-sample-templates-1.png)

1. Cliquez sur **Utiliser ce modèle**.

   ![](assets/authoring-sample-templates-2.png)

1. Modifiez le contenu suivant vos besoins à l’aide du concepteur de contenu visuel.

>[!TAB Modèles enregistrés]

1. Cliquez sur l’onglet **Modèles enregistrés** et sélectionnez le modèle de votre choix.

   ![](assets/authoring-saved-templates-1.png)

1. Cliquez sur **Utiliser ce modèle**.

   ![](assets/authoring-saved-templates-2.png)

1. Modifiez le contenu suivant vos besoins à l’aide du concepteur de contenu visuel.

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

```
ADD ASSETS OR ADD IMAGES? WHAT OTHER ASSETS CAN YOU ADD?
```

```
Access assets stored in the Assets library. IMAGES AND FILES ONLY?
```

1. Pour accéder à vos images, cliquez sur l’icône Sélecteur de ressources .

   CAPTURE D’ÉCRAN

1. Faites glisser et déposez l’image souhaitée dans un composant de structure.

   CAPTURE D’ÉCRAN

   >[!NOTE]
   >
   >Pour remplacer une image existante, sélectionnez-la, puis cliquez sur **Sélectionner une ressource** dans l’onglet Paramètres à droite.

Cliquez sur Activer le contenu des conditions pour ajouter du contenu dynamique et adapter le contenu aux profils ciblés selon des règles conditionnelles.



Si nécessaire, vous pouvez personnaliser davantage votre email en cliquant sur Passer à l’éditeur de code dans le menu avancé. Vous pouvez ainsi modifier le code source de l’email, par exemple pour ajouter des balises d’HTML personnalisées ou de suivi.

ATTENTION
Vous ne pouvez pas revenir au concepteur visuel de cet email après avoir basculé vers l’éditeur de code.

Une fois votre contenu prêt, cliquez sur le bouton Simuler le contenu pour vérifier le rendu. Vous pouvez choisir la vue bureau ou la vue mobile.

Une fois prêt, cliquez sur Enregistrer .

### Calques, paramètres et styles {#layers-settings-styles}

```
ARE THEY CALLED LAYERS OR COMPONENTS
```

Ouvrez l’arborescence de navigation pour accéder à des structures spécifiques et à leurs colonnes/composants afin d’effectuer des modifications plus granulaires.

1. Pour y accéder, cliquez sur l&#39;icône Arborescence de navigation .

CAPTURE D’ÉCRAN




### Personnaliser le contenu {#personalize-content}

Les jetons fonctionnent dans le nouvel éditeur de la même manière que dans l’ancien, mais l’icône est différente. L’exemple ci-dessous illustre l’ajout d’un jeton de prénom avec du texte de remplacement.

1. Sélectionnez le composant de texte. Placez le curseur à l’endroit où vous souhaitez que le jeton s’affiche et cliquez sur l’icône **Ajouter une personnalisation** .

   ![](assets/authoring-personalize-content-1.png)

1. Cliquez sur le [type de jeton](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} souhaité.

   ![](assets/authoring-personalize-content-2.png)

1. Recherchez le jeton souhaité et cliquez sur l’icône **...** (cliquez sur l’icône + pour ajouter un jeton sans texte de secours).

   ![](assets/authoring-personalize-content-3.png)

   >[!NOTE]
   >
   >&quot;Texte de rechange&quot; est le nouveau terme de l’éditeur pour la valeur par défaut. Exemple : ``{{lead.First Name:default=Friend}}``. Il est recommandé si la personne n’a pas de valeur dans le champ que vous choisissez.

1. Définissez votre texte de secours et cliquez sur **Ajouter**.

   ![](assets/authoring-personalize-content-4.png)

1. Cliquez sur **Enregistrer**.

### Modifier le suivi des URL {#edit-url-tracking}

Il arrive que vous ne souhaitiez pas activer l’URL de suivi Marketo sur un lien d’un email. Cela s’avère utile lorsque la page de destination ne prend pas en charge les paramètres d’URL et peut entraîner la rupture du lien.

1. Cliquez sur l&#39;icône Liens pour afficher toutes les URL de votre email.

   CAPTURE D’ÉCRAN

1. Cliquez sur l’icône représentant un crayon pour modifier le suivi des liens de votre choix.

   CAPTURE D’ÉCRAN

   ```
   LABEL?
   
   TAGS?
   ```

   <table><tbody>
     <tr>
       <td><b>Suivi sans mkt_tok</b></td>
       <td>définition</td>
     </tr>
     <tr>
       <td><b>Suivi avec mkt_tok</b></td>
       <td>définition</td>
     </tr>
     <tr>
       <td><b>Ne pas suivre</b></td>
       <td>définition</td>
     </tr>
   </tbody>
   </table>

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

## Vérification des alertes {#check-alerts}

Lorsque vous concevez votre contenu, des alertes s’affichent en haut à droite de l’écran lorsque des paramètres clés sont manquants.

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

## Tester votre email {#test-your-email}

Lorsque le contenu de votre message est défini, vous pouvez utiliser des profils de test pour le prévisualiser, envoyer des bons à tirer et contrôler le rendu de votre message sur les clients courants de bureau, de mobile et web. Si vous avez inséré du contenu personnalisé, vous pouvez vérifier son affichage dans le message à l’aide des données de profil de test.

Pour prévisualiser le contenu de votre email, cliquez sur **Simuler le contenu**, puis ajoutez un profil de test pour vérifier votre message à l’aide des données de profil de test.

CAPTURE D’ÉCRAN

## Référencer un email {#reference-an-email}

Après avoir créé un email dans le nouvel éditeur, vous pouvez le référencer dans les campagnes dynamiques et/ou les listes dynamiques comme vous le feriez avec tout autre email.

* Référencez-le dans une liste dynamique en [ suivant les étapes habituelles](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md).

* Référencez-la dans une campagne dynamique en [ suivant les étapes habituelles](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

>[!NOTE]
>
>Seuls les emails enregistrés peuvent être référencés. Il n’existe pas d’état &quot;approuvé&quot; dans le nouvel éditeur de messagerie.

>[!MORELIKETHIS]
>
>[Modèles d’email](/help/marketo/product-docs/email-marketing/general/beta-new-email-editor/email-templates.md){target="_blank"} : découvrez comment créer, concevoir et accéder à un modèle d’email dans le nouvel éditeur.
