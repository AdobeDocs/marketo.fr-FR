---
unique-page-id: 2953415
description: Utilisation de la page Détails de la personne - Documents Marketo - Documentation du produit
title: Utilisation de la page Détails de la personne
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 33%

---

# Utilisation de la page Détails de la personne {#using-the-person-detail-page}

La page des détails d’une personne contient toutes les informations que Marketo connaît sur cette personne. Vous pouvez modifier les données directement depuis cette page.

## Accès à la page Détails de la personne {#getting-to-person-detail-page}

Il existe de nombreuses façons d’ouvrir des personnes spécifiques. Voici quelques exemples :

* Dans la **Base de données**, vous pouvez effectuer une recherche dans la recherche rapide
* Toute **liste dynamique** ou liste
* **Membres** onglet d’un programme
* **Afficher les membres de la campagne** dans une campagne dynamique
* Quelques **rapports**
  <br> 

1. Double-cliquez sur une personne ou cliquez une seule fois sur l’ID sur la gauche.

   ![](assets/one-1.png)

1. Cette action ouvre l’écran des détails de la personne.

   ![](assets/two-5.png)

## Organisation de la page - Salesforce {#page-organization-salesforce}

Les informations sur les personnes sont classées dans les onglets suivants :

| Tabulation | Description |
|---|---|
| Infos | Coordonnées et champs personnalisés relatifs à une personne. |
| Informations sur la société | Informations sur la société et adresse de la personne. |
| Infos sur l&#39;opportunité | Informations sur l’opportunité synchronisées à partir de Salesforce. |
| Champ du lead SFDC | Champs Salesforce intégrés. |
| Champ personnalisé SFDC | Champs Salesforce personnalisés. |
| Journal d&#39;activité | Toutes les activités liées à la personne. |

## Organisation de la page - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Tabulation | Description |
|---|---|
| Infos | Coordonnées et champs personnalisés relatifs à une personne. |
| Informations sur la société | Informations sur la société et adresse de la personne. |
| Infos sur l&#39;opportunité | Informations sur l’opportunité synchronisées à partir de Microsoft. |
| Champs personnalisés Microsoft | Champs Microsoft personnalisés. |
| Champ lead Microsoft | Champs Microsoft intégrés. |
| Journal d&#39;activité | Toutes les activités liées à la personne. |

>[!NOTE]
>
>Vous pouvez également consulter les informations sur les opportunités [insérées via l’API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities) pour les instances qui ne sont pas synchronisées avec un CRM.

## Modification d’un champ {#editing-a-field}

De nombreux champs sont modifiables. Pour mettre à jour les informations d’une personne, saisissez une nouvelle valeur et cliquez en dehors du champ pour enregistrer.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Champs par défaut de Marketo avant la synchronisation du CRM {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
|---|---|---|---|---|
| Adresse | Chiffre d&#39;affaires annuel | IP anonyme | Adresse de facturation | Ville de facturation |
| Pays de facturation | Code postal de facturation | État de facturation | Ville | Nom de la société |
| Pays | Créé à | Date de naissance | Service | Ne pas appeler |
| Cause Ne pas appeler | Raison Ne pas appeler | Adresse e-mail | E-mail non valide | Cause e-mail non valide |
| ID de la société externe | ID du commercial externe | Numéro de fax | Prénom | Nom complet |
| Secteur industriel | Ville déduite | Société déduite | Pays déduit | Aire métropolitaine déduite |
| Indicatif téléphonique local déduit | Code postal déduit | Région déduite | Est anonyme | Est client |
| Est partenaire | Intitulé du poste | Nom | Évaluation | Score |
| Source de personne | Statut | Téléphone principal | Nom d’affichage du [!DNL Facebook] social Marketo | Identifiant du [!DNL Facebook] social Marketo |
| URL de la photo du [!DNL Facebook] social Marketo | URL du profil de [!DNL Facebook] social Marketo | Marketo Social [!DNL Facebook] Reach | Marketo Social [!DNL Facebook] Enrollment Référencées | Visites référencées du [!DNL Facebook] social Marketo |
| Sexe Marketo pour réseaux sociaux | Dernière inscription Marketo sur recommandation via réseaux sociaux | Dernière visite Marketo sur recommandation via réseaux sociaux | Nom d’affichage du [!DNL LinkedIn] social Marketo | Identifiant du [!DNL LinkedIn] social Marketo |
| URL de la photo du [!DNL LinkedIn] social Marketo | URL du profil de [!DNL LinkedIn] social Marketo | Marketo Social [!DNL LinkedIn] Reach | Marketo Social [!DNL LinkedIn] Enrollment Référencées | Visites référencées du [!DNL LinkedIn] social Marketo |
| ID association sociale Marketo | Total des inscriptions Marketo sur recommandation via LinkedIn | Total des visites Marketo sur recommandation via LinkedIn | Nom d’affichage du [!DNL Twitter] social Marketo | Identifiant du [!DNL Twitter] social Marketo |
| URL de la photo du [!DNL Twitter] social Marketo | URL du profil de [!DNL Twitter] social Marketo | Marketo Social [!DNL Twitter] Reach | Marketo Social [!DNL Twitter] Enrollment Référencées | Visites référencées du [!DNL Twitter] social Marketo |
| Deuxième prénom | Numéro téléphone mobile | Nombre d&#39;employés | Numéro de téléphone | Code postal |
| Priorité | Évaluation relative | Rôle | Titre | Code SIC |
| Site | État | Non abonné | Raison désabonnement | Mis à jour à |
| Urgence | Site web |  |  |  |

>[!NOTE]
>
>Certains champs ne sont _pas_ modifiables :
>
>* Journal d&#39;activité
>* Informations sur la société
>* Opportunités pour les contacts SFDC
>* Certains champs spécifiques à Marketo, tels que Date de création et Type de Source d’origine.
>
>En savoir plus sur les [champs gérés par le système](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Création d’un onglet personnalisé pour la page Détails de la personne](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md){target="_blank"}
