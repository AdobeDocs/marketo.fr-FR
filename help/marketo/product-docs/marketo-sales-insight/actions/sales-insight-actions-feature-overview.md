---
description: Présentation des actions Sales Insight - Documents Marketo - Documentation du produit
title: Présentation de la fonction Actions d’aperçu des ventes
exl-id: 059de248-d1a2-42cd-a7ec-f10b15d0b526
feature: Sales Insight Actions
source-git-commit: 1f228323c18204149630a7cb77d6ae0a88b425e3
workflow-type: tm+mt
source-wordcount: '1361'
ht-degree: 1%

---

# Présentation de la fonction Actions d’aperçu des ventes {#msi-actions-feature-overview}

Accélérez les efforts de prospection grâce à des outils d’intelligence et d’engagement optimisés par le marketing au sein d’un seul workflow à l’aide des actions Sales Insight.

>[!NOTE]
>
>Marketo Sales Insight Actions est une application web qui s’intègre exclusivement au CRM Salesforce via le [ package Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. On parle parfois de &quot;ventes Marketo&quot; ou simplement de &quot;actions&quot;.

Pour une présentation vidéo des actions Sales Insight, [cliquez ici](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/sales-insight-actions/overview.html){target="_blank"}.

![](assets/sales-insight-actions-feature-overview-1.png)

## Disposition de piste et disposition de contact {#lead-layout-and-contact-layout}

Les actions suivantes sont disponibles dans la liste déroulante &quot;Choisir les actions&quot; dans le volet de navigation supérieur :

* Envoyer un e-mail de vente
   * Les emails de vente ont un suivi des affichages, des clics et des réponses (lorsque le canal de diffusion est configuré)
   * Inclut le Personalization par courrier électronique, la signature personnalisée et les pièces jointes
   * Partage de modèles et rapports
   * Partage d’équipe, e-mails de groupe et fonctionnalité CC/Cci
   * L’activité de courrier électronique de vente sera enregistrée dans l’enregistrement de personne Marketo.
   * Filtres et déclencheurs correspondants dans les campagnes dynamiques Marketo (détails ci-dessous)

* Ajouter à la campagne de ventes
   * Ajout de pistes aux classeurs de ventes, qui est une séquence d’emails et de tâches
   * Inclut l’accès et le partage de l’équipe, la génération de tâches, les week-ends de saut, l’exclusion des emails OO comme réponses et la fin automatique.
   * L’activité de campagne sera enregistrée dans l’enregistrement de personne Marketo.
   * Filtres et déclencheurs correspondants dans les campagnes dynamiques Marketo (détails ci-dessous)

* Dialecte de ventes
   * Lancer des appels de vente à l’aide de la boîte de dialogue dans le CRM
   * Inclut la présence locale, pré-enregistrée
   * Consigner le résultat de l’appel, l’enregistrement des appels dans le panneau et l’historique des activités
   * L’activité d’appel sera consignée dans l’enregistrement de personne Marketo.
   * Filtres et déclencheurs dans les campagnes dynamiques Marketo

* Ajouter une tâche
   * Créer des tâches par courrier électronique, d’appel, InMail et personnalisées pour vos pistes
   * Automatiser la création de tâches avec les campagnes commerciales
   * Synchronisation des tâches avec Salesforce
   * Enregistrer les tâches dans la section Historique des activités Salesforce

Vous pouvez accéder au flux en direct en cliquant sur l’icône ((0)) dans le volet de navigation supérieur. Il permet d’afficher les mises à jour en direct des activités de vente, ainsi que la fonction d’ancrage des écrans.

![](assets/sales-insight-actions-feature-overview-2.png)

Les données suivantes sont disponibles dans les onglets du panneau MSI :

* Tableau de bord des statistiques
   * La grille de vitesse d’engagement comprend des activités provenant des e-mails de vente, des actions de campagne de vente et de la boîte de dialogue de vente.
   * Campagnes de vente à venir : lorsqu’un prospect fait partie d’une campagne en cours, ces informations seront disponibles dans l’onglet Campagnes de vente à venir.
   * Tâches à venir : lorsqu’une tâche à venir se rapporte à un prospect, ces informations seront disponibles dans l’onglet Tâches à venir.

* Onglet Email
   * Tous les courriers électroniques de vente envoyés seront consignés ici. Les activités seront également consignées dans l’enregistrement de personne Marketo.
   * Les colonnes incluent Objet, Ouvrir, Clic, Répondre (disponible uniquement pour les emails de vente avec configuration du canal de diffusion), Expéditeur, Date
   * Inclut une carte déroulante avec des détails supplémentaires tels que l’expéditeur, le modèle, la campagne de ventes et l’aperçu du courrier électronique.

* Onglet Appel
   * Tous les appels placés à l’aide de la fonction de boîte de dialogue de vente seront consignés ici. Les activités seront également consignées dans l’enregistrement de personne Marketo.
   * Les colonnes comprennent le nom, le résultat, les notes, l’appel à, la durée et le lien vers l’enregistrement.
   * Inclut une carte déroulante avec des détails supplémentaires tels que Appel effectué par, Appel répondu par, Numéro de téléphone et État

## Disposition du compte et des opportunités {#account-and-opportunity-layout}

Les actions suivantes sont disponibles dans le volet de navigation supérieur :

* Envoyer un e-mail de vente : possibilité d’envoyer des e-mails de groupe personnalisés ou modélisés avec un suivi des vues, des clics et des réponses à tous les contacts associés à un compte/une opportunité.
   * Les emails de vente ont un suivi des affichages, des clics et des réponses (lorsque le canal de diffusion est configuré)
   * Inclut le Personalization par courrier électronique, la signature personnalisée et les pièces jointes
   * Partage de modèles et rapports
   * Partage d’équipe, e-mails de groupe et fonctionnalité CC/Cci
   * L’activité de courrier électronique de vente sera enregistrée dans l’enregistrement de personne Marketo.
   * Filtres et déclencheurs correspondants dans les campagnes dynamiques Marketo (détails ci-dessous)

* Ajouter à la campagne de ventes : ajoutez tous les contacts associés à un compte/une opportunité aux classeurs de ventes qui est une séquence d’emails et de tâches.
   * Ajout de pistes aux classeurs de ventes, qui est une séquence d’emails et de tâches
   * Inclut l’accès et le partage de l’équipe, la génération de tâches, les week-ends de saut, l’exclusion des emails OO comme réponses et la fin automatique.
   * L’activité de campagne sera enregistrée dans l’enregistrement de personne Marketo.
   * Filtres et déclencheurs correspondants dans les campagnes dynamiques Marketo (détails ci-dessous)

Vous pouvez accéder au flux en direct en cliquant sur l’icône ((0)) dans le volet de navigation supérieur. Il permet d’afficher les mises à jour en direct des activités de vente, ainsi que la fonction d’ancrage des écrans.

Les données suivantes sont disponibles dans les onglets :

* Tableau de bord des statistiques
   * La grille de vitesse d’engagement comprend les activités des e-mails de vente, des actions de campagne de vente et du dialecte de vente.
   * Campagnes de vente à venir : lorsqu’un contact du compte/de l’opportunité fait partie d’une campagne en cours, ces informations seront disponibles dans l’onglet Campagnes de vente à venir.
   * Tâches à venir : lorsqu’il y a une tâche à venir concernant un contact du compte/de l’opportunité, ces informations seront disponibles dans l’onglet Tâches à venir.

* Onglet Email
   * Tous les emails de vente envoyés aux contacts du compte/de l’opportunité seront consignés ici. Les activités seront également consignées dans l’enregistrement de personne Marketo.
   * Les colonnes comprennent Objet, Ouverture, Clic, Réponse (disponible uniquement pour les emails de vente avec configuration du canal de diffusion), Expéditeur et Date.
   * Inclut une carte déroulante avec des détails supplémentaires tels que l’expéditeur, le modèle, la campagne de ventes et l’aperçu du courrier électronique.

* Onglet Appel
   * Tous les appels effectués aux contacts du compte/de l’opportunité à l’aide de la fonction de boîte de dialogue de vente seront consignés ici. Les activités seront également consignées dans l’enregistrement de personne Marketo.
   * Les colonnes incluent le nom, le résultat, les notes, le statut appelé, la durée et le lien vers l’enregistrement.
   * Inclut une carte déroulante avec des détails supplémentaires tels que Appel effectué par, Appel répondu par, Numéro de téléphone et État

## Mode Liste des pistes et des contacts (actions en bloc) {#lead-and-contact-list-view}

* Envoyer un email de vente : possibilité d’envoyer des emails personnalisés ou modélisés avec un suivi des vues, des clics et des réponses à une liste de contacts/prospects.
* Envoyer une campagne de ventes : ajoutez aux classeurs de ventes une séquence d’emails et de tâches à une liste de contacts/de prospects.

## Onglet global Marketo {#marketo-global-tab}

**Onglet Meilleurs billets**

![](assets/sales-insight-actions-feature-overview-3.png)

Les actions en bloc suivantes sont disponibles dans la liste déroulante de l’onglet Meilleurs paris :

* Envoyer un e-mail de vente : possibilité d’envoyer des e-mails personnalisés ou modélisés avec suivi des affichages, clics et réponses.
* Envoyer la campagne de ventes : ajoutez des pistes aux classeurs de ventes qui est une séquence d’emails et de tâches.

  ![](assets/sales-insight-actions-feature-overview-4.png)

Les actions en ligne suivantes sont disponibles pour les pistes/contacts individuels dans l’onglet Meilleurs paris :

* Envoyer un e-mail de vente : possibilité d’envoyer des e-mails personnalisés ou modélisés avec suivi des affichages, clics et réponses.
* Envoyer la campagne de ventes : ajoutez des pistes aux classeurs de ventes qui est une séquence d’emails et de tâches.
* Dialeur de ventes : effectuez des appels de vente à l’aide de la boîte de dialogue dans le CRM.
* Ajouter une tâche : créez des tâches de courrier électronique, d’appel, de client ou de liaison pour les prospects.

  ![](assets/sales-insight-actions-feature-overview-5.png)

**Onglet Email**

* Tous les courriers électroniques de vente envoyés seront consignés ici. Les activités seront également consignées dans l’enregistrement de personne Marketo.
* Les colonnes comprennent Objet, Ouverture, Clic, Réponse (disponible uniquement pour les emails de vente avec configuration du canal de diffusion), Expéditeur et Date.
* Inclut une carte déroulante avec des détails supplémentaires tels que l’expéditeur, le modèle, la campagne de ventes et l’aperçu du courrier électronique.

**Onglet Appel**

* Tous les appels placés à l’aide de la fonction de boîte de dialogue de vente seront consignés ici. Les activités seront également consignées dans l’enregistrement de personne Marketo.
* Les colonnes incluent le nom, le résultat, les notes, le statut appelé, la durée et le lien vers l’enregistrement.
* Inclut une carte déroulante avec des détails supplémentaires tels que Appel effectué par, Appel répondu par, Numéro de téléphone et État

**Onglet Tâche**

* Les tâches email, d’appel, InMail et personnalisées créées et terminées seront disponibles pour la gestion des tâches dans cet onglet. Possibilité d’ajouter une tâche
* Automatiser la création de tâches avec les campagnes commerciales
* Synchronisation des tâches avec Salesforce
* Enregistrer les tâches dans la section Historique des activités Salesforce

  ![](assets/sales-insight-actions-feature-overview-6.png)

**Flux actif**

* Possibilité d’afficher les mises à jour en direct sur les activités de vente, ainsi que la fonctionnalité d’ancrage d’écran
* Les boutons Incorporer email, appel et cadence permettent à chaque client de disposer d’informations exploitables.

## Fonctionnalités disponibles dans Marketo {#features-available-in-marketo}

Activités commerciales capturées dans Marketo :

* Envoyer un courrier électronique de vente : l’utilisateur a envoyé un courrier électronique de vente à un prospect.
* Ouverture d’un courrier électronique de vente : un prospect a ouvert un courrier électronique de vente envoyé
* Clic sur le courrier électronique de vente : le prospect a cliqué sur un lien dans un courrier électronique de vente
* Courrier électronique de vente répondu : le prospect a répondu à un courrier électronique de vente.
* Recevoir l’appel de vente : le prospect a reçu un appel d’un vendeur à l’aide du dialecte de ventes.
* Ajouter à la campagne de ventes : le prospect a été ajouté à la campagne de vente créée.
* Supprimé de la campagne de ventes : le prospect a été supprimé d’une campagne de vente créée.

Les filtres et déclencheurs incluent :

* Envoyer un e-mail de vente
* E-mail de vente ouvert
* Courrier électronique de vente cliqué
* A répondu à l&#39;e-mail commercial
* Appel de vente reçu
* Ajout à la campagne de ventes
* Supprimé de la campagne SFDC

  ![](assets/sales-insight-actions-feature-overview-7.png)
