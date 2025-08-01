---
description: Statut de synchronisation de Salesforce - Documentation de Marketo - Documentation du produit
title: Statut de synchronisation Salesforce
exl-id: 61197808-7812-4e0a-8ac6-4a60af0f7979
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 14%

---

# Statut de synchronisation Salesforce {#salesforce-sync-status}

Utilisez le tableau de bord Statut de la synchronisation pour afficher les statuts de synchronisation dans le cadre des étapes de synchronisation et leur statut de réussite.

Les étapes de synchronisation reflètent les opérations de transfert ou d’extraction par chaque type d’objet pour le schéma d’objet et les données lui-même. Les statistiques couvrent les nouveaux enregistrements, les mises à jour, les suppressions et les nombres d’échecs lors de la synchronisation. Les utilisateurs peuvent filtrer par date, type d’opération ou type d’objet. Le tableau de bord de statut de la synchronisation affiche le statut des cycles de synchronisation des cinq derniers jours.

>[!NOTE]
>
>Autorisations d’administrateur requises

## Afficher le statut de synchronisation {#view-sync-status}

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/salesforce-sync-status-1.png)

1. Sous [!UICONTROL Intégration], cliquez sur **Salesforce**, puis sur l’onglet **[!UICONTROL État de synchronisation]**.

   ![](assets/salesforce-sync-status-2.png)

Par défaut, les statistiques sont triées selon le démarrage le plus récent. Vous pouvez trier par Date de début ou Date de fin (du plus récent au plus ancien) en cliquant sur l’icône de tri.

![](assets/salesforce-sync-status-3.png)

## Statut de synchronisation du filtre {#filter-sync-status}

1. Pour filtrer les données, cliquez sur l’icône de filtrage située à l’extrémité droite de la page.

   ![](assets/salesforce-sync-status-4.png)

1. Sélectionnez votre période et votre heure, puis cliquez sur les listes déroulantes pour filtrer par [!UICONTROL Type d’objet], [!UICONTROL Type d’opération] et/ou [!UICONTROL Type d’état].

   ![](assets/salesforce-sync-status-5.png)

1. Cliquez sur **[!UICONTROL Appliquer]**.

   ![](assets/salesforce-sync-status-6.png)

**ÉTAPE FACULTATIVE** : Pour exporter les erreurs de synchronisation, cliquez sur **[!UICONTROL Exporter]**. Les données seront exportées au format CSV.

![](assets/salesforce-sync-status-7.png)

## Champs de statut de synchronisation {#sync-status-fields}

<table>
 <colgroup>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th>Champ</th>
   <th>Description</th>
   <th>Valeurs d’énumération</th>
  </tr>
  <tr>
   <td colspan="1">Début</td>
   <td colspan="1">Date/heure de début du cycle de synchronisation (fuseau horaire de l’utilisateur)</td>
   <td colspan="1"></td>
  </tr>
  <tr>
   <td colspan="1">Fin</td>
   <td colspan="1">Date/heure de fin du cycle de synchronisation (fuseau horaire de l’utilisateur)</td>
   <td colspan="1"></td>
  </tr>
  <tr>
   <td colspan="1">Objet</td>
   <td colspan="1">Type d’objet</td>
   <td colspan="1">Contact, Personne, Tâche, Opportunité, Lead, Autres comme ci-dessous</td>
  </tr>
  <tr>
   <td colspan="1">Opération</td>
   <td colspan="1">Type d’opération</td>
   <td colspan="1">Types d’opérations, comme ci-dessous</td>
  </tr>
  <tr>
   <td colspan="1">Statut</td>
   <td colspan="1">Statut du lot</td>
   <td colspan="1">Réussite, Échec, Incomplet, En cours, Nettoyage*</td>
  </tr>
  <tr>
   <td colspan="1">Nouveau</td>
   <td colspan="1">Nombre de nouveaux enregistrements</td>
   <td colspan="1"></td>
  </tr>
  <tr>
   <td colspan="1">Mis à jour</td>
   <td colspan="1">Nombre d’enregistrements mis à jour</td>
   <td colspan="1"></td>
  </tr>
  <tr>
   <td colspan="1">Supprimé</td>
   <td colspan="1">Nombre d’enregistrements supprimés</td>
   <td colspan="1"></td>
  </tr>
  <tr>
   <td colspan="1">Élément présentant un échec</td>
   <td colspan="1">Nombre d’enregistrements dont la synchronisation a échoué</td>
   <td colspan="1"><br></td>
  </tr>
  <tr>
   <td colspan="1">Ignoré</td>
   <td colspan="1">Nombre d’enregistrements ignorés car aucun changement n’a été apporté aux champs ciblés pour la synchronisation</td>
   <td colspan="1"></td>
  </tr>
 </tbody>
</table>

&#42;Les données sont redevenues intactes après l’échec de l’étape de synchronisation.

## Type d&#39;objet {#object-type}

