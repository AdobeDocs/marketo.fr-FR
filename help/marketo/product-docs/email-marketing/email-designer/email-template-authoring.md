---
description: Modèles d’e-mail - Documents Marketo - Documentation du produit
title: Modèles d’e-mail
hide: true
hidefromtoc: true
feature: Email Editor
exl-id: 92af4ba4-f214-423c-ab2d-ade07b368797
source-git-commit: f6a8f9ec79240a10549adb12ca8b1b4124f683a3
workflow-type: tm+mt
source-wordcount: '1842'
ht-degree: 4%

---

# Modèles d’e-mail {#email-templates}

Pour accélérer et améliorer le processus de conception, vous pouvez créer des modèles d’e-mail autonomes pour réutiliser facilement du contenu personnalisé.

>[!PREREQUISITES]
>
>Pour accéder au nouveau concepteur d’e-mail, votre abonnement de Marketo Engage doit être migré vers le système IMS (Adobe Identity Management System) [](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview). Si le vôtre n’a pas encore été envoyé et que vous souhaitez qu’il soit traité rapidement, veuillez contacter l’équipe du compte d’Adobe (votre gestionnaire de compte) ou l’assistance de [Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

>[!NOTE]
>
>Les modèles d’e-mail du nouveau concepteur d’e-mail ne peuvent être utilisés que pour créer des e-mails dans le nouveau concepteur d’e-mail. Elles ne peuvent pas être référencées dans l’ancien éditeur d’e-mail.

## Création d’un modèle d’e-mail {#create-an-email-template}

1. Connectez-vous à Marketo Engage via [Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"}.

1. Dans Mon Marketo, sélectionnez **Design Studio**.

   ![](assets/create-an-email-template-1.png)

1. Dans l&#39;arborescence, sélectionnez **Modèles d&#39;email (nouvel éditeur)**.

   ![](assets/create-an-email-template-2.png)

1. Cliquez sur le bouton **Créer un modèle**.

   ![](assets/create-an-email-template-3.png)

1. Saisissez un nom de modèle et une description facultative. Cliquez sur **Créer**.

   ![](assets/create-an-email-template-4.png)

## Concevoir votre modèle {#design-your-template}

Sur la page _Concevoir votre modèle_, vous pouvez choisir parmi plusieurs options. [Concevoir en partant de zéro](#design-from-scratch), [importer votre propre HTML ](#import-html) ou [sélectionner un modèle existant](#choose-a-template) (l’un de nos exemples ou celui que vous avez déjà enregistré).

![](assets/design-your-template-1.png)

### Créer en partant de zéro {#design-from-scratch}

Définissez votre contenu en ajoutant et en déplaçant des éléments structurels à l’aide de simples actions de glisser-déposer.

1. Sur la page _Concevoir votre modèle_, sélectionnez **Créer en partant de zéro**.

1. Ajoutez [structure et contenu](#add-structure-and-content).

### Importer votre HTML {#import-your-html}

Vous pouvez importer du contenu d’HTML existant pour concevoir vos modèles d’e-mail. Le contenu peut être :

* Fichier HTML avec feuille de style incorporée

* Un fichier .zip qui comprend un fichier HTML, la feuille de style (.css) et les images

>[!NOTE]
>
>Il n’existe aucune contrainte sur la structure des fichiers .zip. Cependant, les références doivent être relatives et s’ajuster à l’arborescence du dossier .zip.

1. Sur la page _Concevoir votre modèle_, sélectionnez **Importer l’HTML**.

1. Faites glisser et déposez le fichier .zip ou d’HTML souhaité (ou sélectionnez un fichier sur votre ordinateur), puis cliquez sur **Importer**.

   ![](assets/import-your-html-1.png)

   >[!NOTE]
   >
   >Lorsque le contenu de l’HTML est chargé, votre contenu se trouve en mode de compatibilité. Dans ce mode, vous pouvez uniquement personnaliser votre texte, ajouter des liens ou ajouter des ressources à votre contenu.

1. Pour tirer parti des composants de contenu Designer d’e-mail, cliquez sur l’onglet **Convertisseur d’HTML** puis sur **Convertir**.

   >[!CAUTION]
   >
   >L’utilisation d’une balise `<table>` comme première couche d’un fichier HTML peut entraîner une perte de style, y compris les paramètres d’arrière-plan et de largeur dans la balise de couche supérieure.

Vous pouvez désormais personnaliser le fichier importé selon vos besoins à l’aide de l’éditeur visuel d’e-mail.

### Choisir un modèle {#choose-a-template}

Vous avez le choix entre deux types de modèles.

* **Exemples de modèles** : Marketo Engage propose quatre modèles d’e-mail prêts à l’emploi.

* **Modèles enregistrés** : il s’agit de modèles que vous avez créés à partir de zéro à l’aide du menu Modèles , ou d’un e-mail que vous avez créé et que vous avez choisi d’enregistrer en tant que modèle.

>[!BEGINTABS]

>[!TAB Exemples de modèles]

Choisissez l’un des modèles prêts à l’emploi pour prendre un bon départ dans la conception de votre modèle d’e-mail.

1. L’onglet Exemples de modèles est ouvert par défaut.

1. Sélectionnez le modèle que vous souhaitez utiliser.

   ![](assets/sample-templates-1.png)

1. Cliquez sur **Utiliser ce modèle**.

   ![](assets/sample-templates-2.png)

1. Modifiez le contenu selon vos besoins à l’aide du concepteur de contenu visuel.

>[!TAB Modèles enregistrés]

1. Cliquez sur l’onglet **Modèles enregistrés** et sélectionnez le modèle souhaité.

   ![](assets/saved-templates-1.png)

1. Cliquez sur **Utiliser ce modèle**.

   ![](assets/saved-templates-2.png)

1. Modifiez le contenu selon vos besoins à l’aide du concepteur de contenu visuel.

>[!ENDTABS]

## Ajouter la structure et le contenu {#add-structure-and-content}

1. Pour commencer à créer ou modifier du contenu, faites glisser et déposez un élément de Structures sur la zone de travail. Modifiez ses paramètres dans le volet de droite.

   >[!TIP]
   >
   >Sélectionnez le composant n:n colonne pour définir le nombre de colonnes de votre choix (entre trois et 10). Vous pouvez également définir la largeur de chaque colonne en déplaçant les flèches situées sous celle-ci.

   ![](assets/add-structure-and-content-1.png)

   >[!NOTE]
   >
   >La taille de chaque colonne ne peut pas être inférieure à 10 % de la largeur totale du composant de structure. Seules les colonnes vides peuvent être supprimées.

1. Dans la section Contenu , faites glisser les éléments de votre choix et déposez-les dans un ou plusieurs composants de structure.

   ![](assets/add-structure-and-content-2.png)

1. Chaque composant peut être personnalisé via les onglets Paramètres ou Style . Modifiez la police, le style de texte, la marge, etc.

### Ajouter des fragments {#add-fragments}

1. Pour accéder à vos fragments, sélectionnez l’icône _Fragments_ ( ![icône Fragments](assets/icon-fragments.svg) ) dans le volet de navigation de gauche.

   ![Sélectionner un fragment](assets/add-fragments-1.png){width="700" zoomable="yes"}

1. Faites glisser et déposez l’un des fragments dans l’espace réservé du composant structurel.

L’éditeur effectue le rendu du fragment dans la section/l’élément de la structure de l’e-mail. Le contenu du fragment est mis à jour dynamiquement dans la structure pour afficher le contenu tel qu’il apparaît dans l’e-mail.

>[!TIP]
>
>Si vous souhaitez que le fragment occupe toute la disposition horizontale de l’e-mail, ajoutez une structure de colonnes 1:1, puis faites-y glisser le fragment et déposez-le.

Une fois l’e-mail enregistré, il apparaît dans l’onglet _[!UICONTROL Utilisé par]_ de la page des détails du fragment. Les fragments ajoutés à un modèle d’e-mail ne sont pas modifiables dans le modèle ; le fragment source définit le contenu.

### Ajout d’Assets {#add-assets}

Ajoutez les images stockées dans la section [Images et fichiers](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md){target="_blank"} de votre instance de Marketo Engage.

>[!NOTE]
>
>Vous pouvez uniquement ajouter des images dans le nouveau concepteur, mais aucun autre type de fichier pour le moment.

1. Pour accéder à vos images, cliquez sur l’icône Sélecteur de ressources .

   ![](assets/add-assets-1.png)

1. Faites glisser et déposez l’image souhaitée dans un composant de structure.

   ![](assets/add-assets-2.png)

   >[!NOTE]
   >
   >Pour remplacer une image existante, sélectionnez-la, puis cliquez sur **Sélectionner une ressource** dans l’onglet Paramètres à droite.

### Calques, paramètres et styles {#layers-settings-styles}

Ouvrez l’arborescence de navigation pour accéder à des structures spécifiques et à leurs colonnes/composants en vue d’une modification plus granulaire. Pour y accéder, cliquez sur l’icône Arborescence de navigation .

![](assets/layers-settings-styles-1.png)

L’exemple ci-dessous décrit les étapes à suivre pour ajuster la marge intérieure et l’alignement vertical à l’intérieur d’un composant de structure composé de colonnes.

1. Sélectionnez la colonne dans le composant de structure directement dans la zone de travail ou à l’aide de l’_arborescence de navigation_ affichée à gauche.

1. Dans la barre d’outils Colonne, cliquez sur l’outil _[!UICONTROL Sélectionner une colonne]_ et choisissez celle à modifier.

   Vous pouvez également le sélectionner dans l’arborescence de la structure. Les paramètres modifiables de cette colonne sont affichés dans les onglets _[!UICONTROL Paramètres]_ et _[!UICONTROL Styles]_ sur la droite.

   ![](assets/layers-settings-styles-2.png)

1. Pour modifier les propriétés de la colonne, cliquez sur l’onglet _[!UICONTROL Styles]_ à droite et modifiez-les selon vos besoins :

   * Pour **[!UICONTROL Arrière-plan]**, modifiez la couleur d’arrière-plan si nécessaire.

     Décochez la case pour un arrière-plan transparent. Activez le paramètre **[!UICONTROL Image d’arrière-plan]** pour utiliser une image comme arrière-plan au lieu d’une couleur unie.

   * Pour **[!UICONTROL Alignement]**, sélectionnez l’icône _Haut_, _Milieu_ ou _Bas_.
   * Pour **[!UICONTROL Marge intérieure]**, définissez la marge intérieure pour tous les côtés.

     Sélectionnez **[!UICONTROL Marge intérieure différente pour chaque côté]** si vous souhaitez ajuster la marge intérieure. Cliquez sur l’icône _Verrouiller_ pour interrompre la synchronisation.

   * Développez la section **[!UICONTROL Avancé]** pour définir les styles intégrés de la colonne.

   ![](assets/layers-settings-styles-3.png)

1. Répétez ces étapes selon les besoins pour ajuster l’alignement et la marge intérieure des autres colonnes du composant.

1. Enregistrez vos modifications.

### Personnaliser le contenu {#personalize-content}

Les jetons fonctionnent dans le nouvel éditeur de la même manière que dans l’ancien, mais l’icône a un aspect différent. L’exemple ci-dessous décrit l’ajout d’un jeton de prénom avec un texte de remplacement.

1. Sélectionnez le composant de texte. Placez le curseur à l’endroit où vous souhaitez que le jeton apparaisse, puis cliquez sur l’icône **Ajouter une personnalisation**.

   ![](assets/personalize-content-1.png)

1. Cliquez sur le [type de jeton](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} souhaité.

   ![](assets/personalize-content-2.png)

1. Recherchez le jeton souhaité et cliquez sur l’icône **...** (cliquer sur l’icône + ajoute un jeton sans texte de remplacement).

   ![](assets/personalize-content-3.png)

   >[!NOTE]
   >
   >« Texte de remplacement » est le nouveau terme de l’éditeur pour la valeur par défaut. Exemple : ``{{lead.First Name:default=Friend}}``. Il est recommandé au cas où il n’y aurait aucune valeur pour la personne dans le champ que vous choisissez.

1. Définissez le texte de remplacement, puis cliquez sur **Ajouter**.

   ![](assets/personalize-content-4.png)

1. Cliquez sur **Enregistrer**.

### Modifier le tracking des URL {#edit-url-tracking}

Il arrive que vous ne souhaitiez pas activer l’URL de tracking Marketo sur un lien d’un e-mail. Cela s’avère utile lorsque la page de destination ne prend pas en charge les paramètres d’URL et peut entraîner la rupture d’un lien.

1. Cliquez sur l’icône Liens pour afficher toutes les URL de votre e-mail.

   ![](assets/edit-url-tracking-1.png)

1. Cliquez sur l’icône en forme de crayon pour modifier le suivi de tous les liens souhaités.

1. Cliquez sur la liste déroulante **Type de tracking** et effectuez votre sélection.

   ![](assets/edit-url-tracking-2.png)

   <table><tbody>
     <tr>
       <td><b>Suivi sans mkt_tok</b></td>
       <td>Active le tracking sur l’URL sans utiliser le paramètre de chaîne de requête mkt_tok dans l’URL de destination</td>
     </tr>
     <tr>
       <td><b>Suivi avec mkt_tok</b></td>
       <td>Active le tracking sur l’URL avec utilisation du paramètre de chaîne de requête mkt_tok dans l’URL de destination</td>
     </tr>
     <tr>
       <td><b>Ne pas suivre</b></td>
       <td>Désactive le tracking de l'URL</td>
     </tr>
   </tbody>
   </table>

1. Vous pouvez éventuellement attribuer un libellé à l’URL ou ajouter des balises.

1. Cliquez sur **Enregistrer** lorsque vous avez terminé.

### Afficher les options {#view-options}

Tirez parti des options d’affichage et de validation du contenu disponibles dans l’éditeur visuel d’e-mail.

* Effectuez un zoom avant/arrière sur le contenu à l’aide des options de zoom prédéfinies.

* Affichez le contenu sur les appareils de bureau, mobiles ou en texte seul/texte brut.

   * Cliquez sur l’icône Affichage dynamique (œil) pour afficher un aperçu du contenu sur tous les appareils.

   * Sélectionnez l’un des appareils prêts à l’emploi ou saisissez des dimensions personnalisées pour prévisualiser votre contenu.

### Plus d’options {#more-options}

À partir des options **Plus** de l’éditeur de contenu, vous pouvez effectuer les actions suivantes :

![](assets/more-options-1.png)

* **Réinitialiser le modèle** : sélectionnez cette option pour vider la zone de travail du concepteur d’e-mail visuel et redémarrer la création de contenu.

* **Modifier votre conception** : revenez à la page _Concevoir votre modèle_. À partir de là, vous pouvez effectuer n’importe quelle action comme indiqué dans la section [Concevoir votre modèle](#design-your-template).

* **Exporter l’HTML** : téléchargez le contenu de la zone de travail visuelle sur votre système local au format HTML compressé sous la forme d’un fichier zip.

## Affichage des détails du modèle {#view-template-details}

Dans la page de liste _Modèles d’e-mail_, cliquez sur le nom d’un modèle d’e-mail pour en afficher les détails.

(assets/view-template-details-1.png

Les détails de base tels que le nom et la description peuvent être modifiés. Cliquez en dehors du champ que vous avez modifié pour enregistrer vos modifications.

Cliquez sur **Plus** pour supprimer ou dupliquer rapidement votre modèle.

S’il existe des alertes actives (erreurs/avertissements pour le modèle d’e-mail), cliquez sur Alertes pour afficher les informations.

>[!NOTE]
>
>Bien que ces alertes n’interdisent pas l’utilisation du modèle d’e-mail pour la création d’e-mails, les informations fournissent une visibilité sur ce qui peut ne pas fonctionner et sur les mises à jour requises avant que l’e-mail ne puisse être utilisé pour la diffusion.

## Afficher le modèle d’e-mail utilisé par les références {#email-template-used-by-references}

Dans le résumé du modèle d’e-mail, cliquez sur l’onglet **Utilisé par** pour afficher les détails sur l’utilisation de ce modèle d’e-mail dans Marketo Engage.

![](assets/email-template-used-by-references-1.png)

## Modifier les modèles d’e-mail {#edit-email-templates}

Cette action peut être effectuée à partir de :

* Onglet Détails - Cliquez sur **Modifier le modèle d’e-mail**.

Cette action vous conduit à la page _Concevoir votre modèle_ ou à la page de l’éditeur de contenu visuel en fonction du dernier statut enregistré du modèle d’e-mail. À partir de là, vous pouvez modifier le contenu de votre modèle d’e-mail selon vos besoins. Voir Création de modèles d’e-mail pour plus d’informations sur les options de modification.

## Dupliquer les modèles d’e-mail {#duplicate-email-templates}

Il existe deux manières de dupliquer un modèle d’e-mail :

* Dans les détails du modèle d’e-mail sur la droite, cliquez sur **Plus** et sélectionnez **Dupliquer**.

  ![](assets/duplicate-email-templates-1.png)

* Sur la page de liste _Modèles d’e-mail_, cliquez sur l’icône Plus d’actions (points de suspension) du modèle d’e-mail souhaité, puis sélectionnez **Dupliquer**.

Dans la boîte de dialogue, saisissez un nom unique et une description facultative. Cliquez sur **Dupliquer** lorsque vous avez terminé.

Le modèle d’e-mail dupliqué apparaît alors dans la page de liste _Modèles d’e-mail_.

## Supprimer les modèles d’e-mail {#delete-email-templates}

Vous pouvez supprimer un modèle d’e-mail de deux façons.

>[!CAUTION]
>
>La suppression d’un modèle d’e-mail est irréversible.

* Dans les détails du modèle d’e-mail sur la droite, cliquez sur **Plus** et sélectionnez **Supprimer**.

  ![](assets/delete-email-templates-1.png)

* Sur la page de liste _Modèles d’e-mail_, cliquez sur l’icône Plus d’actions (points de suspension) du modèle d’e-mail souhaité, puis choisissez **Supprimer**.

## Actions en masse {#bulk-actions}

Sur la page de liste _Modèles d’e-mail_, sélectionnez plusieurs modèles en cochant les cases situées à gauche. Une bannière s’affiche en bas.

**Supprimer** : vous pouvez supprimer un maximum de 20 modèles à la fois. Une boîte de dialogue de confirmation vous permet d’abandonner l’action ou de confirmer la suppression.

>[!MORELIKETHIS]
>
>[Création d’e-mail](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md){target="_blank"} : découvrez comment créer, concevoir et référencer un e-mail dans le nouveau concepteur.
