---
description: Modèles de courrier électronique - Documents Marketo - Documentation du produit
title: Modèles d’e-mail
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 22f667b27168eafe51df75f81be74e18f5497c3f
workflow-type: tm+mt
source-wordcount: '1775'
ht-degree: 5%

---

# Modèles d’e-mail {#email-templates}

Pour accélérer et améliorer le processus de conception, vous pouvez créer des modèles d’email autonomes pour réutiliser facilement du contenu personnalisé.

>[!IMPORTANT]
>
>Cet article est destiné uniquement aux membres de la version bêta du nouveau Designer de messagerie du Marketo Engage. S&#39;il vous plaît, ne diffusez pas.

>[!NOTE]
>
>Les modèles d&#39;email du nouveau concepteur d&#39;email ne peuvent être utilisés que pour créer des emails dans le nouveau concepteur d&#39;email. Ils ne peuvent pas être référencés dans l’ancien éditeur d’email.

## Création d’un modèle de courrier électronique {#create-an-email-template}

1. Connectez-vous à Marketo Engage via [Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"}.

1. Dans My Marketo, sélectionnez **Design Studio**.

   ![](assets/create-an-email-template-1.png)

1. Dans l’arborescence, sélectionnez **Modèles d’email (nouvel éditeur)**.

   ![](assets/create-an-email-template-2.png)

1. Cliquez sur le bouton **Créer un modèle** .

   ![](assets/create-an-email-template-3.png)

1. Saisissez un nom de modèle et éventuellement une description. Cliquez sur **Créer**.

   ![](assets/create-an-email-template-4.png)

## Concevoir votre modèle {#design-your-template}

Dans la page _Concevoir votre modèle_ , vous pouvez choisir parmi quelques options. [Conception à partir de zéro](#design-from-scratch), [importez votre propre HTML](#import-html) ou [sélectionnez un modèle existant](#choose-a-template) (l’un de nos exemples ou celui que vous avez déjà enregistré).

![](assets/design-your-template-1.png)

### Créer en partant de zéro {#design-from-scratch}

Définissez votre contenu en ajoutant et en déplaçant des éléments structurels à l’aide d’actions de glisser-déposer simples.

1. Sur la page _Concevez votre modèle_, sélectionnez **Concevoir à partir de zéro**.

1. Ajoutez [structure et contenu](#add-structure-and-content).

### Importer votre HTML {#import-your-html}

Vous pouvez importer du contenu d’HTML existant pour concevoir vos modèles d’email. Le contenu peut être :

* Un fichier d’HTML avec une feuille de style intégrée

* Fichier .zip contenant un fichier d’HTML, la feuille de style (.css) et les images

>[!NOTE]
>
>Il n’existe aucune contrainte sur la structure des fichiers .zip. Cependant, les références doivent être relatives et s’ajuster à l’arborescence du dossier .zip.

1. Dans la page _Concevoir votre modèle_, sélectionnez **Importer l&#39;HTML**.

1. Faites glisser et déposez le fichier d’HTML ou .zip souhaité (ou sélectionnez un fichier sur votre ordinateur) et cliquez sur **Importer**.

   ![](assets/import-your-html-1.png)

   >[!NOTE]
   >
   >Lorsque le contenu de l’HTML est chargé, votre contenu est en mode de compatibilité. Dans ce mode, vous pouvez uniquement personnaliser votre texte, ajouter des liens ou ajouter des ressources à votre contenu.

1. Pour pouvoir exploiter les composants de contenu Designer par e-mail, cliquez sur l’onglet **Convertisseur d’HTMLS** et cliquez sur **Convertir**.

   CAPTURE D’ÉCRAN

   >[!CAUTION]
   >
   >L’utilisation d’une balise `<table>` comme première couche d’un fichier HTML peut entraîner une perte de style, y compris les paramètres d’arrière-plan et de largeur dans la balise de couche supérieure.

Vous pouvez maintenant personnaliser le fichier importé selon vos besoins à l’aide de l’éditeur visuel de messagerie.

### Choisir un modèle {#choose-a-template}

Deux types de modèles sont proposés.

* **Exemples de modèles** : Marketo Engage propose quatre modèles d’email d’usine.

* **Modèles enregistrés** : il s’agit de modèles que vous avez créés à partir de zéro à l’aide du menu Modèles ou d’un email que vous avez créé et que vous avez choisi d’enregistrer en tant que modèle.

>[!BEGINTABS]

>[!TAB Exemples de modèles]

Choisissez l&#39;un des modèles d&#39;usine pour démarrer la conception de votre modèle d&#39;email.

1. L’onglet Exemples de modèles est ouvert par défaut.

1. Sélectionnez le modèle à utiliser.

   ![](assets/sample-templates-1.png)

1. Cliquez sur **Utiliser ce modèle**.

   ![](assets/sample-templates-2.png)

1. Modifiez le contenu suivant vos besoins à l’aide du concepteur de contenu visuel.

>[!TAB Modèles enregistrés]

1. Cliquez sur l’onglet **Modèles enregistrés** et sélectionnez le modèle de votre choix.

   ![](assets/saved-templates-1.png)

1. Cliquez sur **Utiliser ce modèle**.

   ![](assets/saved-templates-2.png)

1. Modifiez le contenu suivant vos besoins à l’aide du concepteur de contenu visuel.

>[!ENDTABS]

## Ajouter la structure et le contenu {#add-structure-and-content}

1. Pour commencer à créer ou modifier du contenu, faites glisser et déposez un élément de Structures sur la zone de travail. Modifiez ses paramètres dans le volet de droite.

   >[!TIP]
   >
   >Sélectionnez le composant n:n colonne pour définir le nombre de colonnes de votre choix (entre trois et dix). Vous pouvez également définir la largeur de chaque colonne en déplaçant les flèches sous la colonne.

   ![](assets/add-structure-and-content-1.png)

   >[!NOTE]
   >
   >La taille de chaque colonne ne peut pas être inférieure à 10 % de la largeur totale du composant de structure. Seules les colonnes vides peuvent être supprimées.

1. Dans la section Contenu , faites glisser les éléments de votre choix sur un ou plusieurs composants de structure.

   ![](assets/add-structure-and-content-2.png)

1. Chaque composant peut être personnalisé à partir des onglets Paramètres ou Style . Modifiez la police, le style de texte, la marge, etc.

### Ajout d’Assets {#add-assets}

```
ADD ASSETS OR ADD IMAGES? WHAT OTHER ASSETS CAN YOU ADD??
```

```
Access assets stored in the Assets library. IMAGES AND FILES ONLY? - SEE EMAIL AUTHORING FOR ANSWERS - KG
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

Ouvrez l’arborescence de navigation pour accéder à des structures spécifiques et à leurs colonnes/composants afin d’effectuer des modifications plus granulaires. Pour y accéder, cliquez sur l&#39;icône Arborescence de navigation .

![](assets/layers-settings-styles-1.png)

L’exemple ci-dessous décrit les étapes à suivre pour ajuster la marge intérieure et l’alignement vertical à l’intérieur d’un composant de structure composé de colonnes.

1. Sélectionnez la colonne dans le composant de structure directement dans la zone de travail ou à l’aide de l’_Arborescence de navigation_ affichée à gauche.

1. Dans la barre d&#39;outils des colonnes, cliquez sur l&#39;outil _[!UICONTROL Sélectionner une colonne]_ et choisissez celle que vous souhaitez modifier.

   Vous pouvez également la sélectionner dans l&#39;arborescence. Les paramètres modifiables pour cette colonne sont affichés dans les onglets _[!UICONTROL Paramètres]_ et _[!UICONTROL Styles]_ à droite.

   ![](assets/layers-settings-styles-2.png)

1. Pour modifier les propriétés de colonne, cliquez sur l’onglet _[!UICONTROL Styles]_ à droite et modifiez-les selon vos besoins :

   * Pour **[!UICONTROL Background]**, modifiez la couleur d’arrière-plan selon les besoins.

     Décochez la case pour un arrière-plan transparent. Activez le paramètre **[!UICONTROL Image d&#39;arrière-plan]** pour utiliser une image comme arrière-plan au lieu d&#39;une couleur unie.

   * Pour **[!UICONTROL Alignement]**, sélectionnez l’icône _Haut_, _Milieu_ ou _Bas_.
   * Pour **[!UICONTROL Marge intérieure]**, définissez la marge intérieure de tous les côtés.

     Sélectionnez **[!UICONTROL Remplissage différent pour chaque côté]** si vous souhaitez ajuster la marge intérieure. Cliquez sur l’icône _Verrouiller_ pour interrompre la synchronisation.

   * Développez la section **[!UICONTROL Avancé]** pour définir des styles intégrés pour la colonne.

   ![](assets/layers-settings-styles-3.png)

1. Répétez ces étapes si nécessaire pour ajuster l’alignement et la marge intérieure des autres colonnes du composant.

1. Enregistrez vos modifications.

### Personnaliser le contenu {#personalize-content}

Les jetons fonctionnent dans le nouvel éditeur de la même manière que dans l’ancien, mais l’icône est différente. L’exemple ci-dessous illustre l’ajout d’un jeton de prénom avec du texte de remplacement.

1. Sélectionnez le composant de texte. Placez le curseur à l’endroit où vous souhaitez que le jeton s’affiche et cliquez sur l’icône **Ajouter une personnalisation** .

   ![](assets/personalize-content-1.png)

1. Cliquez sur le [type de jeton](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} souhaité.

   ![](assets/personalize-content-2.png)

1. Recherchez le jeton souhaité et cliquez sur l’icône **...** (cliquez sur l’icône + pour ajouter un jeton sans texte de secours).

   ![](assets/personalize-content-3.png)

   >[!NOTE]
   >
   >&quot;Texte de rechange&quot; est le nouveau terme de l’éditeur pour la valeur par défaut. Exemple : ``{{lead.First Name:default=Friend}}``. Il est recommandé si la personne n’a pas de valeur dans le champ que vous choisissez.

1. Définissez votre texte de secours et cliquez sur **Ajouter**.

   ![](assets/personalize-content-4.png)

1. Cliquez sur **Enregistrer**.

### Modifier le suivi des URL {#edit-url-tracking}

Il arrive que vous ne souhaitiez pas activer l’URL de suivi Marketo sur un lien d’un email. Cela s’avère utile lorsque la page de destination ne prend pas en charge les paramètres d’URL et peut entraîner la rupture du lien.

1. Cliquez sur l&#39;icône Liens pour afficher toutes les URL de votre email.

   ![](assets/edit-url-tracking-1.png)

1. Cliquez sur l’icône représentant un crayon pour modifier le suivi des liens de votre choix.

1. Cliquez sur la liste déroulante **Type de suivi** et effectuez votre sélection.

   ![](assets/edit-url-tracking-2.png)

   <table><tbody>
     <tr>
       <td><b>Suivi sans mkt_tok</b></td>
       <td>Active le suivi sur l’URL sans utiliser le paramètre de chaîne de requête mkt_tok dans l’URL de destination.</td>
     </tr>
     <tr>
       <td><b>Suivi avec mkt_tok</b></td>
       <td>Active le suivi sur l’URL à l’aide du paramètre de chaîne de requête mkt_tok dans l’URL de destination.</td>
     </tr>
     <tr>
       <td><b>Ne pas suivre</b></td>
       <td>Désactive le tracking de l'URL</td>
     </tr>
   </tbody>
   </table>

1. Vous pouvez éventuellement attribuer un libellé à l’URL ou ajouter des balises.

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

### Options d’affichage {#view-options}

Tirez parti des options de vue et de validation du contenu disponibles dans l’éditeur visuel de courrier électronique.

* Effectuez un zoom avant/arrière sur le contenu à l’aide des options de zoom prédéfinies.

* Affichez le contenu sur l’ordinateur de bureau, mobile ou texte unique/texte brut.

   * Cliquez sur l’icône de vue en direct (oeil) pour prévisualiser le contenu sur plusieurs appareils.

   * Sélectionnez l’un des appareils prêts à l’emploi ou saisissez des dimensions personnalisées pour prévisualiser votre contenu.

### Plus d’options {#more-options}

À partir des options **Plus** de l’éditeur de contenu, vous pouvez effectuer les actions suivantes :

CAPTURE D’ÉCRAN

* **Réinitialiser le modèle** : sélectionnez cette option pour effacer le canevas visuel du concepteur d’email sur une barre d’outils vide et redémarrer la création de contenu.

* **Modifiez votre conception** : revenez à la page _Concevez votre modèle_. À partir de là, vous pouvez effectuer toute action comme indiqué dans la section [Concevoir votre modèle](#design-your-template) .

* **Exporter l’HTML** : téléchargez le contenu du canevas visuel vers votre système local au format d’HTML compressé en tant que fichier zip.

## Afficher les détails du modèle {#view-template-details}

Sur la page de liste _Modèles d&#39;email_, cliquez sur le nom d&#39;un modèle d&#39;email pour afficher ses détails.

CAPTURE D’ÉCRAN

Les détails de base tels que le nom et la description peuvent être modifiés. Cliquez en dehors du champ que vous avez modifié pour enregistrer vos modifications.

Cliquez sur **Plus** pour supprimer ou dupliquer rapidement votre modèle.

Si des alertes sont actives (erreurs/avertissements pour le modèle d&#39;email), cliquez sur Alertes pour afficher les informations.

>[!NOTE]
>
>Bien que ces alertes n’interdisent pas l’utilisation du modèle d’email pour la création d’un email, les informations fournissent une visibilité sur ce qui pourrait ne pas fonctionner et les mises à jour requises avant que l’email puisse être utilisé pour la diffusion.

## Affichage des références utilisées par le modèle de courrier électronique {#email-template-used-by-references}

Dans la synthèse du modèle d&#39;email, cliquez sur l&#39;onglet **Utilisé par** pour afficher les détails sur l&#39;emplacement d&#39;utilisation de ce modèle d&#39;email dans Marketo Engage.

CAPTURE D’ÉCRAN

## Modifier des modèles de courrier électronique {#edit-email-templates}

Cette action peut être réalisée à partir des éléments suivants :

* Onglet Détails - Cliquez sur **Modifier le modèle d&#39;email**.

* La page de liste _Modèles d’email_ - Cliquez sur l’icône Autres actions (trois points) du modèle d’email souhaité, puis sélectionnez Modifier.

```
THE SECOND ONE DOESN'T WORK IN MARKETO?? JUST LISTS DUPE AND DELETE - CONFIRMED WITH NILESH - KG
```

Cette action vous conduit à la page _Concevoir votre modèle_ ou à la page de l’éditeur de contenu visuel en fonction du dernier état enregistré du modèle d’email. À partir de là, vous pouvez modifier le contenu de votre modèle d’email selon vos besoins. Voir Création de modèles d’email pour plus d’informations sur les options d’édition.

## Dupliquer des modèles d&#39;email {#duplicate-email-templates}

Il existe deux manières de dupliquer un modèle d&#39;email :

* Dans les détails du modèle d&#39;email sur la droite, cliquez sur **Plus** et sélectionnez **Dupliquer**.

CAPTURE D’ÉCRAN

* Sur la page de liste _Modèles d&#39;email_, cliquez sur l&#39;icône Autres actions (trois points) du modèle d&#39;email souhaité et sélectionnez **Dupliquer**.

Dans la boîte de dialogue, saisissez un nom unique et une description facultative. Cliquez sur **Dupliquer** une fois terminé.

Le modèle d&#39;email dupliqué apparaît ensuite dans la page de liste _Modèles d&#39;email_.

## Supprimer des modèles de courrier électronique {#delete-email-templates}

Il existe deux manières de supprimer un modèle d’email.

>[!CAUTION]
>
>La suppression d’un modèle d’email est irréversible.

* Dans les détails du modèle d&#39;email sur la droite, cliquez sur **Plus** et sélectionnez **Supprimer**.

CAPTURE D’ÉCRAN

* Sur la page de liste _Modèles d&#39;email_, cliquez sur l&#39;icône Autres actions (trois points) du modèle d&#39;email souhaité et choisissez **Supprimer**.

## Actions en masse {#bulk-actions}

Sur la page de liste _Modèles d&#39;email_, sélectionnez plusieurs modèles en cochant les cases à gauche. Une bannière s’affiche en bas.

**Supprimer** : vous pouvez supprimer un maximum de 20 modèles à la fois. Une boîte de dialogue de confirmation vous permet d’annuler l’action ou de confirmer la suppression.

>[!MORELIKETHIS]
>
>[Création d’emails](/help/marketo/product-docs/email-marketing/general/beta-new-email-designer/email-authoring.md){target="_blank"} : découvrez comment créer, concevoir et référencer un email dans le nouveau concepteur.