<table>
 <colgroup>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td colspan="1">Compte</td>
  </tr>
  <tr>
   <td colspan="1">Type de compte</td>
  </tr>
  <tr>
   <td colspan="1">Objets personnalisés</td>
  </tr>
  <tr>
   <td colspan="1">Campagne</td>
  </tr>
  <tr>
   <td colspan="1">Statut du membre de la campagne</td>
  </tr>
  <tr>
   <td colspan="1">Contact</td>
  </tr>
  <tr>
   <td colspan="1">Modèle d'e-mail</td>
  </tr>
  <tr>
   <td colspan="1">Événement</td>
  </tr>
  <tr>
   <td colspan="1">Personne (Lead)</td>
  </tr>
  <tr>
   <td colspan="1">Opportunité</td>
  </tr>
  <tr>
   <td colspan="1">Rôle du contact d’opportunité</td>
  </tr>
  <tr>
   <td colspan="1">Tâche</td>
  </tr>
  <tr>
   <td colspan="1">Utilisateur</td>
  </tr>
 </tbody>
</table>

## Type d’opération {#operation-type}

<table>
 <colgroup>
  <col>
  <col>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <th>Type d’opération</th>
   <th>Trouvé pour ces objets</th>
   <th>Remarques</th>
   <th>Type d’opération</th>
  </tr>
  <tr>
   <td colspan="1">Créer un lien avec le programme</td>
   <td colspan="1">Campagne</td>
   <td colspan="1">Liaison de campagnes à des programmes</td>
   <td colspan="1">Mise à jour </td>
  </tr>
  <tr>
   <td colspan="1">Extraire les conversions</td>
   <td colspan="1">Personne (Lead)*</td>
   <td colspan="1">Extraction des actions de conversion de SFDC vers Marketo. Les unités (nombres) sont des leads convertis en contacts</td>
   <td colspan="1">Mise à jour, élément en échec ou ignoré</td>
  </tr>
  <tr>
   <td colspan="1">Extraire les suppressions</td>
   <td colspan="1">Contact, Personne (Lead), Opportunité, Campagne, Membres de la campagne, Contact de l’opportunité, Objets personnalisés, Campagnes, Statut de membre de la campagne, Rôle de contact de l’opportunité</td>
   <td colspan="1">Enregistrements supprimés du SFDC synchronisé avec Marketo</td>
   <td colspan="1">Supprimé, Élément en échec ou Ignoré</td>
  </tr>
  <tr>
   <td colspan="1">Extraire les mises à jour</td>
   <td colspan="1">Tâche, Personne (Lead), File D’Attente De Personne (Lead), Contact, Événement, Opportunité, Compte, Type De Compte, Membres De La Campagne, Objets Personnalisés, Campagnes, Statut De Membre De La Campagne, Événements, Statut De Personne, Opportunité, Rôle De Contact De L’Opportunité</td>
   <td colspan="1">Mises à jour ou nouveaux enregistrements dans SFDC synchronisés avec Marketo, extraction des événements en tant qu’activités</td>
   <td colspan="1">Nouvel élément, élément mis à jour, élément en échec ou élément ignoré</td>
  </tr>
  <tr>
   <td colspan="1">Intégrer les nouveaux</td>
   <td colspan="1">Tâches, Modèles d’e-mail</td>
   <td colspan="1">Tâches des notifications push (activités)</td>
   <td colspan="1"></td>
  </tr>
  <tr>
   <td colspan="1">Intégrer les mises à jour</td>
   <td colspan="1">Tâches, Modèles d’e-mail, Personne, Contact, Campagnes</td>
   <td colspan="1">Envoi de mises à jour à SFDC et supprime également</td>
   <td colspan="1">Mise à jour, élément en échec ou ignoré</td>
  </tr>
  <tr>
   <td colspan="1">Synchroniser le schéma</td>
   <td colspan="1">Membres de la campagne, objets personnalisés, campagnes, statut de membre de la campagne, tâches, personne, opportunité, rôle du contact de l’opportunité, utilisateurs</td>
   <td colspan="1">Synchronise les métadonnées de différents objets afin de décider des nouveaux champs à synchroniser au cours du cycle suivant</td>
   <td colspan="1"></td>
  </tr>
  <tr>
   <td colspan="1">Synchroniser avec le programme</td>
   <td colspan="1">Campagnes</td>
   <td colspan="1">Synchronise le programme Marketo avec les campagnes SFDC</td>
   <td colspan="1">Nouveau, Mises à jour, Échec ou Ignoré</td>
  </tr>
  <tr>
   <td colspan="1">Mise à jour des activités</td>
   <td colspan="1">Tâches</td>
   <td colspan="1">Extraire des activités de Salesforce</td>
   <td colspan="1"></td>
  </tr>
  <tr>
   <td colspan="1">Mettre à jour le FKS</td>
   <td colspan="1">Toutes</td>
   <td colspan="1">Mettre à jour la clé étrangère de tous les objets</td>
   <td colspan="1">S/O</td>
  </tr>
 </tbody>
</table>

&#42; La configuration de l’image de marque au niveau de l’abonnement détermine le libellé : « Lead » ou « Personne » dans le rapport.
