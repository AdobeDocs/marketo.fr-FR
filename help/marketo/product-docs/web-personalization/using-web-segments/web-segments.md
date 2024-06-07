---
unique-page-id: 4719093
description: Segments web - Documents Marketo - Documentation du produit
title: Segments web
exl-id: ec62c1ae-579a-4753-9b2d-18c7c2fa1ff5
feature: Web Personalization
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '2051'
ht-degree: 5%

---

# Segments web {#web-segments}

## Afficher le segment {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

L’onglet Segments affiche tous les segments définis personnalisés que vous configurez en fonction de divers attributs.  **Un segment est un ensemble de visiteurs qui répondent aux critères spécifiés définis dans la page &quot;Définir un segment&quot;.**  Un segment peut être des visiteurs provenant d’un secteur industriel, d’un emplacement ou d’une activité sur site spécifique.

Dans la personnalisation web, un visiteur peut correspondre à plusieurs segments. Par exemple, s’il existe un segment pour les visiteurs E.U. et un segment pour les sociétés financières, un visiteur web de Bank of America correspondra à **both** le segment pour les visiteurs aux États-Unis et le segment pour les sociétés financières.

**GRAPHIQUE :**  La page Segments affiche un graphique à barres des segments sélectionnés en fonction du nombre de visiteurs provenant du segment (axe y) et du nom du segment (axe x).

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Nom</th> 
   <th colspan="1" rowspan="1">Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Nom</strong></td> 
   <td colspan="1" rowspan="1">Titre du segment</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Correspond</strong></p></td> 
   <td colspan="1" rowspan="1">Nombre de visiteurs répondant aux critères personnalisés et définis du segment.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Définir la campagne</strong></td> 
   <td colspan="1" rowspan="1">Permet de configurer une CTA de campagne associée au terme de recherche sélectionné.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Visiteurs</strong></td> 
   <td colspan="1">Aperçu de la table des visiteurs associée au terme de recherche sélectionné</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Parcours de visites</strong></td> 
   <td colspan="1" rowspan="1">Affiche un tableau de l’activité et du chemin d’URL du visiteur sur le site, ainsi que la durée de visite de chaque page. </td> 
  </tr> 
 </tbody> 
</table>

Voir [comment créer et afficher des libellés de segment](/help/marketo/product-docs/web-personalization/using-web-segments/label-your-segment.md)

**Segments - Panneau de droite**

![](assets/image2014-11-12-10-3a46-3a32.png)

La sélection d’un segment dans le tableau affiche des détails supplémentaires sur le segment dans le panneau de droite.

Ces détails incluent :

* Nom du segment
* Date de création du segment
* Les campagnes associées affichant les campagnes qui opèrent avec le segment. Cliquez sur le nombre de réactions pour accéder à la page des campagnes qui affiche l’CTA (Appel à l’action) de la campagne pour le segment.
* Le nombre de correspondances (nombre de visiteurs qui ont rempli les critères du segment) pour le segment et le nombre de visiteurs distincts (uniques) qui ont correspondu au segment. Cliquez sur le lien du visiteur unique pour accéder à la page du visiteur affichant les résultats du segment.
* Créateur propriétaire/utilisateur du segment
* Les sites de domaine associés au segment
* Résumé court des critères sélectionnés du segment

## Activation ou désactivation d’un segment {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

Pour activer ou désactiver un segment, cochez la case correspondant à ce segment dans le tableau et, dans la liste déroulante &quot;Choisir une action&quot; au bas du tableau, sélectionnez l’action &quot;Activer&quot; ou &quot;Désactiver&quot;. Lorsqu’un segment est désactivé, le mot &quot;désactiver&quot; s’affiche sous la colonne État.

## Création de segments {#create-segments}

Le segment que vous créez répond aux critères spécifiques que vous définissez dans la variable **Définir un segment** page. Vous pouvez également personnaliser vos segments en fonction d’une combinaison de critères, ciblant une audience spécifique dans votre campagne.

Pour créer un segment

Dans la **Segments** page, cliquez sur **Créer** sous le graphique. L’écran suivant s’affiche.

![](assets/four.png)

Définissez les paramètres généraux de votre segment :

* **Nom :**  Nommez votre segment.
* **Description :**  Fournissez une explication plus détaillée des critères de segment.
* **Domaines :**  Sélectionnez le ou les domaines que vous souhaitez inclure dans le segment.
* **Logique de règle de segment :**  Sélectionnez une logique ET/OU pour créer chaque attribut de segmentation.
* **Minutage :** Définition du niveau d’engagement des visiteurs souhaité dans votre campagne

   * **À l’entrée**: l’engagement du visiteur arrive sur le site web.
   * **Après le 1er au 9e clic**: engage le visiteur après un nombre spécifique de clics sur le site web

