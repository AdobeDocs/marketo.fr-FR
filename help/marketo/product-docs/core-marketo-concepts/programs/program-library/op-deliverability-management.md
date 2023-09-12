---
description: Gestion de la délivrabilité des OP - Documents Marketo - Documentation du produit
title: Gestion de la délivrabilité des OP
feature: Programs
source-git-commit: 720215ea958206931413f2d273a4a058bc051579
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 19%

---

# Gestion de la délivrabilité des OP {#op-deliverability-management}

Il s’agit d’un exemple des bonnes pratiques de gestion de la délivrabilité utilisant un programme par défaut de Marketo Engage, pour passer en revue votre état actuel de délivrabilité des emails et gérer les bounces et les non-répondeurs chroniques.

>[!NOTE]
>
>Nécessite l’importation d’un champ de chaîne personnalisé &quot;Motif de suspension marketing&quot;. [En savoir plus](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}.

Pour obtenir de l’aide sur la stratégie ou personnaliser un programme, contactez l’équipe Compte d’Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} page.

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

## Champs prérequis {#prerequisite-fields}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Type</th> 
   <th>Nom convivial</th>
   <th>Nom de l'API</th>
  </tr>
  <tr> 
   <td>Chaîne</td> 
   <td>Raison de la suspension du marketing</td>
   <td>MarketingSuspendedReason</td>
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
   <td>Marketing Suspendre Les Non-Responsables Chroniques</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>Marketing Suspendre Les Emails Rebonds Chroniques</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>Réinitialiser "Email Invalid" après la mise à jour de l’email</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>Réinitialiser "Marketing suspendu" après la mise à jour de l’email</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Gérer</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Examiner</td>
  </tr>
 </tbody> 
</table>

![](assets/op-deliverability-management-1.png)

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

* Chaque campagne créée a pour but de servir d’exemple sur la génération des bonnes pratiques et non de répondre à vos cas d’utilisation. N’oubliez pas de mettre à jour les campagnes intelligentes afin de répondre à vos problèmes spécifiques et à vos défis en matière de données.

* Envisagez de mettre à jour la convention d’affectation des noms de cet exemple de programme pour vous aligner sur votre convention d’affectation des noms.
