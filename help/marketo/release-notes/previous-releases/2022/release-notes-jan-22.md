---
description: Notes de mise à jour - Janvier 2022 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Janvier 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 3%

---

# Notes de mise à jour : Janvier 2022 {#release-notes-jan-22}

Les fonctionnalités suivantes sont incluses dans la version du 22 janvier. Vérifiez la disponibilité de votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_**

Les fonctionnalités suivantes commenceront à être publiées sur **21 janvier 2022**, avec un déploiement échelonné de chaque fonctionnalité au cours des semaines suivantes (sauf indication contraire).

## Expérience de nouvelle génération {#modern-ux}

* **Mise à jour d’Screens dans l’expérience de nouvelle génération**: Nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour, accessibles par le biais d’un bouton d’activation/désactivation :

   * Détails des ressources de page d’entrée dans Design Studio
   * Détails des ressources de page d’entrée dans les activités marketing

## Intégration à Microsoft Dynamics {#microsoft-dynamics-integration}

* **Synchronisation du type de champ à sélection multiple facultatif disponible en général**: Synchronisez le type de champ d’ensemble d’options à sélection multiple à partir de Microsoft Dynamics pour tirer parti des listes dynamiques et des campagnes dynamiques pour un ciblage d’audience plus granulaire. Par exemple : rubriques/produits intéressants, modes de communication préférés, etc. Cette nouvelle synchronisation est disponible pour Microsoft Dynamics version 9.X (y compris Dynamics 365 Online).

* **Authentification serveur à serveur pour Microsoft Dynamics 365 Online**: Pour une sécurité accrue, nous allons désormais prendre en charge Serveur vers Serveur (S2S) comme mode d’authentification supplémentaire pour l’utilisateur de synchronisation du Marketo Engage sur Azure Principal Directory pour un accès non interactif à Microsoft Dynamics 365 Online. Cela vous permet d’utiliser l’authentification multifactorielle, car toutes les authentifications et les connexions seront basées sur OAuth (uniquement l’identifiant client et le secret client).

>[!NOTE]
>
>Le mode S2S est basé sur Utilisateur de l’application plutôt que Utilisateur sous licence, ce qui enregistre l’utilisation d’une licence supplémentaire.

## Administration {#administration}

* **[Règles de validation de formulaire](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: Préserver l’intégrité de votre base de données avec la possibilité de bloquer les domaines d’email problématiques ou indésirables de l’envoi de formulaires Marketo Engage. Le panneau Règle de validation de formulaire globale permet aux administrateurs de définir une liste bloquée ou d’activer une liste prédéfinie de domaines consommateurs libres à bloquer à partir de formulaires.

* **[Sécurité des en-têtes de page d’entrée](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: Les administrateurs peuvent gérer les en-têtes Strict Transport Security et X-Frame Options sur leurs domaines de page d’entrée afin d’appliquer des exigences de sécurité strictes.

**_Sortie pendant tout le trimestre_**

Les fonctionnalités suivantes, qui ne sont pas trimestrielles, seront publiées au cours des prochains mois.

## Connecteur de destination Marketo Engage AEP - Créer des pistes Net-new {#aep-marketo-engage-destination-connector}

Les clients Marketo Engage qui utilisent également Adobe Experience Platform (AEP) peuvent optimiser leur base de données avec la possibilité de transférer de nouveaux enregistrements de personne vers Marketo Engage à partir d’AEP via le connecteur de destination AEP. Lors de l’envoi de segments d’audience d’AEP vers Marketo Engage, les personnes du segment qui n’existent pas déjà dans votre base de données de Marketo Engage [peut y être automatiquement ajouté](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## Sales Insight {#sales-insight}

![(étoile)](assets/yellow-star.png)

**Sales Insight for Salesforce CRM**

* **Nouvelle colonne Type pour les meilleurs paris**: Les vendeurs obtiendront des informations plus rapides avec une nouvelle colonne intitulée &quot;Type&quot; afin de différencier les pistes et les contacts sur la page Meilleurs paris.

* **Mise à jour de l’API de Platform Salesforce**: En réponse à la retraite de l’API Salesforce Platform versions 21.0 à 30.0, le package Sales Insight a été mis à jour avec les dernières API.

* **Marque mise à jour**: Toutes les pages d’aperçu des ventes sont mises à jour afin de s’aligner sur la valorisation de marque Adobe.

**Sales Insight for Microsoft Dynamics**

* **Mise en page du compte mise à jour**: Les vendeurs peuvent obtenir une vue collective des principales activités, telles que : activités d’e-mail, activités web, moments intéressants et changements de score pour tous les contacts d’un compte.

## SalesConnect {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Appeler les résultats et les raisons**: Découvrez et effectuez le suivi des efforts sortants de vos équipes commerciales plus en détail grâce aux nouvelles options de motif et de résultat d’appel entièrement personnalisables. Outre ces nouveaux champs, nous introduisons une nouvelle gouvernance pour appliquer la raison de l’appel et la sélection des résultats pendant que les vendeurs lancent des appels, une nouvelle gouvernance pour activer ou désactiver les motifs et les résultats de l’appel, ainsi qu’un nouveau champ personnalisé Raison de l’appel et Activité de Salesforce de résultat pour consigner les données dans Salesforce. [Cliquez ici](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) pour en savoir plus.

* **Personnalisation des détails de l’activité Salesforce**: Capturez davantage de données sur les activités et les tâches de vente dans Salesforce en personnalisant les informations ajoutées au champ Objet de la tâche Salesforce lorsqu’une activité de vente est connectée à Salesforce à partir de Sales Connect. [Cliquez ici](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) pour en savoir plus.

## Annonces {#announcements}

* **Obsolescence du Marketo Sky**: En mars, Marketo Sky ne sera plus disponible, car nous concentrons nos ressources sur la diffusion de l’expérience utilisateur de nouvelle génération. Afin de maintenir l’accès aux fonctionnalités exclusives à Marketo Sky aujourd’hui, nous incluons l’expiration des ressources et le remplacement de la priorité des campagnes dynamiques dans l’expérience principale en mars. [Cliquez ici](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) pour en savoir plus.

* **Obsolescence des points de fin de formulaire**: Les POST de formulaire programmatique non pris en charge vers le point de terminaison leadCapture/save2 seront rejetés par les formulaires Marketo Engage. [Cliquez ici](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) pour en savoir plus.

**Domaines Marketo Engage - Configuration de Sales Insight**: Pour les domaines de Marketo Engage pour lesquels le certificat SSL n’est pas configuré et https://, les appels échouent avec une erreur de liaison SSL. Par conséquent, ces domaines vont être supprimés. Par conséquent, les utilisateurs de Sales Insight disposant d’une ancienne configuration pointant vers l’un de ces domaines peuvent rencontrer des erreurs d’légende système sur leur page Lead, contact, compte, panneaux d’opportunités ou globale Marketo. Nous vous recommandons de mettre à jour votre [Configuration du Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) dans Salesforce si vous rencontrez cette erreur. Il vous suffit de mettre à jour les informations d’identification du Marketo Engage en surbrillance dans la section &quot;Configuration de Marketo Sales Insight&quot; du document.

**_Webinaire sur la version du produit_**

[Webinaire de mise à jour de janvier 2022 pour les Marketo Engage](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
