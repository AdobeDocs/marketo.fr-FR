---
description: Statut de synchronisation de Salesforce - Documents marketing - Documentation du produit
title: Statut de synchronisation Salesforce
translation-type: tm+mt
source-git-commit: 98af67caaf485535ba2177aa661a503990e8698d
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---


# Statut de synchronisation Salesforce {#salesforce-sync-status}

Utilisez le Tableau de bord Etat de synchronisation pour vue les statistiques de synchronisation dans le cadre des étapes de synchronisation et de son état de réussite.

Les étapes de synchronisation reflètent les opérations de type Push ou Extraction selon chaque type d’objet pour le schéma d’objet et les données elles-mêmes. Les statistiques couvrent les nouveaux enregistrements, les mises à jour, les suppressions et les échecs de comptage pendant la synchronisation. Les utilisateurs peuvent filtrer par date, type d’opération ou type d’objet. Le Tableau de bord d&#39;état de synchronisation affiche l&#39;état des cycles de synchronisation pour les cinq derniers jours.

>[!NOTE]
>
>Autorisations d’administrateur requises

## Etat de synchronisation de la vue {#view-sync-status}

1. Cliquez sur **Admin**.

   ![](assets/salesforce-sync-status-1.png)

1. Sous Intégration, cliquez sur Salesforce, puis sur l’onglet Etat de synchronisation.

   ![](assets/salesforce-sync-status-2.png)

Par défaut, les statistiques sont triées en fonction du plus récent démarrage. Vous pouvez trier en cliquant sur l’icône de tri, en commençant par Démarré à ou Terminé à, du plus récent au plus ancien.

![](assets/salesforce-sync-status-3.png)

## Statut de synchronisation du filtre {#filter-sync-status}

1. Pour filtrer les données, cliquez sur l’icône de filtre située à l’extrémité droite de la page.

   ![](assets/salesforce-sync-status-4.png)

1. Sélectionnez la date et l’heure, puis cliquez sur les listes déroulantes pour filtrer par type d’objet, type d’opération et/ou type d’état.

   ![](assets/salesforce-sync-status-5.png)

1. Cliquez sur **Appliquer**.

   ![](assets/salesforce-sync-status-6.png)

**Étape** facultative : Pour exporter les erreurs de synchronisation, cliquez sur  **Exporter**. Les données seront exportées au format CSV.

![](assets/salesforce-sync-status-7.png)

## Champs d&#39;état de synchronisation {#sync-status-fields}

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
   <td colspan="1">Commencé à</td> 
   <td colspan="1">Date/heure du début de cycle de synchronisation (fuseau horaire de l’utilisateur)</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Terminé à</td> 
   <td colspan="1">Date/heure de fin du cycle de synchronisation (fuseau horaire de l’utilisateur)</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Objet</td> 
   <td colspan="1">Type d’objet</td> 
   <td colspan="1">Contact, Personne, Tâche, Opportunité, Piste, Autres comme ci-dessous</td> 
  </tr>  
  <tr> 
   <td colspan="1">Opération</td> 
   <td colspan="1">Type d'opération</td> 
   <td colspan="1">Types d'opération ci-dessous</td> 
  </tr>  
  <tr> 
   <td colspan="1">Statut</td> 
   <td colspan="1">Statut du lot</td> 
   <td colspan="1">Réussite, Échec, Incomplet, En cours, Nettoyé*</td> 
  </tr>
  <tr> 
   <td colspan="1">Nouveau</td> 
   <td colspan="1">Nombre de nouveaux enregistrements</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Mis à jour</td> 
   <td colspan="1">Nombre d'enregistrements mis à jour</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Supprimé</td> 
   <td colspan="1">Nombre d'enregistrements supprimés</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Échec de l'élément</td> 
   <td colspan="1">Nombre d'enregistrements dont la synchronisation a échoué</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">Ignoré</td> 
   <td colspan="1">Nombre d'enregistrements ignorés, car aucun changement n'a été apporté aux champs d'intérêt pour la synchronisation</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

