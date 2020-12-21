---
unique-page-id: 15695924
description: Classement et réglage du profil de compte - Docs marketing - Documentation du produit
title: Classement et réglage des profils de compte
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# Classement et réglage du profil de compte {#account-profiling-ranking-and-tuning}

Le profilage de compte identifie votre Profil client idéal (ICP), classe les sociétés dans votre base de données en fonction du PCI et ajoute des données d&#39;indicateur ICP aux comptes promus en tant que comptes nommés.

## Résultats du modèle {#model-results}

Les résultats vous montrent tous vos comptes connus ventilés par note. A est la note la plus élevée, D la note la plus basse.

![](assets/results.png)

Bien que cette case soit facultative, nous vous recommandons de la cocher Promouvoir automatiquement, car elle vous fera gagner une tonne de temps. Cependant, si vous souhaitez passer en revue chaque compte et [les ajouter manuellement](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md#discover-crm-accounts), laissez simplement la case décochée.

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

**Catégories d&#39;indicateur**

<table> 
 <tbody> 
  <tr> 
   <td><strong>Conformité</strong></td> 
   <td> 
    <div>
      Certifications, postes liés à la conformité/embauche. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Opérations</strong></td> 
   <td> 
    <div>
      Postes liés aux opérations/embauche. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>HR</strong></td> 
   <td> 
    <div>
      Logiciel des RH ou de la paye, postes liés aux RH/embauche.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Ingénierie</strong></td> 
   <td> 
    <div>
      Technologies, cadres, postes liés à l'ingénierie/embauche. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Ventes</strong></td> 
   <td> 
    <div>
      Solutions et logiciels pour les ventes, les postes liés aux ventes/l'embauche. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Intention</strong></td> 
   <td> 
    <div>
      Indicateurs d’intention. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      Solutions matérielles et logicielles, technologies, postes informatiques/embauche.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Finances</strong></td> 
   <td> 
    <div>
      Logiciels financiers, postes financiers/embauche. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Marketing</strong></td> 
   <td> 
    <div>
      Technologies et logiciels de marketing, postes liés au marketing/embauche. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Entreprise</strong></td> 
   <td> 
    <div>
      Forbes ou Inc annonces ou partenariats d'affaires. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Expérience client et relations</strong></td> 
   <td> 
    <div>
      Positions/embauches sur la réussite et les relations client.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Passez la souris sur les info-bulles pour obtenir une description de chaque colonne.

![](assets/tool-tip.png)

Cliquez sur la liste déroulante Ajouter un indicateur ICP pour insérer des indicateurs supplémentaires dans votre modèle.

![](assets/add-icp.png)

Si vous cochez la case Exporter, vous pouvez afficher l&#39;indicateur ICP sur la page Détails du compte nommé et utiliser l&#39;indicateur ICP sélectionné comme contraintes dans les [filtres de compte nommés](/help/marketo/product-docs/account-based-marketing/engage/account-filters.md).

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
