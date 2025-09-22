---
description: Notes De Mise À Jour - Janvier 2022 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Janvier 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 4%

---

# Notes de mise à jour : janvier 2022 {#release-notes-jan-22}

Les fonctionnalités suivantes sont incluses dans la version de janvier 2022. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **21 janvier 2022**, avec un déploiement échelonné de chaque fonctionnalité au cours des semaines suivantes (sauf indication contraire).

## Expérience nouvelle génération {#modern-ux}

* **Mise à jour de Screens dans l’expérience de nouvelle génération** : nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour et accessibles via le bouton bascule :

   * Détails de la ressource de page de destination dans [!UICONTROL Design Studio]
   * Détails de la ressource de page de destination dans [!UICONTROL Activités marketing]

## Intégration [!DNL Microsoft Dynamics] {#microsoft-dynamics-integration}

* **Synchronisation du type de champ de jeu d’options à sélection multiple généralement disponible** : synchronisez le type de champ de jeu d’options à sélection multiple de [!DNL Microsoft Dynamics] pour l’exploiter dans les listes dynamiques et les campagnes dynamiques pour un ciblage d’audience plus granulaire. Par exemple : sujets/produits d’intérêt, modes de communication préférés, etc. Cette nouvelle synchronisation est disponible pour [!DNL Microsoft Dynamics] version 9.X (y compris Dynamics 365 Online).

* **Authentification de serveur à serveur pour[!DNL Microsoft Dynamics 365 Online]** : pour une sécurité accrue, nous prendrons désormais en charge Serveur à serveur (S2S) en tant que mode d’authentification supplémentaire pour l’utilisateur de synchronisation Marketo Engage sur Azure Active Directory pour un accès non interactif à [!DNL Microsoft Dynamics 365 Online]. Vous pouvez ainsi utiliser l’authentification à plusieurs facteurs, car toutes les authentifications seront basées sur OAuth (uniquement l’identifiant et le secret client).

>[!NOTE]
>
>Le mode S2S est basé sur l’utilisateur de l’application plutôt que sur l’utilisateur sous licence, ce qui permet d’économiser l’utilisation d’une licence supplémentaire.

## Administration {#administration}

* **[Règles de validation des formulaires](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)** : préservez l’intégrité de votre base de données et bloquez les domaines d’e-mail problématiques ou indésirables pour l’envoi de formulaires Marketo Engage. Le panneau Règle de validation globale des formulaires permet aux administrateurs de définir une liste bloquée ou d’activer une liste prédéfinie de domaines consommateurs libres à bloquer des formulaires.

* **[Sécurité des en-têtes de page de destination](/help/marketo/product-docs/administration/settings/landing-page-headers.md)** : les administrateurs peuvent gérer les en-têtes Strict Transport Security et X-Frame Options sur leurs domaines de page de destination pour appliquer des exigences de sécurité strictes.

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes font l’objet d’un cycle non trimestriel et seront publiées au cours des prochains mois.

## Connecteur de destination AEP Marketo Engage - Créer de nouveaux prospects {#aep-marketo-engage-destination-connector}

