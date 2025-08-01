---
description: OP-Data Management - Documents Marketo - Documentation du produit
title: Gestion des données du PO
feature: Programs
exl-id: ac4a522b-37a7-4080-83d6-fbc2203a568b
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 26%

---

# Gestion des données du PO {#op-data-management}

Il s’agit d’un exemple de workflows simples des bonnes pratiques de gestion des données opérationnelles à l’aide d’un programme par défaut qui vous aide à gérer la cohérence des données pour les enregistrements de votre base de données Marketo Engage.

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
   <td>Normaliser le pays - États-Unis</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Normaliser le pays - Royaume-Uni</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Placer sur la liste bloquée Défini sur True</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Définir Est partenaire sur Vrai</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Importer une liste</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Évènement en direct</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Publicité en ligne</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Salon professionnel</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Contenu Web</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Demande sur le Web</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Webinaire</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Nouvelle personne à partir de l’import de liste</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Nouvelle personne de l’événement en direct</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Nouvelle personne à partir d’Advertising en ligne</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Nouvelle personne du salon professionnel</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Nouvelle personne à partir du contenu web</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Nouvelle personne à partir de la demande web</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>Nouvelle personne à partir du webinaire</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Lot de Source de nuit de personnes (pour les instances à trafic élevé)</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Personne Source déclenchée (pour les instances à faible trafic)</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Capturer le Source de la personne</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Normalisation</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Gestion des enregistrements</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Liste de blocage</td>
  </tr>
 </tbody>
</table>

![](assets/op-data-management-1.png)

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
