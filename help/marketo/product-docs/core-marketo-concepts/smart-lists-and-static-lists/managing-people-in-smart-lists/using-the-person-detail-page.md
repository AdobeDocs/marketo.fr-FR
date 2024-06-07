---
unique-page-id: 2953415
description: Utilisation de la page Détails de la personne - Documents Marketo - Documentation du produit
title: Utilisation de la page Détails de la personne
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 50%

---

# Utilisation de la page Détails de la personne {#using-the-person-detail-page}

La page des détails de la personne contient toutes les informations que Marketo sait sur une personne. Vous pouvez modifier les données directement à partir de cette page.

## Accès à la page Détails de la personne {#getting-to-person-detail-page}

Il y a de nombreuses façons d&#39;ouvrir des personnes spécifiques. Voici quelques exemples :

* Dans la **Base**, vous pouvez effectuer une recherche dans la recherche rapide .
* Quelconque **Liste dynamique** ou liste
* **Membres** onglet d’un programme
* **Affichage des membres de campagne** dans une campagne dynamique
* Certains **rapports**
  <br> 

1. Double-cliquez sur une personne ou cliquez une seule fois sur l’identifiant à gauche.

   ![](assets/one-1.png)

1. L’écran des détails de la personne s’affiche.

   ![](assets/two-5.png)

## Organisation de page - Salesforce {#page-organization-salesforce}

Les informations sur les personnes sont classées dans les onglets suivants :

| Onglet | Description |
|---|---|
| Infos | Coordonnées et champs personnalisés concernant une personne. |
| Informations sur la société | Informations et adresse de la personne. |
| Infos sur l&#39;opportunité | Informations sur les opportunités synchronisées depuis Salesforce. |
| Champ du lead SFDC | Champs Salesforce intégrés. |
| Champ personnalisé SFDC | Champs Salesforce personnalisés. |
| Journal d&#39;activité | Toutes les activités liées à la personne. |

## Organisation de page - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Onglet | Description |
|---|---|
| Infos | Coordonnées et champs personnalisés concernant une personne. |
| Informations sur la société | Informations et adresse de la personne. |
| Infos sur l&#39;opportunité | Informations sur les opportunités synchronisées à partir de Microsoft. |
| Champs personnalisés Microsoft | Champs Microsoft personnalisés. |
| Champ lead Microsoft | Champs Microsoft intégrés. |
| Journal d&#39;activité | Toutes les activités liées à la personne. |

>[!NOTE]
>
>Vous pouvez également afficher les informations sur les opportunités [inséré via l’API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities) pour les instances qui ne sont pas synchronisées avec un CRM.

## Modification d’un champ {#editing-a-field}

De nombreux champs sont modifiables. Pour mettre à jour les informations d’une personne, saisissez une nouvelle valeur et cliquez en dehors du champ à enregistrer.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Champs par défaut de Marketo avant synchronisation CRM {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
|---|---|---|---|---|
| Adresse | Chiffre d&#39;affaires annuel | IP anonyme | Adresse de facturation | Ville de facturation |
| Pays de facturation | Code postal de facturation | État de facturation | Ville | Nom de l’entreprise |
| Pays | Créé à | Date de naissance | Service | Ne pas appeler |
| Cause Ne pas appeler | Raison Ne pas appeler | Adresse e-mail | E-mail non valide | Cause e-mail non valide |
| ID de la société externe | ID du commercial externe | Numéro de fax | Prénom | Nom complet |
| Industrie | Ville déduite | Société déduite | Pays déduit | Aire métropolitaine déduite |
| Indicatif téléphonique local déduit | Code postal déduit | Région déduite | Est anonyme | Est client |
| Est partenaire | Intitulé du poste | Nom | Classement | Évaluation |
| Source de personne | Statut | Téléphone principal | Nom d&#39;affichage Marketo pour Facebook | ID Marketo via Facebook |
| URL de photo Marketo pour Facebook  | URL du profil Marketo pour Facebook  | Portée sociale Marketo via Facebook  | Inscriptions sur recommandation Marketo via Facebook  | Visites sur recommandation Marketo via Facebook  |
| Sexe Marketo pour réseaux sociaux | Dernière inscription Marketo sur recommandation via réseaux sociaux | Dernière visite Marketo sur recommandation via réseaux sociaux | Nom d&#39;affichage Marketo pour LinkedIn | ID Marketo via LinkedIn |
| URL de la photo Marketo pour LinkedIn | URL du profil Marketo pour LinkedIn | Portée sociale Marketo via LinkedIn | Inscriptions Marketo sur recommandation via LinkedIn | Visites sur recommandation Marketo via LinkedIn |
| ID association sociale Marketo | Total des inscriptions Marketo sur recommandation via LinkedIn | Total des visites Marketo sur recommandation via LinkedIn | Nom d&#39;affichage Marketo pour Twitter | ID Marketo via Twitter |
| URL de la photo Marketo pour Twitter | URL du profil Marketo pour Twitter | Portée sociale Marketo via Twitter | Inscriptions Marketo sur recommandation via Twitter | Visites Marketo sur recommandation via Twitter |
| Deuxième prénom | Numéro téléphone mobile | Nombre d&#39;employés | Numéro de téléphone | Code postal |
| Priorité | Évaluation relative | Rôle | Titre | Code SIC |
| Site | État | Non abonné | Raison désabonnement | Mis à jour à |
| Urgence | Site web |  |  |  |

>[!NOTE]
>
>Certains champs sont _not_ editable :
>
>* Journal d&#39;activité
>* Informations sur la société
>* Opportunités de contacts de la DDC
>* Certains champs spécifiques à Marketo, tels que Date de création et Type source d’origine.
>
>En savoir plus sur [Champs gérés par le système](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Création d’un onglet personnalisé pour la page Détails de la personne](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md){target="_blank"}