Les clients Marketo Engage qui utilisent également Adobe Experience Platform (AEP) peuvent optimiser leur base de données grâce à la possibilité d’envoyer des enregistrements de nouvelles personnes dans Marketo Engage depuis AEP via le connecteur de destination AEP. Lors de l’envoi de segments d’audience d’AEP vers Marketo Engage, les personnes du segment qui n’existent pas encore dans votre base de données Marketo Engage [peuvent y être automatiquement ajoutées](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## [!DNL Sales Insight] {#sales-insight}

![(étoile)](assets/yellow-star.png)

**[!DNL Sales Insight]pour [!DNL Salesforce] CRM**

* **Nouvelle colonne Type pour les [!UICONTROL Meilleurs résultats]** : les vendeurs obtiendront des informations plus rapides grâce à une nouvelle colonne intitulée « Type » pour différencier les prospects et les contacts sur la page [!UICONTROL Meilleurs résultats].

* **[!DNL Salesforce]mise à jour de l’API Platform** : en réponse au retrait [!DNL Salesforce] des versions 21.0 à 30.0 de l’API [!DNL Salesforce] Platform, le package [!DNL Sales Insight] a été mis à jour avec les dernières API.

* **Image de marque mise à jour** : toutes les pages [!DNL Sales Insight] sont mises à jour pour s’aligner sur l’image de marque Adobe.

**[!DNL Sales Insight]for[!DNL Microsoft Dynamics]**

* **Mise à jour de la disposition du compte** : les vendeurs peuvent obtenir une vue collective des principales activités, telles que : les activités de messagerie électronique, les activités web, les moments intéressants et les changements de score pour tous les contacts d’un compte.

## [!DNL Sales Connect] {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Résultats et motifs de l’appel** : comprenez et suivez plus en détail les efforts sortants de vos équipes commerciales grâce à de nouvelles options entièrement personnalisables de résultat d’appel et de motif d’appel. Outre ces nouveaux champs, nous introduisons une nouvelle gouvernance pour appliquer la sélection du motif de l’appel et du résultat pendant que les vendeurs effectuent des appels, une nouvelle gouvernance pour activer ou désactiver les motifs et les résultats des appels, ainsi qu’un nouveau champ personnalisé Motif de l’appel et Activité de [!DNL Salesforce] du résultat de l’appel pour la journalisation des données dans les [!DNL Salesforce]. [Cliquez ici](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) pour en savoir plus.

* Personnalisation des détails de l’activité **[!DNL Salesforce]** : capturez d’autres données d’activité de vente et de tâche dans [!DNL Salesforce] en personnalisant les informations qui sont ajoutées au champ d’objet de la tâche [!DNL Salesforce] lorsqu’une activité de vente est consignée dans un [!DNL Salesforce] à partir de [!DNL Sales Connect]. [Cliquez ici](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) pour en savoir plus.

## Annonces {#announcements}

* **Obsolescence de Marketo Sky** : en mars, Marketo Sky ne sera plus disponible, car nous concentrons nos ressources sur la diffusion de l’expérience utilisateur de nouvelle génération. Dans un effort de conserver l’accès à une fonctionnalité exclusive à Marketo Sky aujourd’hui, nous intégrons l’expiration des ressources et le remplacement de priorité de campagne intelligent dans l’expérience grand public de mars. [Cliquez ici](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) pour en savoir plus.

* **Obsolescence des points d’entrée de formulaire** : les publications de formulaire programmatiques non prises en charge sur le point d’entrée leadCapture/save2 seront rejetées par les formulaires Marketo Engage. [Cliquez ici](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) pour en savoir plus.

* **Connexion à la boîte de dialogue d’invitation d’utilisateur** : en mars, la fonctionnalité facultative existante « Connexion à la boîte de dialogue d’invitation d’utilisateur » sera abandonnée. La fonctionnalité « [!UICONTROL Se connecter dans la boîte de dialogue d’invitation d’utilisateur] » est remplacée par la fonctionnalité d’ID universel, requise pour la prochaine intégration du système Adobe Identity Management et activée en août 2021 sur tous les abonnements. Suite à l’obsolescence, Marketo Engage n’obligera qu’un seul utilisateur à être associé par adresse e-mail dans un abonnement.

**Domaines Marketo Engage - Configuration [!DNL Sales Insight]** : pour les domaines Marketo Engage pour lesquels le certificat SSL n&#39;est pas configuré et pour https://, les appels échouent avec une erreur de négociation SSL. Par conséquent, ces domaines vont disparaître. Par conséquent, les utilisateurs [!DNL Sales Insight] disposant d’une configuration plus ancienne pointant vers l’un de ces domaines peuvent rencontrer des erreurs de légende système sur leur page Lead, Contact, Compte, Panneaux d’opportunité ou Page globale Marketo. Nous vous recommandons de mettre à jour votre configuration [Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) dans [!DNL Salesforce] si vous rencontrez cette erreur. Il vous suffit de mettre à jour les informations d’identification Marketo Engage mises en surbrillance dans la section « Configuration [!DNL Marketo Sales Insight] » du document.

**_Webinaire de mise à jour du produit_**

[Webinaire De Mise À Jour De Marketo Engage De Janvier 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
