---
unique-page-id: 4719093
description: Segments Web - Documents Marketo - Documentation Du Produit
title: Segments Web
exl-id: ec62c1ae-579a-4753-9b2d-18c7c2fa1ff5
feature: Web Personalization
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '2043'
ht-degree: 5%

---

# Segments Web {#web-segments}

## Afficher le segment {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

L’onglet Segments affiche tous les segments personnalisés définis que vous configurez en fonction de divers attributs.  **Un segment est un ensemble de visiteurs qui répondent aux critères spécifiés définis dans la page « Définir un segment ».** Un segment peut être constitué de visiteurs provenant d’un secteur ou d’un emplacement spécifique, ou en fonction de l’activité sur site du visiteur.

Dans [!DNL Web Personalizatio] , un visiteur peut correspondre à plusieurs segments. Par exemple, s’il existe un segment pour les visiteurs des États-Unis et un segment pour les sociétés de financement, un visiteur web de Bank of America correspondrait **à la fois** au segment pour les visiteurs des États-Unis et au segment pour les sociétés de financement.

**GRAPHIQUE :** la page Segments affiche un graphique à barres des segments sélectionnés en fonction du nombre de visiteurs provenant du segment (axe y) et du nom du segment (axe x).

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
   <td colspan="1" rowspan="1"><p><strong>Correspond à</strong></p></td>
   <td colspan="1" rowspan="1">Nombre de visiteurs et visiteuses répondant aux critères personnalisés et définis du segment</td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><strong>Définir la campagne</strong></td>
   <td colspan="1" rowspan="1">Permet de configurer un CTA Campaign associé au terme de recherche sélectionné</td>
  </tr>
  <tr>
   <td colspan="1"><strong>Visiteurs</strong></td>
   <td colspan="1">Un aperçu du tableau des visiteurs associé au terme de recherche sélectionné</td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><strong>Parcours de visites</strong></td>
   <td colspan="1" rowspan="1">Affiche un tableau de l’activité et du chemin d’URL du visiteur sur le site et la durée de sa visite sur chaque page </td>
  </tr>
 </tbody>
</table>

Voir [comment créer et afficher des libellés de segment](/help/marketo/product-docs/web-personalization/using-web-segments/label-your-segment.md)

**Segments - Panneau de droite**

![](assets/image2014-11-12-10-3a46-3a32.png)

Si vous sélectionnez un segment dans le tableau, des détails supplémentaires sur le segment s’affichent dans le panneau de droite.

Ces informations incluent :

* Nom du segment
* Date de création du segment
* Campagnes associées affichant les campagnes fonctionnant avec le segment. Cliquez sur le nombre de réactions pour accéder à la page des campagnes affichant le CTA de campagne (Call to action) pour le segment
* Le nombre de correspondances (nombre de visiteurs et visiteuses qui répondaient aux critères du segment) pour le segment et le nombre de visiteurs et visiteuses distincts (uniques) qui correspondaient au segment. Cliquer sur le lien d’un visiteur ou d’une visiteuse unique vous mène à la page du visiteur ou de la visiteuse affichant les résultats du segment
* Propriétaire/créateur utilisateur du segment
* Sites de domaine associés au segment
* Un bref résumé des critères sélectionnés du segment

## Activation ou désactivation d’un segment {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

Pour activer ou désactiver un segment, cochez la case correspondant à ce segment dans le tableau, puis dans la liste déroulante « [!UICONTROL  Choisir une action ] » au bas du tableau, sélectionnez l’action « [!UICONTROL  Activer ] » ou « [!UICONTROL  Désactiver ]. Lorsqu’un segment est désactivé, le mot « désactiver » s’affiche sous la colonne [!UICONTROL État].

## Création de segments {#create-segments}

Le segment que vous créez répond aux critères spécifiques que vous définissez sur la page **[!UICONTROL Définir le segment]**. Vous pouvez également personnaliser vos segments en fonction d’une combinaison de critères et en ciblant une audience spécifique dans votre campagne.

Pour créer un segment

Sur la page **[!UICONTROL Segments]**, cliquez sur **[!UICONTROL Créer]** sous le graphique. L’écran suivant s’affiche.

![](assets/four.png)

Définissez des paramètres généraux pour votre segment :

