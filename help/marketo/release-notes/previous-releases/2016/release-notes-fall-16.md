---
unique-page-id: 11384018
description: Notes De Mise À Jour - Automne 16 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Automne 16
exl-id: da935951-162e-426c-acf2-12c55ff706b4
source-git-commit: 2b72932606a93d061eb2f57c0ff3256b94a0c20c
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 1%

---

# Notes De Mise À Jour : Automne 16 {#release-notes-fall}

Les fonctionnalités suivantes sont incluses dans la version de l’automne 16. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo. Cliquez sur les liens de titre pour afficher les articles détaillés de chaque fonctionnalité.

## [!UICONTROL Contenu prédictif] dans les e-mails {#predictive-content-in-email}

Notre application [!UICONTROL Contenu prédictif] offre une nouvelle expérience utilisateur permettant de suivre, de gérer et de recommander votre contenu par le biais de notre machine learning et de nos algorithmes prédictifs sur les canaux web et e-mail.

>[!NOTE]
>
>Tous les clients disposant du module Prédictive seront activés d’ici le 10 janvier.

![](assets/shafe.png)

Vous pouvez désormais ajouter du contenu prédictif à votre e-mail. Lorsque l’e-mail est ouvert, le destinataire reçoit automatiquement le contenu pertinent et recommandé qui permet d’augmenter l’engagement et les conversions de contenu.

![](assets/predictive.png)

## [Conversions hors ligne Facebook ](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

Grâce à [!DNL Facebook]’intégration des conversions hors ligne, les données de conversion dans Marketo (pour les leads publicitaires) sont automatiquement renvoyées à [!DNL Facebook] afin que votre équipe publicitaire puisse mieux optimiser ses dépenses publicitaires. Dans ce rapport [!DNL Facebook] Ad Manager, les conversions hors ligne sont mises en surbrillance.

![](assets/facebook.png)

## [ID universel](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

Un identifiant universel vous permet d’accéder à plusieurs abonnements Marketo avec une seule connexion et de passer rapidement d’un abonnement à l’autre. Vous pouvez utiliser un seul profil de communauté pour tous vos abonnements.

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>Veuillez contacter le support technique de Marketo pour activer cette fonctionnalité.

## Améliorations marketing basées sur les comptes Marketo {#marketo-account-based-marketing-enhancements}

Désormais, vous pouvez affecter des équipes de compte à des comptes nommés dans Account Based Marketing (ABM), par exemple, le propriétaire du compte, le représentant du développement des ventes, le représentant du développement commercial et le responsable du succès client. Vous pouvez également créer des listes de comptes spécifiques au propriétaire du compte et envoyer des rapports hebdomadaires personnalisés sur ABM à l’équipe du compte.

![](assets/account-team-11-15-16.png)

**API REST**

Cette version vous permet également de gérer les attributs de compte nommés et les scores de compte dans AEM à l’aide de l’API REST Marketo. Pour plus d’informations sur les opérations de l’API, consultez le [site web du développeur de Marketo](https://developers.marketo.com/rest-api/lead-database/named-accounts).

## [Améliorations du journal d’audit](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

Le journal d&#39;audit fournit un historique complet des modifications apportées à votre abonnement Marketo. Nous avons ajouté des fonctionnalités de suivi supplémentaires pour les programmes et nous avons fait apparaître les détails des modifications importantes pour les campagnes intelligentes, les listes intelligentes et les modifications apportées aux utilisateurs et aux rôles.

## Nouvelles autorisations

**Rendre l’e-mail opérationnel**

L’époque où vous deviez vous inquiéter des utilisateurs qui envoyaient des e-mails transactionnels à des personnes de votre base de données qui s’étaient désabonnées est révolue. Vous pouvez désormais spécifier quels utilisateurs peuvent rendre un e-mail opérationnel ou modifier les e-mails opérationnels.

**Modifier les restrictions de campagne**

Pourquoi définir des [restrictions de campagne](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) si vous ne pouvez pas les appliquer ? Lorsque vous définissez les Paramètres des limites de campagne pour limiter le nombre de personnes de votre base de données qui peuvent être ciblées avec une seule campagne, vous avez désormais la possibilité de limiter les utilisateurs qui peuvent remplacer ces paramètres lors de la planification d’une campagne.

## [Son pour les notifications push mobiles](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

Donnez plus de richesse à votre notification push iOS en activant le son. Cette nouvelle fonctionnalité vous permet de déclencher un son lorsque la notification push s’affiche sur l’appareil mobile.

>[!NOTE]
>
>* Les propriétaires d’appareils peuvent choisir d’empêcher la lecture de sons dans les paramètres de l’appareil et les développeurs d’applications peuvent donner aux propriétaires d’appareils des options dans l’application pour empêcher la lecture de sons.
>* Les sons sont automatiquement émis lorsqu’une notification push est affichée sur un appareil Android.

![](assets/sound-for-push-notifications.png)

## [Ventes Insight compatibles avec le chiffrement Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

Market [!DNL Sales Insight] est désormais compatible avec le chiffrement [!DNL Salesforce] Shield. Tous les clients [!DNL Sales Insight] doivent effectuer une mise à niveau vers ce dernier package géré (version 1.4359.2), [disponible sur le [!DNL Appexchange]](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO).

## [API de comptes nommés](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

Avec cette version, les utilisateurs de Marketo ABM peuvent gérer les comptes nommés via l’API des comptes nommés. Les utilisateurs peuvent créer, mettre à jour et supprimer des comptes nommés, ainsi que lire et mettre à jour les scores des comptes nommés ABM.

## [Prise en charge de l’API de l’éditeur d’e-mail v2.0](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

Gérez les variables et les modules pour les e-mails au format v2.0 à l’aide de l’API REST Marketo.

## [Modifications apportées à la synchronisation de Marketo Salesforce](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

L’intégration de Marketo [!DNL Salesforce] évolue pour améliorer la manière dont les champs Marketo sont synchronisés avec [!DNL Salesforce]. Désormais, au lieu d’avoir à synchroniser un grand groupe de champs dont vous avez besoin ou non, vous pouvez choisir les champs que vous souhaitez inclure. Consultez notre documentation ici pour plus d’informations : [https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840).
