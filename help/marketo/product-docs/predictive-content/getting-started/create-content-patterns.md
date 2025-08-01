---
unique-page-id: 11385579
description: Création De Modèles De Contenu - Documents Marketo - Documentation Du Produit
title: Créez des modèles de contenu
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
feature: Predictive Content
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 2%

---

# Créez des modèles de contenu {#create-content-patterns}

Lorsque vous définissez des modèles de contenu, le contenu est automatiquement découvert lorsqu’un visiteur web clique sur la page web d’HTML appropriée au modèle de contenu. Il est utilisé pour ajouter des pages HTML (articles de blog, communiqués de presse, articles de presse) en tant qu’éléments de contenu à la page Tout le contenu. Lorsque la découverte automatique est basée sur des modèles de contenu, elle détecte et suit les pages HTML associées au modèle d’URL défini lorsqu’un visiteur web affiche ou clique sur un lien vers la page. Cet élément de contenu (l’URL, le nom de la page et les métadonnées, y compris l’URL de l’image et la description) est ajouté à la page Tout le contenu pour préparer le contenu prédictif. Pour la découverte automatique d’autres contenus, tels que des fichiers PDF et des vidéos incorporées, vous devez [activer la découverte de contenu](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Accédez à **[!UICONTROL Paramètres de contenu]**.

   ![](assets/settings-dropdown-hand-2.png)

1. Cliquez sur **[!UICONTROL Modèles d’URL]**.

   ![](assets/click-url-patterns-hand.png)

1. Cliquez sur le **+** pour ouvrir une ligne dans laquelle vous pouvez saisir vos informations.

   ![](assets/content-settings-create-patterns-hand.png)

1. Ajoutez l’extension URL du domaine où se trouve la page web. Sélectionnez la catégorie (par exemple, [!UICONTROL Blog], [!UICONTROL Article], [!UICONTROL Fiche produit], [!UICONTROL Communiqué de presse]).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Les éléments de la liste déroulante de droite correspondent aux catégories que vous avez configurées lors de la [création de catégories](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Cliquez sur **+** pour ajouter un autre chemin.

   ![](assets/url-patterns-add2.png)

1. Ajoutez l’extension et la catégorie pour le chemin supplémentaire, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/url-patterns-save.png)

## Règles de modèle de contenu {#content-pattern-rules}

* Vous pouvez utiliser un caractère générique n’importe où dans une expression (exemple : _domain.com/&#42;_, _domain.com/&#42;blog&#42;_).

* Nous vous recommandons d’utiliser /&#42; à la fin d’une expression pour continuer la découverte de modèles (exemple : _domain.com/blog/&#42;_ détecte toutes les publications dans le dossier Blog)
* Les modèles de contenu ne respectent pas la casse (exemple : _domain.com/Blog/&#42;_ détecte toutes les pages HTML sur _domain.com/Blog_ et _domain.com/blog_)

* Les paramètres d’URL ne sont pas découverts (cela évite de découvrir plusieurs éléments avec la même URL de contenu mais des paramètres différents).

## Exemples {#examples}

Pour _domain.com_ :

<table>
 <tbody>
  <tr>
   <th>Modèle d’URL</th>
   <th>Résultat</th>
  </tr>
  <tr>
   <td>blog/*</td>
   <td><p>Découvre tout le contenu correspondant au modèle domain.com/blog/ :</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td>
  </tr>
  <tr>
   <td>article/2017/*</td>
   <td><p>Découvre tout le contenu correspondant au modèle domain.com/article/2017/ :</p><p>domain.com/article/2017/5-top-tricks</p></td>
  </tr>
  <tr>
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td>
   <td><p>Découvre toute URL contenant le mot « feuilles de données : »</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td>
  </tr>
  <tr>
   <td>communiqué de presse</td>
   <td><p>Une seule page HTML correspondant exactement est découverte :</p><p>domain.com/press-release</p></td>
  </tr>
  <tr>
   <td colspan="1"> </td>
   <td colspan="1"><p>Si l'expression de l'URL est vide, le modèle d'URL ne détecte que la page d'accueil :</p><p>domain.com</p></td>
  </tr>
 </tbody>
</table>
