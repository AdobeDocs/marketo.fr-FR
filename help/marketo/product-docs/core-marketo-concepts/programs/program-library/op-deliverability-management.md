---
description: Gestion de la délivrabilité des opérations - Documents Marketo - Documentation du produit
title: Gestion de la délivrabilité des PO
feature: Programs
exl-id: 7b9bc9ee-65f4-4938-8598-6f8543042159
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 19%

---

# Gestion de la délivrabilité des PO {#op-deliverability-management}

Il s’agit d’un exemple de workflow des bonnes pratiques de gestion de la délivrabilité utilisant un programme par défaut de Marketo Engage, pour examiner votre état actuel de délivrabilité des e-mails et gérer les bounces chroniques et les non-répondeurs.

>[!NOTE]
>
>Nécessite le champ de chaîne personnalisé « Motif de suspension du marketing » à importer. [En savoir plus](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}.

Pour obtenir de l’aide sur la stratégie ou la personnalisation d’un programme, contactez l’équipe du compte Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}.

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
   <td>Motif de suspension marketing</td>
   <td>MarketingSuspendedReason</td>
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
   <td>Suspension du marketing Non-répondeurs chroniques</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Suspension Du Marketing Des E-Mails Rebonds Chroniques</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Réinitialiser « E-mail non valide » après la mise à jour des e-mails</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Réinitialiser le « marketing suspendu » après la mise à jour des e-mails</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Gérer</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Réviser</td>
  </tr>
 </tbody>
</table>

![](assets/op-deliverability-management-1.png)

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

* Chaque version de campagne est destinée à être un exemple de la version des bonnes pratiques et n’est pas spécifique à vos cas d’utilisation. N’oubliez pas de mettre à jour les campagnes intelligentes pour résoudre vos problèmes spécifiques et résoudre les problèmes liés aux données.

* Envisagez de mettre à jour la convention de nommage de cet exemple de programme pour l’aligner sur votre convention de nommage.
