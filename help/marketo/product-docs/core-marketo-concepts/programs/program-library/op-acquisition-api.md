---
description: OP-Acquisition-API - Documents Marketo - Documentation du produit
title: OP-Acquisition-API
feature: Programs
exl-id: 1d6ec686-af0b-46a9-b428-1520b671ca24
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 21%

---

# OP-Acquisition-API {#op-acquisition-api}

Cet exemple de programme est destiné aux processus opérationnels qui effectuent le suivi de l’acquisition d’enregistrements à partir de sources API utilisant un programme par défaut de Marketo Engage.

## Résumé du canal {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Canal</th> 
   <th>État d’appartenance</th>
   <th>Comportement d’analyse</th>
   <th>Type de programme</th>
  </tr> 
  <tr> 
   <td>Opérationnel</td> 
   <td>01-Member</td>
   <td>Opérationnel</td>
   <td>Par défaut</td>
  </tr>
 </tbody> 
</table>

## Le programme contient les ressources suivantes {#program-contains-the-following-assets}

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
   <td>Définition d’une acquisition - Lot</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>Définition de l’acquisition - Déclencheur</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Campagnes (contient toutes les campagnes dynamiques)</td>
  </tr>
 </tbody> 
</table>

![](assets/op-acquisition-api-1.png)

## Règles de conflit {#conflict-rules}

* **Étiquettes du programme**
   * Créer des balises dans cet abonnement - _Recommandé_
   * Ignorer

* **Modèle de page d’entrée du même nom**
   * Copier le modèle d’origine - _Recommandé_
   * Utiliser le modèle de destination

* **Images du même nom**
   * Conserver les deux fichiers - _Recommandé_
   * Remplacer l’élément de cet abonnement

* **Modèles d&#39;email portant le même nom**
   * Conserver les deux modèles - _Recommandé_
   * Remplacer le modèle existant

## Meilleures pratiques {#best-practices}

* Exécutez d’abord la campagne par lots si vous devez rattraper votre retard dans la gestion des données.

* Envisagez d’utiliser des programmes similaires afin de garantir l’alignement sur les bonnes pratiques pour toutes les sources d’entrée afin d’inclure vos intégrations CRM ou de données.

* Au sein des initiatives marketing de canal spécifiques, veillez à capturer l’acquisition si nécessaire.