>[!TIP]
>
>**Logique de règle de segment**
>
>Il existe trois options de filtre :
>
>1. Utiliser tous les filtres (1, 2 et 3...)
>1. Utiliser n’importe quel filtre (1, 2 ou 3...)
>1. Filtres avancés (à l’aide des expressions et / ou )
>
>    Les filtres avancés vous permettent de contrôler la condition du segment. Saisir les numéros de filtres séparés par « et » et « ou ».
>
>    * 1 et 2 et 3
>    * 1 ou 2 ou 3
>
>    Le mélange de « et » et « ou » nécessite des parenthèses pour clarifier la logique d’intention. Par exemple, « 1 ou 2 et 3 » doit être écrit d’une des façons suivantes :
>
>    * 1 et (2 ou 3)
>    * (1 et 2) ou 3
>
>    Les parenthèses imbriquées sont acceptées pour les logiques plus complexes, par exemple
>
>    * (1 et 2) ou (3 et 4)
>    * 1 et (2 ou (3 et 4))
>
>    Vérifiez votre logique après toute insertion, suppression ou réorganisation.

Faites glisser les attributs de segment de la colonne de droite vers l’éditeur de segments sur le côté gauche :

![](assets/five.png)

### Données firmographiques {#firmographics}

**Emplacement**

Glisser-déposer **Emplacement** dans l’éditeur de segments.

* Sélectionnez l’un des paramètres suivants :

   * **Inclure** - Indiquez si vous souhaitez que la campagne inclut ou exclue un emplacement.
   * **Sélectionner le pays à ajouter** - Dans la liste déroulante, sélectionnez le pays que vous souhaitez inclure dans le segment. Le nom du pays s’affiche à droite. Vous pouvez choisir plusieurs pays.

Une fois le pays ajouté, vous pouvez également spécifier l’état, la ville et le code postal du segment.

* **Sélectionnez Etat ou Province à ajouter.** - Dans la liste déroulante, sélectionnez l’État des États-Unis ou la Province canadienne que vous souhaitez inclure. Vous pouvez effectuer plusieurs sélections.
* **Code postal** - Entrez le code postal que vous souhaitez inclure dans votre segment.
* **Villes** - Renseignez la ou les villes que vous souhaitez inclure. Utilisez un point-virgule entre les villes.