* **Nom :** donnez un nom à votre segment.
* **Description :** fournir une explication plus détaillée des critères de segment.
* **Domaines :** permet de sélectionner le ou les domaines à inclure dans le segment.
* **Logique de règle de segment :** sélectionnez une logique AND / OR pour créer chaque attribut de segmentation
* **Planning :** définissez le niveau d’engagement des visiteurs souhaité dans votre campagne.

   * **À l’entrée** : l’engagement du visiteur arrive sur le site web
   * **Après le 1er - 9e clic** : engagez le visiteur après un nombre spécifique de clics sur le site web

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

Faites glisser et déposez Attributs de segment de la colonne de droite vers l’éditeur de segments sur le côté gauche :

![](assets/five.png)

### Données firmographiques {#firmographics}

**Emplacement**

Effectuez un glisser-déposer de **[!UICONTROL Emplacement]** dans l’éditeur de segments.

* Faites votre choix parmi les paramètres suivants :

   * **[!UICONTROL Inclure]** - Indiquez si vous souhaitez que la campagne inclue ou exclue un emplacement.
   * **[!UICONTROL Sélectionner le pays à ajouter]** - Dans la liste déroulante, sélectionnez le pays que vous souhaitez inclure dans le segment. Le nom du pays s’affiche à droite. Vous pouvez choisir plusieurs pays.

Une fois le pays ajouté, vous pouvez également spécifier l’État, la ville et le code postal du segment.

* **[!UICONTROL Sélectionnez l’État ou la province à ajouter]** - Dans la liste déroulante, sélectionnez l’État des États-Unis ou la province canadienne que vous souhaitez inclure. Vous pouvez effectuer plusieurs sélections.
* **[!UICONTROL Code postal]** - Saisissez le code postal que vous souhaitez inclure dans votre segment.
* **[!UICONTROL Villes]** - Saisissez la ou les villes que vous souhaitez inclure. Utilisez un point-virgule entre les villes.

>[!TIP]
>
>**Quelles conditions de segment dois-je choisir ? &#39;AND&#39; ou &#39;OR&#39; ?** OU fonctionne comme une option supplémentaire dans chaque champ. Les prospects n’ont besoin de remplir qu’un seul des critères des différents critères sélectionnés dans chaque champ pour être qualifiés pour le segment. (Par exemple, les prospects peuvent provenir des États-Unis *ou* de l&#39;industrie de la défense). ET fonctionne comme un paramètre obligatoire supplémentaire qui doit être satisfait pour ce segment. (Par exemple, les prospects doivent provenir à la fois des États-Unis et de l&#39;industrie de la défense). Dans chaque profil de segmentation, chaque champ distinct peut fonctionner comme « AND » ou « OR » selon la condition de segment sélectionnée.

**Industries** Dans la section **[!UICONTROL Segmentation de profil]**, cochez la case en regard de **[!UICONTROL Industrie]**.

* Faites votre choix parmi les paramètres suivants :

   * **[!UICONTROL Inclut]** - Indiquez si vous souhaitez que le segment inclue ou exclue un secteur d’activité.
   * **[!UICONTROL Sélectionner les secteurs à ajouter]** - Sélectionnez le secteur que vous souhaitez inclure dans le segment. Le secteur apparaît sous la liste déroulante. Vous pouvez choisir plusieurs secteurs d’activité.

**Groupe d’organisations**

Dans la section **[!UICONTROL Segmentation de profil]**, cochez la case en regard de **[!UICONTROL Groupe d’organisations].**

* Dans la liste déroulante, sélectionnez l’une des options suivantes :

   * Fortune 500 - Inclut uniquement les entreprises Fortune 500 de ce segment
   * Fortune 1000 - Inclut uniquement les entreprises Fortune 1000 de ce segment
   * Global 2000 - Inclut les entreprises Global 2000 de ce segment
   * Entreprise - Inclut les organisations comptant plus de 1 000 employés et dont le chiffre d’affaires dépasse 250 millions de dollars
   * PME - Inclut uniquement les petites et moyennes entreprises de ce segment

**-Named Accounts-**

**Organisations**

* **Provient de ces sociétés (noms spécifiques)**

   * Sélectionnez la société à cibler dans le menu déroulant « Sélectionner la société à ajouter ».
   * Vous pouvez saisir le nom exact de l’organisation que vous souhaitez cibler. *Il est *toujours* recommandé d’utiliser les listes de comptes nommés au lieu de saisir les noms manuellement pour de meilleures correspondances (voir ci-dessous).

**Liste des comptes nommés**

