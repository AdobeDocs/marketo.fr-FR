---
unique-page-id: 15695924
description: Classement et réglage du profil de compte - Documents Marketo - Documentation du produit
title: Classement et réglage des profils de compte
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 3%

---

# Classement et réglage des profils de compte {#account-profiling-ranking-and-tuning}

Le profilage de compte identifie votre profil client idéal (ICP), classe les entreprises de votre base de données en fonction de l’ICP et ajoute les données d’indicateur ICP aux comptes promus en tant que comptes nommés.

## Résultats du modèle {#model-results}

Les résultats vous montrent tous vos comptes connus, ventilés par note. A est la note la plus élevée, D est la note la plus basse.

![](assets/results.png)

Bien que cela soit facultatif, nous vous recommandons de cocher la case Convertir automatiquement , car cela vous fera gagner une tonne de temps. Cependant, si vous souhaitez parcourir chaque compte et [les ajouter manuellement](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts), laissez simplement la case désélectionnée.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Classement</strong></td> 
   <td> 
    <div>
      Classement du compte en fonction du profil client idéal. A est la meilleure, D est la moins bonne. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Propension</strong></td> 
   <td> 
    <div>
      Augmentation estimée du taux de conversion par rapport à une sélection de comptes non basée sur le PII. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Comptes (%)</strong></td> 
   <td> 
    <div>
      Pourcentage de comptes dans l’entrée de modèle ayant ce rang. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% de la base du modèle</strong></td> 
   <td> 
    <div>
      Pourcentage de comptes de type modèle ayant ce rang. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Réglage du modèle {#model-tuning}

Dans l’onglet Modèle , cliquez sur le bouton Régler le modèle .

![](assets/two.png)

Il existe plusieurs onglets, permettant une personnalisation approfondie.

![](assets/tuning-page.png)

**Catégories d’indicateurs**

<table> 
 <tbody> 
  <tr> 
   <td><strong>Conformité</strong></td> 
   <td> 
    <div>
      Certifications, postes ou embauche liés à la conformité. 
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
      Logiciel de gestion des ressources humaines ou de la paie, postes/embauche liés aux ressources humaines.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Ingénierie</strong></td> 
   <td> 
    <div>
      Des technologies, des cadres, des postes liés à l'ingénierie ou à l'embauche. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Service commercial</strong></td> 
   <td> 
    <div>
      Solutions et logiciels pour les ventes, les postes liés aux ventes/l’embauche. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Intention</strong></td> 
   <td> 
    <div>
      Indicateurs d'intention. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      Matériel et logiciels, technologies, postes/embauche liés à l'informatique.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Finance</strong></td> 
   <td> 
    <div>
      Logiciels financiers, postes/embauche liés aux finances. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Marketing</strong></td> 
   <td> 
    <div>
      Technologies marketing et logiciels, postes/embauche liés au marketing. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Entreprises</strong></td> 
   <td> 
    <div>
      Forbes ou Inc listes ou partenariats commerciaux. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Expérience client et relations</strong></td> 
   <td> 
    <div>
      Succès des clients et postes/embauche dans les relations client.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Passez la souris sur les info-bulles pour obtenir une description de chaque colonne.

![](assets/tool-tip.png)

Cliquez sur la liste déroulante Ajouter un indicateur ICP pour insérer des indicateurs supplémentaires dans votre modèle.

![](assets/add-icp.png)

Cochez la case Exporter pour afficher l’indicateur ICP sur la page Détails du compte nommé et utiliser l’indicateur ICP sélectionné comme contraintes dans les [filtres de compte nommé](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>Les indicateurs ICP sont inclus en tant que contraintes dans les filtres et déclencheurs **Member of Named Account** .

La pondération de l’indicateur détermine le niveau d’importance que chaque indicateur reçoit dans votre modèle.

![](assets/weightage.png)

Cliquez sur Actualiser le modèle pour que ces modifications soient prises en compte.

![](assets/refresh-button.png)

Une fois le modèle paramétré (après l’avoir actualisé), revenez à l’onglet Résultats du modèle et cliquez sur **Enregistrer et appliquer des classements**.

![](assets/ranks.png)
