---
unique-page-id: 11385579
description: Création de schémas de contenu - Documents marketing - Documentation du produit
title: Création de modèles de contenu
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---


# Créer des modèles de contenu {#create-content-patterns}

>[!NOTE]
>
>Selon la date d’achat, votre abonnement Marketo peut inclure soit du contenu prédictif ou du contenu `<sup>AI</sup>`. Pour les utilisateurs de contenu prédictif, Marketo active les fonctionnalités Content`<sup>AI</sup>` Analytics jusqu’au 30 avril 2018. Pour conserver ces fonctionnalités au-delà de cette date, contactez votre responsable de succès client Marketo pour effectuer la mise à niveau vers Marketo Content`<sup>AI</sup>`.

Lorsque vous définissez des modèles de contenu, le contenu est automatiquement découvert lorsqu’un visiteur Web clique sur la page Web HTML correspondant au modèle de contenu. Il est utilisé pour ajouter des pages HTML (billets de blog, communiqués de presse, articles d&#39;actualité) en tant que parties de contenu à la page Tout le contenu. Lorsque la détection automatique est basée sur des modèles de contenu, elle détecte et suit les pages HTML liées au modèle d’URL défini lorsqu’un visiteur Web vue ou clique sur un lien vers la page. Cet élément de contenu (URL, nom de page et métadonnées, y compris l’URL de l’image et la description) est ajouté à la page Tout le contenu pour préparer le contenu prédictif. Pour découvrir automatiquement d’autres contenus, tels que des fichiers PDF et des vidéos incorporées, vous devez [activer la détection de contenu](enable-content-discovery.md).

1. Accédez à **Paramètres de contenu**.

   ![](assets/settings-dropdown-hand-2.png)

1. Cliquez sur **Modèles d’URL**.

   ![](assets/click-url-patterns-hand.png)

1. Cliquez sur **+ **pour ouvrir une ligne où vous pouvez saisir vos informations.

   ![](assets/content-settings-create-patterns-hand.png)

1. Ajoutez l’extension d’URL du domaine où se trouve la page Web. Sélectionnez la catégorie (par exemple, Blog, Article, Fiche produit, Communiqué de presse).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Les éléments de la liste déroulante sur la droite reflètent les catégories que vous avez configurées lorsque vous avez [créé des catégories](set-up-categories.md).

1. Cliquez sur **+ **pour ajouter un autre chemin.

   ![](assets/url-patterns-add2.png)

1. Ajoutez l’extension et la catégorie du chemin d’accès supplémentaire et cliquez sur **Enregistrer**.

   ![](assets/url-patterns-save.png)

## Règles de modèle de contenu {#content-pattern-rules}

* Vous pouvez utiliser un caractère générique n’importe où dans une expression (exemple : *domain.com/**, *domain.com/*blog**)

* Nous recommandons d’utiliser /* à la fin d’une expression pour continuer la découverte de modèles (Exemple : *domain.com/blog/** détecte toutes les publications du dossier Blog)
* Les modèles de contenu ne respectent pas la casse (exemple : *domain.com/Blog/** détecte toutes les pages html sur *domain.com/Blog* et *domain.com/blog*)

* Les paramètres d’URL ne sont pas détectés (ce qui évite de découvrir plusieurs éléments avec la même URL de contenu mais des paramètres différents).

## Exemples {#examples}

Pour *domain.com* :

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
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="—"></td> 
   <td><p>Découvre toute URL contenant le mot "feuille de données :".</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>communiqué de presse</td> 
   <td><p>Une seule page HTML à correspondance exacte est découverte :</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Si l’expression d’URL est vide, le modèle d’URL détecte uniquement la page d'accueil :</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>

