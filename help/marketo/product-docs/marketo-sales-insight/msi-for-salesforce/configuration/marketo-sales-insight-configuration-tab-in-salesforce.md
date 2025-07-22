---
unique-page-id: 42762322
description: Onglet Configuration de Marketo Sales Insight dans Salesforce - Documents Marketo - Documentation du produit
title: Onglet Configuration de Marketo Sales Insight dans Salesforce
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---

# Onglet Configuration [!DNL Marketo Sales Insight] dans [!DNL Salesforce] {#marketo-sales-insight-configuration-tab-in-salesforce}

## Paramètres Opérationnels {#operational-settings}

Cette configuration est nécessaire pour commencer à utiliser [!DNL Sales Insight] dans SFDC.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI utilise à la fois les API Soap et REST
* La page Insight de ventes de votre compte Marketo comporte deux panneaux correspondants avec les informations d’identification d’API Soap et Rest que vous pouvez copier et coller ici
* Les API Soap et REST ont des délais d’expiration distincts que vous pouvez définir en fonction des besoins de votre entreprise. La durée maximale autorisée est de 120 secondes
* Désactivation du tableau de bord d’informations : vous pouvez supprimer les informations d’identification de l’API REST et utiliser uniquement l’API Soap. Cela désactive l’onglet Tableau de bord Insights dans tous vos panneaux MSI visualforce

## Configuration MSI {#msi-configuration}

Les configurations s&#39;appliquent à tous les utilisateurs de MSI et ne sont pas spécifiques aux profils.

**Paramètres de page Visualforce**

* Liste déroulante Activer l’action :
   * Possibilité de masquer l’e-mail Send Marketo dans la liste déroulante dans la disposition MSI du lead et du contact
   * Possibilité de masquer les options Ajouter à Marketo Campaign dans la liste déroulante dans la disposition MSI du lead et du contact
* Événements à venir : possibilité d’afficher les événements invités, tous les événements aux utilisateurs ou de masquer complètement cet onglet
* Campagnes à venir : possibilité d’afficher toutes les campagnes par e-mail ou de masquer complètement cet onglet
* Charger les campagnes et événements à venir : possibilité de réduire le nombre d’appels d’API REST effectués par les utilisateurs en plaçant l’onglet Événements et campagnes derrière un bouton « Charger les éléments à venir » à la demande
* Paramètres des onglets : les cinq onglets seront disponibles par défaut. Vous pouvez choisir l’ordre des onglets dans le panneau Ventes Insight. Le même ordre s’appliquera à toutes les mises en page (prospect, contact, compte, opportunité)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Onglet Global Marketo**

* Flux RSS activé : lorsqu’il est activé, les utilisateurs de MSI peuvent afficher leur flux de leads dans un flux RSS (en plus du flux de leads dans Salesforce). Le flux RSS ne peut fonctionner que si la fonction « Expiration du jeton » est désactivée. Ce paramètre est contrôlé dans la page Marketo Sales Insight Admin.
* Mode de débogage des meilleurs paris
* Masquer par défaut : l&#39;option que vous choisissez ici sera le nombre de jours pendant lesquels un meilleur pari sera masqué dans l&#39;onglet Meilleurs paris de Marketo lorsque vous cliquez sur l&#39;icône « Masquer »
* Champ Statut du contact : l’option que vous choisissez ici correspond à la valeur qui est renseignée dans la colonne En-tête du statut de l’onglet Meilleurs résultats de Marketo
* Paramètres des flux en direct : option permettant de choisir d’afficher uniquement le flux en direct (dans les panneaux Lead, Contact, Compte et Opportunité et la page Global Marketo), uniquement le flux en direct (dans la page Global Marketo) ou les deux flux en direct et en lead
* Paramètres des onglets : les cinq onglets seront disponibles par défaut. Vous pouvez choisir l’ordre des onglets dans la page Marketo Global

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**Limites**

* Activité (moment intéressant, activité web, e-mail) est définie sur 1 000 par défaut. Par défaut, les campagnes par e-mail et les événements sont définis sur 200
* Si vous constatez des problèmes de délai d’expiration dans votre organisation, vous pouvez réduire la limite

**Paramètres d’action**

* Envoyer un e-mail Marketo : cette activation donnera à tous les utilisateurs de Sales Insight l’accès pour envoyer des e-mails à partir des panneaux Lead, Contact, Compte, Opportunité et des Meilleurs résultats (actions en masse et engagement sur la ligne)
* Ajouter à Marketo Campaign : l’activation de cette option donnera à tous les utilisateurs de Sales Insight l’accès pour ajouter des campagnes à partir des panneaux Lead, Contact, Compte, Opportunité et de l’onglet Meilleurs résultats (actions en masse et engagement intégré)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## Paramètres de prise en charge {#support-settings}

Si vous cochez cette case, la journalisation du débogage sera activée dans votre instance Salesforce. Cela peut vous aider à résoudre les problèmes.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

## Réinitialiser Marketo Sales Insight {#reset-marketo-sales-insight}

Si vous choisissez de le faire, toutes vos configurations seront effacées dans SFDC et elles ne pourront pas être restaurées. Vous devrez tout reconfigurer.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-6.png)

>[!IMPORTANT]
>
>Ne cochez pas la case « Activer les actions MSI » à moins que vous n’utilisiez les fonctionnalités d’actions Sales Insights.

>[!MORELIKETHIS]
>
>[Ajouter un accès Sales Insight aux profils](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