>[!TIP]
>
>**Quelles conditions de segment dois-je choisir ? &quot;ET&quot; ou &quot;OU&quot; ?** OU fonctionne comme une option supplémentaire dans chaque champ. Les prospects n’ont besoin de remplir qu’un seul critère parmi les multiples critères sélectionnés dans chaque champ pour être éligibles au segment. (Par exemple, les prospects peuvent provenir soit des États-Unis, *ou* de l&#39;industrie de la Défense). ET fonctionne comme un paramètre obligatoire supplémentaire qui doit être rempli pour ce segment. (Par exemple, les perspectives doivent venir à la fois des États-Unis et de l&#39;industrie de la Défense). Dans chaque profil de segmentation, chaque champ distinct peut fonctionner comme les deux, soit comme &quot;AND&quot;, soit comme &quot;OR&quot; selon la condition de segment sélectionnée.

**Industries** Sous , **Segmentation des profils** , cochez la case en regard de **Secteur industriel**.

* Sélectionnez l’un des paramètres suivants :

   * **Inclut** - Indiquez si vous souhaitez que le segment inclut ou exclue un secteur d’activité.
   * **Sélectionner les secteurs à ajouter** - Sélectionnez le secteur que vous souhaitez inclure dans le segment. Le secteur apparaît sous la liste déroulante. Vous pouvez choisir plusieurs secteurs d’activité.

**Groupe d’organisations**

Sous , **Segmentation des profils** , cochez la case en regard de **Groupe d’organisations.**

* Dans la liste déroulante, sélectionnez l’une des options suivantes :

   * Fortune 500 - Inclut uniquement les entreprises Fortune 500 dans ce segment
   * Fortune 1000 - Inclut uniquement les entreprises Fortune 1000 dans ce segment
   * Global 2000 - Inclut les 2 000 entreprises mondiales dans ce segment
   * Entreprise : comprend les entreprises de plus de 1 000 employés et dont les recettes sont supérieures à 250 millions de dollars.
   * PME - Inclut uniquement les petites et moyennes entreprises dans ce segment

**-Comptes nommés**

**Organisations**

* **provient de ces sociétés (noms spécifiques) ;**

   * Sélectionnez la société à cibler dans la liste déroulante &quot;Sélectionner la société à ajouter&quot;.
   * Vous pouvez saisir le nom exact de l’organisation à cibler. *C’est _always_ Il est recommandé d’utiliser des listes de comptes nommés au lieu de saisir les noms manuellement pour obtenir de meilleures correspondances (voir ci-dessous).

**Liste des comptes nommés**

Effectuez une sélection depuis un [Liste des comptes nommés](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md) pour segmenter les comptes ciblés clés.

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>Le nombre entre crochets en regard du nom Liste des comptes nommés est utilisé comme référence d’index pour la liste de personnalisation web. [API de lecture](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/web-personalization).

**Exclure le FAI**

Exclut les fournisseurs de services Internet (FAI) du segment.

### Personnes connues {#known-people}

**Base**

La personnalisation web s’intègre à votre base de données Marketo, ce qui vous permet de segmenter et de personnaliser les campagnes en fonction d’attributs et de données de personnes connues.

Sélectionnez Base de données et sélectionnez un champ de données de personne dans la liste déroulante. Sélectionnez la variable **+** pour ajouter des champs dans la liste déroulante.

![](assets/seven.png)

Vous pouvez ajouter ou supprimer des champs de données de personne dans Paramètres du compte > Base de données.

>[!TIP]
>
>Créez vos critères de segment en fonction de tous les champs de données de personnes de Marketo tels que le titre de la tâche, la note, le rôle, etc.
>
>Par exemple, &quot;Titre de la tâche = CMO&quot; et &quot;Le score est inférieur ou égal à 50&quot;

**Marketo Email Campaign** Segmentez et personnalisez des campagnes à l’aide du renvoi d’un courrier électronique par un visiteur qui clique sur un courrier électronique Marketo et arrive sur le site. Segmenter par nom de programme ou nom de campagne Marketo et poursuivre la conversation du courrier électronique au web. Sélectionnez le + pour ajouter des champs dans la liste déroulante.

![](assets/image2015-5-27-17-3a20-3a34.png)

**État**

Définissez votre segment en fonction du statut d’un prospect : connu ou anonyme.

* Connu : sélectionnez cette option dans la liste déroulante pour les visiteurs connus. Un visiteur est connu lorsqu’il envoie un formulaire sur votre site Web et apparaît sur la page Personnes de personnalisation Web.
* Anonyme : sélectionnez cette option dans la liste déroulante pour les visiteurs anonymes.

![](assets/image2015-5-27-17-3a23-3a2.png)

### Comportemental {#behavioral}

**Visites -** Définissez votre segment en fonction du comportement ou de l’identification du visiteur.

* Nombre de visites : sélectionnez cette option dans la liste déroulante pour indiquer le nombre de visites des prospects sur le site web.

   * Dans la liste déroulante, sélectionnez Equals (Est égal à) ou Greater Than (Est égal à) ou Less Than (Est inférieur à).

* Visites spécifiques : sélectionnez cette option dans la liste déroulante pour spécifier un visiteur spécifique.

   * Dans la zone de texte à droite, saisissez le nombre de visiteurs dont vous souhaitez effectuer le suivi. Le numéro d’identification unique des visiteurs de la personnalisation Web se trouve lorsque vous cliquez sur un visiteur (dans la page des visiteurs) et sur Définir la campagne dans le panneau de droite. L’identifiant visiteur se trouve dans la section Paramètres avancés . L’identifiant visiteur se trouve également dans l’URL (par exemple, VISITOR=JZZJIFJNUI60PZ8Y97BHTY9BL8PKWS).

**Termes de recherche** - Définissez un segment en fonction des termes de recherche d’un prospect.

* Le visiteur a recherché : dans la liste déroulante, sélectionnez les termes dont vous souhaitez effectuer le suivi dans votre recherche de visiteurs ou ajoutez vos propres termes de recherche. (Il n’est pas nécessaire que la variable &#42; caractère générique sur les termes de recherche, dans la mesure où il est défini par défaut pour inclure les expressions qui contiennent le terme de recherche).

**Références** - Ajoutez des URL auxquelles le visiteur a été référencé.

* Sélectionner les références à ajouter : dans la liste déroulante, sélectionnez les sites de référence que vous souhaitez suivre ou ajoutez votre propre référence. Une fois cette option sélectionnée, les références s’affichent dans la zone ci-dessous. (En utilisant &#42; comme caractère générique autorisé)

**Inclure les pages** - Effectuer le suivi des prospects de pages spécifiques visitées sur votre site web.

* Correspondances d’URL : ajoutez l’URL de pages web spécifiques dont vous souhaitez effectuer le suivi. Vous pouvez ajouter plusieurs URL en les séparant par un point-virgule. (En utilisant &#42; comme caractère générique autorisé).

**Exclure des pages** - Excluez les pages spécifiques que vous ne souhaitez pas faire correspondre dans le segment. (En utilisant &#42; comme caractère générique autorisé).

* L’URL ne correspond pas : ajoutez l’URL de pages web spécifiques que vous souhaitez exclure du suivi. Vous pouvez ajouter plusieurs URL en les séparant par un point-virgule.

![](assets/segment-extra.png)

### Appareil / navigateur {#device-browser}

**SE Mobile**

Faites glisser et déposez le SE Mobile dans l’éditeur de segments.

![](assets/image2015-5-27-17-3a45-3a3.png)

* **Type de visiteur**<br />
  **SE Mobile** - Dans la liste déroulante, sélectionnez un ou plusieurs systèmes d’exploitation mobiles répertoriés. Le système d’exploitation mobile sélectionné s’affiche en dessous.

   * Le visiteur utilise n’importe quel appareil mobile.
   * Le visiteur utilise ce périphérique/système d’exploitation spécifique
   * Le visiteur n’utilise aucun appareil mobile.

* **Appareil**  - Dans la liste déroulante, sélectionnez un ou plusieurs appareils (Apple, Samsung, LG, HTC, Nexus, Blackberry, etc.). Les périphériques sélectionnés s’affichent en dessous.

**Navigateur**

Visiteur Target qui utilise des types et/ou versions de navigateur spécifiques.

* Type de navigateur : dans la liste déroulante, sélectionnez un ou plusieurs navigateurs Internet . Les navigateurs sélectionnés s’affichent ci-dessous.
* Version du navigateur : saisissez la version du navigateur que vous souhaitez ajouter au segment. Vous pouvez sélectionner plusieurs versions en les séparant par une virgule. (En utilisant &#42; comme caractère générique autorisé).

### API {#api}

**Événements de données** - Segmenter les visiteurs qui déclenchent des événements de données personnalisées spécifiques

Ajoutez la valeur Event que vous souhaitez cibler. Par exemple, à partir de sources de données tierces.

**API de contexte d’utilisateur**

Appel de l’API de personnalisation web  [pour en savoir plus, cliquez ici .](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/web-personalization)

>[!TIP]
>
>**Utilisation de caractères génériques -** Lorsque vous souhaitez inclure un terme de recherche ou une URL qui contient un élément, c’est-à-dire &quot;[google.com](https://google.com)&quot; ou &quot;produit de terme de recherche&quot;, nous appelons cela un caractère générique et il devrait être saisi avec un astérisque - ce petit gars&#42; - à chaque extrémité. Donc tout vient de [google.com](https://google.com) doit être saisi en tant que &#42; [google.com](https://google.com)&#42;

## Modifier les segments {#edit-segments}

Vous pouvez modifier un segment qui a été créé.

1. Pour modifier un segment, accédez à **Segments**.

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. Dans le **Segments** , cliquez sur l’icône d’édition ( ![](assets/segment-edit.png)) du segment que vous souhaitez modifier. La variable **Définir un segment** s’ouvre avec le segment sélectionné.
1. Appliquez les modifications que vous souhaitez apporter au segment.
1. Cliquez sur **Enregistrer**.

## Suppression de segments {#delete-segments}

Vous pouvez supprimer les segments que vous avez créés.

1. Dans la **Segments** Sélectionnez un segment ci-dessus.
1. Cliquez sur l’icône de suppression ( ![](assets/segment-delete.png) ) du segment que vous souhaitez supprimer.
1. Un message de confirmation s’affiche, confirmant que vous êtes sur le point de supprimer la variable **Segment**.

>[!NOTE]
>
Vous ne pouvez pas supprimer un segment associé à une campagne. Vous devez d’abord supprimer la campagne, puis le segment.

Fantastique ! Maintenant que vous comprenez la section Segments , découvrons les campagnes.

>[!MORELIKETHIS]
>
* [Création d’un segment web de base](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)
* [Créer une campagne web de boîte de dialogue](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
* [Créer une campagne web dans la zone](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
* [Créer une campagne web de widgets](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
