---
unique-page-id: 13795395
description: Notes de mise à jour - Hiver 2018 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - hiver 18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 6%

---

# Notes de mise à jour : hiver 18 {#release-notes-winter}

Les fonctionnalités suivantes sont incluses dans la version de l’hiver 18. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Marketo.

Cliquez sur les liens de titre pour afficher des articles détaillés pour chaque fonctionnalité. **Remarque** : Certaines des fonctionnalités incluses dans cette version n’ont pas d’articles associés. Si une rubrique comporte plusieurs sous-titres, les liens y sont placés.

## Amélioration des performances et du débit des campagnes {#campaign-performance-and-throughput-enhancements}

Marketo exploite notre architecture de données massives pour augmenter le débit des campagnes et améliorer le traitement des activités web, afin que vous puissiez réagir plus rapidement aux actions de votre audience.

## Améliorations au niveau de l’intégration de la solution CRM de Salesforce par Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Deux améliorations ont été apportées à notre intégration Salesforce CRM :

* [ Notifications de l’administrateur Marketo ](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) pour certains échecs de synchronisation CRM (informations d’identification expirées, limites de l’API atteintes, etc.)

* [Possibilité de désactiver les notifications par e-mail](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) pour les propriétaires de piste lors de l’attribution de pistes

Ces améliorations seront déployées en 2018.

## [Marketo Performance Insights](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>Performance Insights est un produit complémentaire. Contactez votre gestionnaire de compte ou votre gestionnaire de compte Marketo pour obtenir un devis.

Découvrez l’impact de vos campagnes et canaux sur les résultats de l’entreprise grâce aux analyses d’attribution, aux visualisations interactives et à un tableau de données détaillé.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Améliorations marketing basées sur les comptes {#account-based-marketing-enhancements}

**[Hiérarchies ABM](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Pour les clients ABM avec Salesforce ou Microsoft Dynamics, ABM héritera désormais automatiquement (et affichera) les relations parents-enfants établies dans le CRM. Vous pourrez utiliser ces relations dans les rapports de cumul et dans l’exécution des campagnes.

## Marketing par e-mail {#email-marketing}

**[Script de messagerie dynamique](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Les scripts Velocity sont désormais pris en charge dans les emails utilisant du contenu dynamique. Combinez du contenu dynamique basé sur la vitesse et la segmentation pour créer des emails hautement personnalisés.

**Fuseau horaire du destinataire**

* **[Cadence mensuelle d’allaitement](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)** : nous avons ajouté la possibilité de planifier des programmes d’éducation en cadence mensuelle.

* **[Arrêter la diffusion](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)** : vous pouvez désormais arrêter tous les envois restants en cours d’exécution.

## Intégrations de réseaux publicitaires {#ad-network-integrations}

**[Intégration du ciblage par liste de clients de Google](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Avec cette intégration, vous pouvez envoyer une audience Marketo à Google pour qu’elle soit ciblée à l’aide de Google AdWords, ainsi que re-cibler les audiences dans YouTube, Search et Gmail.

**[Amélioration de l’API d’audiences mappées LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

Notre nouvelle API LinkedIn vous permet désormais de recibler des personnes de votre base de données Marketo sur plusieurs comptes LinkedIn Campaign Manager.

## Personnalisation Web {#web-personalization}

**Source de données japonaises pour Personalization web**

Marketo ajoute une source de données japonaise supplémentaire pour le Personalization web afin d’améliorer l’identification des visiteurs web (recherche d’adresses IP inversées) et la personnalisation pour les visiteurs venus du Japon. Les noms des organisations s’affichent en japonais.

**[Création d’un segment Web avec des listes statiques](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Web Personalization peut désormais personnaliser le contenu pour un visiteur Web connu qui fait partie d’une liste statique définie dans les activités marketing (MLM). Grâce à cette amélioration, vous pouvez désormais commercialiser des listes statiques sur plusieurs canaux et cibler des personnes sur ces listes avec du contenu personnalisé sur votre site web.

## ContentAI {#contentai}

**Amélioration de l’algorithme prédictif**

Le contenu recommandé via les algorithmes optimisés de Marketo ContentAI génère jusqu’à deux fois plus de clics que de contenu aléatoire.

## Intégration {#integration}

**[Activer/Désactiver l’API Campaign](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/assets/smart-campaigns)**

Cette nouvelle API vous permet d’activer et de désactiver à distance les campagnes de déclenchement. Vous pouvez ainsi créer des modèles de programme entièrement automatisés. Créez un modèle de programme une seule fois, puis automatisez le clonage, les mises à jour des documents marketing et maintenant l’activation/la planification des campagnes intelligentes.

## ToutApp {#toutapp}

**Mise à jour de la désinscription**

À compter du 1er mars 2018, tous les emails envoyés à partir de [ToutApp.com](https://ToutApp.com) (et en utilisant le bouton &quot;Envoyer un courriel avec tout&quot; dans Salesforce) auront un lien de désabonnement ajouté en bas de la page.

**Mise à jour du flux en direct**

Nous avons mis à jour l’aspect des onglets Engagement et Tâche afin que les membres du service commercial puissent plus facilement et plus rapidement répondre aux activités de leurs clients directement à partir du flux en direct.

**Mise à jour de la vue détaillée de personne**

La vue Détails des personnes (PDV) améliorée offre une vue complète de vos contacts en rassemblant vos coordonnées Tout et Salesforce CRM.