*Les données ont retrouvé l’état d’intégrité précédent après l’échec de l’étape de synchronisation.

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
   <td colspan="1">Campaign</td> 
  </tr>  
  <tr> 
   <td colspan="1">Statut du membre Campaign</td> 
  </tr>
  <tr> 
   <td colspan="1">Contact</td> 
  </tr>  
  <tr> 
   <td colspan="1">Modèle de courriel</td> 
  </tr>  
  <tr> 
   <td colspan="1">Événement</td> 
  </tr> 
  <tr> 
   <td colspan="1">Personne (responsable)</td> 
  </tr>  
  <tr> 
   <td colspan="1">Opportunité</td> 
  </tr>  
  <tr> 
   <td colspan="1">Rôle de contact d'opportunité</td> 
  </tr>  
  <tr> 
   <td colspan="1">Tâche</td> 
  </tr>  
  <tr> 
   <td colspan="1">Utilisateur</td> 
  </tr>  
 </tbody> 
</table>

## Type d&#39;opération {#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Type d'opération</th> 
   <th>Trouvé par rapport à ces objets</th> 
   <th>Remarques</th> 
   <th>Type d'opération</th>
  </tr> 
  <tr> 
   <td colspan="1">Lien d’initialisation avec Programme</td> 
   <td colspan="1">Campaign</td> 
   <td colspan="1">Liaison de campagnes aux Programmes</td> 
   <td colspan="1">Mettre à jour</td>
  </tr>  
  <tr> 
   <td colspan="1">Extraire les conversions</td> 
   <td colspan="1">Personne (responsable)*</td> 
   <td colspan="1">Récupérez les actions de conversion de la collecte de données sur le marketing. Les unités (nombres) sont des pistes convertissant en contacts</td> 
   <td colspan="1">Mise à jour, élément non validé ou ignoré</td>
  </tr> 
  <tr> 
   <td colspan="1">Supprimer supprime</td> 
   <td colspan="1">Contact, Personne (responsable), Opportunité, Campaign, Membres Campaign, Contact d'opportunité, Objets personnalisés, Campagnes, Statut de membre Campaign, Rôle Contact d'opportunité</td> 
   <td colspan="1">Suppression d’enregistrements de la collecte de données régionale synchronisés sur le marché</td> 
   <td colspan="1">Supprimé, élément en échec ou ignoré</td>
  </tr>  
  <tr> 
   <td colspan="1">Extraire les mises à jour</td> 
   <td colspan="1">Tâche, personne (responsable), file d'attente de personne (responsable), contact, Événement, opportunité, compte, type de compte, membres Campaign, objets personnalisés, campagnes, statut de membre Campaign, Événements, statut de personne, opportunité, opportunité Rôle contact</td> 
   <td colspan="1">Mises à jour ou nouveaux enregistrements dans SFDC synchronisés sur Marketo, extraction de Événements en tant qu’Activités</td> 
   <td colspan="1">Nouveau, mis à jour, élément non validé ou ignoré</td>
  </tr>  
  <tr> 
   <td colspan="1">Push new</td> 
   <td colspan="1">Tâches, modèles de courrier électronique</td> 
   <td colspan="1">Tâches Push (activités)</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">Mises à jour Push</td> 
   <td colspan="1">Tâches, modèles de courriel, personne, contact, campagnes</td> 
   <td colspan="1">Pousser les mises à jour vers SFDC et supprimer également</td> 
   <td colspan="1">Mise à jour, élément non validé ou ignoré</td>
  </tr>  
  <tr> 
   <td colspan="1">Schéma de synchronisation</td> 
   <td colspan="1">Membres Campaign, Objets personnalisés, Campagnes, Statut de membre Campaign, Tâches, Personne, Opportunité, Rôle Contact d'opportunité, Utilisateurs</td> 
   <td colspan="1">Synchronise les métadonnées pour différents objets afin de déterminer les nouveaux champs à synchroniser lors du cycle suivant.</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Synchroniser avec le programme</td> 
   <td colspan="1">Campagnes</td> 
   <td colspan="1">Synchronisation du programme Marketo avec les campagnes SFDC</td> 
   <td colspan="1">Nouveau, mises à jour, échec ou saut</td>
  </tr> 
  <tr> 
   <td colspan="1">Mettre à jour les activités</td> 
   <td colspan="1">Tâches</td> 
   <td colspan="1">Extraire les Activités de Salesforce</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Mettre à jour FKS</td> 
   <td colspan="1">Tout</td> 
   <td colspan="1">Mettre à jour la clé étrangère de tous les objets</td> 
   <td colspan="1">S/O</td>
  </tr>  
 </tbody> 
</table>

*La configuration de la marque au niveau de l&#39;abonnement détermine l&#39;étiquette &quot;prospect&quot; ou &quot;personne&quot; dans le rapport.
