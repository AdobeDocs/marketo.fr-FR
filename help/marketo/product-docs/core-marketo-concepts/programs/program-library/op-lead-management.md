---
description: Gestion des pistes OP - Documents Marketo - Documentation du produit
title: Gestion des leads OP
feature: Programs
exl-id: bde644fe-d40b-4c9c-925d-a0f522e6de01
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 13%

---

# Gestion des leads OP {#op-lead-management}

Il s’agit d’un exemple de workflow de bonnes pratiques de gestion des pistes, qui utilise un programme par défaut de Marketo Engage, pour vous aider à gérer les enregistrements dans votre base de données de Marketo Engage dans votre gestion de la relation client (CRM).

>[!NOTE]
>
>Dans Marketo Engage, les enregistrements de votre base de données sont appelés personnes/personnes. Dans cet exemple, la gestion des pistes fait référence aux enregistrements de votre CRM.

Pour obtenir de l’aide sur la stratégie ou personnaliser un programme, contactez l’équipe chargée du compte Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) .

## Résumé du canal {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Canal</th> 
   <th>État d’appartenance</th>
   <th>Comportement d'analyse</th>
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

## Le programme contient l’Assets suivante {#program-contains-the-following-assets}

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
   <td>01 - Synchroniser les nouvelles personnes avec le CRM</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>02 - Marketing qualifié</td>
  </tr>
  <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle de courrier électronique de démarrage rapide</a></td>
   <td>01 - Email - ALERT - MQL</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Campagnes</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Alerte par email</td>
  </tr>
 </tbody> 
</table>

![](assets/op-lead-management-1.png)

## Règles de conflit {#conflict-rules}

* **Balises de programme**
   * Créer des balises dans cet abonnement - _Recommandé_
   * Ignorer

* **Modèle de page d’entrée avec le même nom**
   * Copier le modèle d’origine - _Recommandé_
   * Utiliser le modèle de destination

* **Images du même nom**
   * Conserver les deux fichiers - _Recommandé_
   * Remplacer l&#39;élément de cet abonnement

* **Modèles d&#39;email portant le même nom**
   * Conserver les deux modèles - _Recommandé_
   * Remplacer le modèle existant

## Meilleures pratiques {#best-practices}

* Envisagez d’ajouter des campagnes intelligentes supplémentaires pour répondre à chacun des besoins de cycle de vie dont vous effectuez le suivi dans votre entreprise. Chaque campagne créée dans ce programme est destinée à servir d’exemple de création de bonnes pratiques et n’est pas spécifique à tous les cas d’utilisation. N’oubliez pas de mettre à jour les campagnes intelligentes pour tenir compte de votre processus spécifique de gestion du cycle de vie des prospects.

* Envisagez de mettre à jour la convention de dénomination de cet exemple de programme pour vous aligner sur la vôtre.
