---
description: Gestion des prospects - Documents Marketo - Documentation du produit
title: Gestion des leads d’opération
feature: Programs
exl-id: bde644fe-d40b-4c9c-925d-a0f522e6de01
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 13%

---

# Gestion des leads d’opération {#op-lead-management}

Il s’agit d’un exemple de workflow des bonnes pratiques de gestion de prospect, utilisant un programme par défaut de Marketo Engage, pour vous aider à gérer les enregistrements de votre base de données Marketo Engage vers votre CRM.

>[!NOTE]
>
>Dans Marketo Engage, les enregistrements de votre base de données sont appelés personnes/personne. Dans cet exemple, la gestion des prospects se rapporte aux enregistrements de votre CRM.

Pour obtenir de l’aide sur la stratégie ou la personnalisation d’un programme, contactez l’équipe du compte Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html).

## Résumé du canal {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Canal</th>
   <th>Statut d’abonnement</th>
   <th>Comportement d'analyse</th>
   <th>Type de programme</th>
  </tr>
  <tr>
   <td>Opérationnel</td>
   <td>01-Membre</td>
   <td>Opérationnel</td>
   <td>Par défaut</td>
  </tr>
 </tbody>
</table>

## Le programme contient les Assets suivantes {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Type</th>
   <th>Nom du modèle</th>
   <th>Nom de la ressource</th>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>01 - Synchroniser les nouvelles personnes avec CRM</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>02 - Qualifié pour le marketing</td>
  </tr>
  <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle d’e-mail de démarrage rapide</a></td>
   <td>01 - Email - ALERTE - MQL</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Campagnes</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Alerte par courrier électronique</td>
  </tr>
 </tbody>
</table>

![](assets/op-lead-management-1.png)

## Règles de conflit {#conflict-rules}

* **Balises de programme**
   * Créer des balises dans cet abonnement - _Recommandé_
   * Ignorer

* **Modèle de page de destination portant le même nom**
   * Copier le modèle d’origine - _Recommandé_
   * Utiliser le modèle de destination

* **Images du même nom**
   * Conserver les deux fichiers - _Recommandé_
   * Remplacer l&#39;élément de cet abonnement

* **Modèles d’e-mail portant le même nom**
   * Conserver les deux modèles - _Recommandé_
   * Remplacer le modèle existant

## Meilleures pratiques {#best-practices}

* Envisagez d’ajouter d’autres campagnes intelligentes pour répondre à chacun des besoins liés au statut du cycle de vie dont vous effectuez peut-être le suivi au sein de votre organisation. Chaque campagne créée dans ce programme est destinée à être un exemple de la version des bonnes pratiques et n’est pas spécifique à tous les cas d’utilisation. N’oubliez pas de mettre à jour les campagnes intelligentes pour répondre à votre processus spécifique de gestion du cycle de vie des prospects.

* Envisagez de mettre à jour la convention de nommage de cet exemple de programme pour qu’elle corresponde à la vôtre.
