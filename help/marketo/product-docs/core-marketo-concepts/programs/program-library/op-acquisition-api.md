---
description: OP-Acquisition-API - Documents Marketo - Documentation du produit
title: OP-Acquisition-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 19%

---

# OP-Acquisition-API {#op-acquisition-api}

Cet exemple de programme concerne les processus opérationnels permettant de suivre l’acquisition d’enregistrements à partir de sources API à l’aide d’un programme par défaut Marketo Engage.

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
   <td>Définir l'acquisition - Lot</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Définir l’acquisition - Déclencheur</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Campagnes (contient toutes les campagnes intelligentes)</td>
  </tr>
 </tbody>
</table>

![](assets/op-acquisition-api-1.png)

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

* Exécutez d’abord la campagne par lots si vous devez rattraper votre retard en matière de gestion des données.

* Envisagez d’utiliser des programmes similaires pour garantir l’alignement sur les bonnes pratiques de toutes les sources d’entrée afin d’inclure vos intégrations de données ou CRM.

* Dans le cadre des initiatives marketing spécifiques aux canaux, veillez à capturer l’acquisition en cas de besoin.
