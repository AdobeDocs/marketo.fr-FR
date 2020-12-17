---
unique-page-id: 15695924
description: Classement et réglage du profil de compte - Docs marketing - Documentation du produit
title: Classement et réglage des profils de compte
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---


# Classement et réglage du profil de compte {#account-profiling-ranking-and-tuning}

Le profilage de compte identifie votre Profil client idéal (ICP), classe les sociétés dans votre base de données en fonction du PCI et ajoute des données d&#39;indicateur ICP aux comptes promus en tant que comptes nommés.

## Résultats du modèle {#model-results}

Les résultats vous montrent tous vos comptes connus ventilés par note. A est la note la plus élevée, D la note la plus basse.

![](assets/results.png)

Bien que cette case soit facultative, nous vous recommandons de la cocher Promouvoir automatiquement, car elle vous fera gagner une tonne de temps. Cependant, si vous souhaitez passer en revue chaque compte et [les ajouter manuellement](http://docs.marketo.com/display/DOCS/Discover+Accounts#DiscoverAccounts-DiscoverCRMAccounts), laissez simplement la case décochée.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Classement</strong></td> 
   <td> 
    <div>
      Classement du compte en fonction du Profil client idéal. A est la meilleure, D est la moins bonne. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Propensité</strong></td> 
   <td> 
    <div>
      Augmentation estimée du taux de conversion par rapport à une sélection de comptes non fondée sur le PCI. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Comptes (%)</strong></td> 
   <td> 
    <div>
      Pourcentage de comptes dans les entrées de modèle ayant ce classement. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% de la base du modèle</strong></td> 
   <td> 
    <div>
      Pourcentage de comptes de la base du modèle ayant ce classement. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Réglage du modèle {#model-tuning}

Dans l&#39;onglet Modèle, cliquez sur le bouton Réglage du modèle.

![](assets/two.png)

Il existe plusieurs onglets qui permettent une personnalisation approfondie.

![](assets/tuning-page.png)

Catégories d&#39;indicateur

| **Conformité** | Certifications, postes liés à la conformité/embauche. |
|---|---|
| **Opérations** | Postes liés aux opérations/embauche. |
| **HR** | Logiciel des RH ou de la paye, postes liés aux RH/embauche. |
| **Ingénierie** | Technologies, cadres, postes liés à l&#39;ingénierie/embauche. |
| **Ventes** | Solutions et logiciels pour les ventes, les postes liés aux ventes/l&#39;embauche. |
| **Intention** | Indicateurs d’intention. |
| **IT** | Solutions matérielles et logicielles, technologies, postes informatiques/embauche. |
| **Finances** | Logiciels financiers, postes financiers/embauche. |
| **Marketing** | Technologies et logiciels de marketing, postes liés au marketing/embauche. |
| **Entreprise** | Forbes ou Inc annonces ou partenariats d&#39;affaires. |
| **Expérience client et relations** | Positions/embauches sur la réussite et les relations client. |

Passez la souris sur les info-bulles pour obtenir une description de chaque colonne.

![](assets/tool-tip.png)

Cliquez sur la liste déroulante Ajouter un indicateur ICP pour insérer des indicateurs supplémentaires dans votre modèle.

![](assets/add-icp.png)

Si vous cochez la case Exporter, vous pouvez afficher l&#39;indicateur ICP sur la page Détails du compte nommé et utiliser l&#39;indicateur ICP sélectionné comme contraintes dans les [filtres de compte nommés](http://docs.marketo.com/display/DOCS/Account+Filters).

![](assets/export.png)

>[!NOTE]
>
>Les indicateurs ICP sont inclus en tant que contraintes dans les Filtres et déclencheurs **Membre du compte nommé**.

La pondération de l&#39;indicateur détermine le niveau d&#39;importance que chaque indicateur reçoit dans votre modèle.

![](assets/weightage.png)

Cliquez sur Actualiser le modèle pour que ces modifications prennent effet.

![](assets/refresh-button.png)

Lorsque vous avez terminé de régler votre modèle (après l&#39;avoir actualisé), revenez à l&#39;onglet Résultats du modèle et cliquez sur **Enregistrer et appliquer les classements**.

![](assets/ranks.png)

