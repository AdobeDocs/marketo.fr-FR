---
unique-page-id: 15695924
description: Classement et réglage du profil de compte - Documents Marketo - Documentation du produit
title: Classement et réglage du profilage de compte
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 3%

---

# Classement et réglage du profilage de compte {#account-profiling-ranking-and-tuning}

Le profilage de compte identifie votre profil client idéal, classe les sociétés de votre base de données en fonction du profil ICP et ajoute les données d&#39;indicateur ICP aux comptes promus en tant que [!UICONTROL comptes nommés].

>[!IMPORTANT]
>
>Depuis 2025, le profilage de compte n’est plus disponible pour les nouveaux utilisateurs. Il continuera à fonctionner pour les utilisateurs existants.

## Résultats du modèle {#model-results}

Les résultats vous montrent tous vos comptes connus, répartis par grade. A est la note la plus élevée, D est la note la plus basse.

![](assets/results.png)

Bien que cela soit facultatif, nous vous recommandons de cocher la case Promouvoir automatiquement , car cela vous permettra de gagner beaucoup de temps. Cependant, si vous souhaitez parcourir chaque compte et [les ajouter manuellement](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts), laissez simplement la case décochée.

<table>
 <tbody>
  <tr>
   <td><strong><span class="uicontrol">Classement</span></strong></td>
   <td>
    <div>
      Classement de compte en fonction du profil client idéal. A est le plus adapté, D est le moins adapté.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Propension</span></strong></td>
   <td>
    <div>
      Augmentation estimée du taux de conversion par rapport à une sélection de comptes non basée sur le PCI.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Comptes (%)</span></strong></td>
   <td>
    <div>
      Pourcentage de comptes dans l’entrée du modèle ayant ce rang.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">% de la base du modèle</span></strong></td>
   <td>
    <div>
      Pourcentage de comptes de base modèle ayant ce rang.
    </div></td>
  </tr>
 </tbody>
</table>

## Réglage du modèle {#model-tuning}

Dans l’onglet Modèle , cliquez sur le bouton **[!UICONTROL Régler le modèle]**.

![](assets/two.png)

Plusieurs onglets sont proposés pour une personnalisation en profondeur.

![](assets/tuning-page.png)

**Catégories d’indicateurs**

<table>
 <tbody>
  <tr>
   <td><strong><span class="uicontrol">Conformité</span></strong></td>
   <td>
    <div>
      Certifications, postes liés à la conformité/embauche.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Opérations</span></strong></td>
   <td>
    <div>
      Postes liés aux opérations/embauche.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">H</span></strong></td>
   <td>
    <div>
      Logiciel de RH ou de paie, postes liés aux RH/embauche.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Ingénierie</span></strong></td>
   <td>
    <div>
      Technologies, cadres, postes liés à l'ingénierie/embauche.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Service commercial</span></strong></td>
   <td>
    <div>
      Solutions et logiciels pour les ventes, les postes liés aux ventes et l'embauche.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Intention</span></strong></td>
   <td>
    <div>
      Indicateurs d’intention.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">IT</span></strong></td>
   <td>
    <div>
      Solutions matérielles et logicielles, technologies, postes liés aux TI/embauche.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Finance</span></strong></td>
   <td>
    <div>
      Logiciel de finance, postes liés à la finance/embauche.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Marketing</span></strong></td>
   <td>
    <div>
      Technologies et logiciels de marketing, postes liés au marketing et embauche.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Commerciale</span></strong></td>
   <td>
    <div>
      Listes Forbes ou Inc. ou partenariats d'affaires.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Expérience client et relations</span></strong></td>
   <td>
    <div>
      Positions/embauches en matière de succès client et de relations client.
    </div></td>
  </tr>
 </tbody>
</table>

Pointez sur les info-bulles pour obtenir une description de chaque colonne.

![](assets/tool-tip.png)

Cliquez sur le menu déroulant [!UICONTROL  Ajouter un indicateur ICP ] pour insérer des indicateurs supplémentaires dans votre modèle.

![](assets/add-icp.png)

En cochant la case [!UICONTROL Exporter], vous pouvez afficher l’indicateur ICP sur la page de détails [!UICONTROL Compte nommé] et utiliser l’indicateur ICP sélectionné comme contraintes dans les [filtres de compte nommés](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>Les indicateurs ICP sont inclus en tant que contraintes dans **[!UICONTROL Membre du compte nommé]** Filtres et Triggers.

Le [!UICONTROL Poids de l’indicateur] contrôle le niveau d’importance que chaque indicateur reçoit dans votre modèle.

![](assets/weightage.png)

Cliquez sur **[!UICONTROL Actualiser le modèle]** pour que ces modifications soient prises en compte.

![](assets/refresh-button.png)

Une fois le réglage du modèle terminé (après l&#39;actualisation), revenez à l&#39;onglet Résultats du modèle et cliquez sur **[!UICONTROL Enregistrer et appliquer des rangs]**.

![](assets/ranks.png)