Effectuez une sélection dans une [Liste de comptes nommés](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md) pour segmenter les comptes ciblés clés.

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>Le nombre entre crochets en regard du nom de la liste des comptes nommés est utilisé comme référence d’index pour la liste de Web Personalization [API de lecture](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/web-personalization).

**Exclure le FAI**

Exclut les fournisseurs d’accès Internet (FAI) du segment.

### Personnes connues {#known-people}

**[!UICONTROL Base de données]**

[!DNL Web Personalization] s’intègre à votre base de données Marketo, ce qui vous permet de segmenter et de personnaliser des campagnes selon des attributs et des données de personne connus.

Sélectionnez Base de données , puis sélectionnez un champ de données personne dans la liste déroulante. Sélectionnez **+** pour ajouter des champs dans la liste déroulante.

![](assets/seven.png)

Vous pouvez ajouter ou supprimer des champs de données de personne depuis Paramètres du compte > Base de données

>[!TIP]
>
>Créez vos critères de segment en fonction de tous les champs de données de personne des personnes Marketo, tels que le titre de la fonction, le score, le rôle, etc.
>
>Par exemple, « Titre du poste est égal à CMO » et « Score est inférieur ou égal à 50 »

**[!UICONTROL Campagne par e-mail Marketo]** segmentez et personnalisez les campagnes par référence d’e-mail d’un visiteur qui clique sur un e-mail Marketo et qui arrive sur le site. Segmentez par nom de programme Marketo ou nom de campagne et poursuivez la conversation de l’e-mail au web. Sélectionnez le signe + pour ajouter des champs dans la liste déroulante.

![](assets/image2015-5-27-17-3a20-3a34.png)

**[!UICONTROL Statut]**

Définissez votre segment en fonction du statut d’un prospect : connu ou anonyme.

* Connu - Sélectionnez cette option dans la liste déroulante pour les visiteurs connus. Un visiteur est connu lorsqu’il envoie un formulaire sur votre site web et apparaît sur la page [!DNL Web Personalization] [!UICONTROL Personnes].
* Anonyme - Sélectionnez cette option dans la liste déroulante pour les visiteurs anonymes.

![](assets/image2015-5-27-17-3a23-3a2.png)

### Comportemental {#behavioral}

**[!UICONTROL Visites] -** Définissez votre segment en fonction du comportement ou de l’identification des visiteurs.

* Nombre de visites - Sélectionnez cette option dans la liste déroulante pour spécifier le nombre de visites des prospects du site web.

   * Sélectionnez Est égal à, Est égal à ou Supérieur à, ou Est égal à ou Inférieur à dans la liste déroulante.

* Visites spécifiques - Sélectionnez cette option dans la liste déroulante pour spécifier un visiteur spécifique.

   * Dans la zone de texte de droite, saisissez le nombre de visiteurs que vous souhaitez suivre. Le numéro d’identification unique du visiteur [!DNL Web Personalization] se trouve lorsque vous cliquez sur un visiteur (dans la page des visiteurs) et sur la visionneuse de campagnes dans le panneau latéral droit. L’identifiant visiteur se trouve dans la section Paramètres avancés . L’identifiant visiteur se trouve également dans l’URL (par exemple VISITOR=JZZJIFJNUI60PZ8Y97BHTY9BL8PKWS).

**Termes de recherche** - Définissez un segment en fonction des termes de recherche d’un prospect.

* Le visiteur recherché : dans la liste déroulante, sélectionnez les termes que vous souhaitez suivre dans votre recherche de visiteurs ou ajoutez vos propres termes de recherche. (Le caractère générique &#42; n’est pas nécessaire sur les termes de recherche, car il est défini par défaut pour inclure les expressions qui contiennent le terme de recherche).

**[!UICONTROL Références]** - Ajoutez les URL par lesquelles le visiteur a été référencé.

* Sélectionner les références à ajouter - Dans la liste déroulante, sélectionnez les sites de référence que vous souhaitez suivre ou ajoutez votre propre référence. Une fois sélectionnées, les références apparaîtront dans la zone ci-dessous. (L’utilisation de &#42; comme caractère générique est autorisée)

**[!UICONTROL Inclure des pages]** - Effectuez le suivi de pages spécifiques visitées par les prospects sur votre site web.

* Correspondances d’URL : ajoutez l’URL de pages web spécifiques que vous souhaitez suivre. Vous pouvez ajouter plusieurs URL en les séparant par un point-virgule. (L’utilisation de &#42; comme caractère générique est autorisée).

**[!UICONTROL Exclure des pages]** - Excluez les pages spécifiques que vous ne souhaitez pas faire correspondre dans le segment. (L’utilisation de &#42; comme caractère générique est autorisée).

* L’URL ne correspond pas : ajoutez l’URL de pages web spécifiques que vous souhaitez exclure du suivi. Vous pouvez ajouter plusieurs URL en les séparant par un point-virgule

![](assets/segment-extra.png)

### Appareil / navigateur {#device-browser}

**[!UICONTROL Système d’exploitation mobile]**

Faites glisser et déposez le [!UICONTROL système d’exploitation mobile] dans l’éditeur de segments.

![](assets/image2015-5-27-17-3a45-3a3.png)

* **Type de visiteur**<br />
  **[!UICONTROL Mobile OS]** : dans la liste déroulante, sélectionnez un ou plusieurs systèmes d’exploitation mobiles répertoriés. Le système d’exploitation mobile sélectionné s’affiche ci-dessous.

   * Le visiteur utilise un appareil mobile
   * Le visiteur utilise ce périphérique/système d’exploitation spécifique
   * Le visiteur n’utilise aucun appareil mobile

* **[!UICONTROL Appareil]** - Dans la liste déroulante, choisissez un ou plusieurs appareils (Apple, Samsung, LG, HTC, Nexus, Blackberry etc...). Les appareils sélectionnés s’affichent ci-dessous.

**Navigateur**

Ciblez les visiteurs et visiteuses qui utilisent des types et/ou des versions de navigateur spécifiques.

* Type de navigateur : dans la liste déroulante, sélectionnez un ou plusieurs navigateurs Internet . Les navigateurs sélectionnés s’affichent ci-dessous.
* Version du navigateur - Saisissez la version du navigateur que vous souhaitez ajouter au segment. Vous pouvez sélectionner plusieurs versions en les séparant par une virgule. (L’utilisation de &#42; comme caractère générique est autorisée).

### API {#api}

**Événements de données** - Segmentez les visiteurs qui déclenchent des événements de données personnalisés spécifiques

Ajoutez la valeur d’événement à cibler. Par exemple, à partir de sources de données tierces.

**API de contexte utilisateur**

Appel API Web Personalization [en savoir plus ici.](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/web-personalization)

>[!TIP]
>
>**Utilisation de caractères génériques -** Lorsque vous souhaitez inclure un terme de recherche ou une URL qui contient quelque chose, c’est-à-dire « [google.com](https://google.com) » ou « produit du terme de recherche », nous appelons cela un caractère générique et il doit être saisi avec un astérisque - ce petit gars &#42; - à chaque extrémité. Ainsi, tout ce qui provient de [google.com](https://google.com) doit être saisi sous la forme &#42; [google.com](https://google.com)&#42;

## Modifier [!UICONTROL Segments] {#edit-segments}

Vous pouvez modifier un segment qui a été créé.

1. Pour modifier un segment, accédez à **[!UICONTROL Segments]**.

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. Dans le tableau **[!UICONTROL Segments]**, cliquez sur l’icône de modification ( ![](assets/segment-edit.png)) du segment que vous souhaitez modifier. La page **[!UICONTROL Définir le segment]** s’ouvre avec le segment sélectionné.
1. Appliquez les modifications que vous souhaitez apporter au segment.
1. Cliquez sur **[!UICONTROL Enregistrer]**.

## Supprimer les segments {#delete-segments}

Vous pouvez supprimer les segments que vous avez créés.

1. Sélectionnez un segment sur la page **[!UICONTROL Segments]** ci-dessus.
1. Cliquez sur l’icône de suppression ( ![](assets/segment-delete.png) ) du segment que vous souhaitez supprimer.
1. Un message de confirmation s’affiche, confirmant que vous êtes sur le point de supprimer le **segment**.

>[!NOTE]
>
>Vous ne pouvez pas supprimer un segment associé à une campagne. Vous devez d’abord supprimer la campagne, puis le segment.

Fantastique ! Maintenant que vous comprenez la section Segments , nous allons en savoir plus sur les campagnes.

>[!MORELIKETHIS]
>
>* [Créer un segment web de base](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)
>* [Créer une campagne web de boîte de dialogue](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [Créer une campagne web dans la zone](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Créer une campagne web de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
