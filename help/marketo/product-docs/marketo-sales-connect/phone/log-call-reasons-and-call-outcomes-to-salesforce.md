---
description: Enregistrer les motifs des appels et les résultats des appels dans Salesforce - Documents Marketo - Documentation du produit
title: Enregistrer les motifs des appels et les résultats des appels dans Salesforce
hide: true
hidefromtoc: true
source-git-commit: 1dd4a4f6bfac0b101f85f3776396aeef1a1f7182
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Enregistrer les motifs des appels et les résultats des appels dans Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Si vous souhaitez consigner les résultats des appels et les raisons des appels à Salesforce à des fins de reporting ou de visibilité, vous pouvez créer un champ d’activité personnalisé pour chacun d’eux. Chaque champ doit utiliser un nom d’API spécifique.

* Nom de l’API des résultats de l’appel : mktosales_call_result
* Nom de l’API des raisons d’appeler : mktosales_call_reason

Pour utiliser ces champs, vous devez d’abord créer le champ en tant que champ d’activité personnalisé. Pour le rendre visible par les utilisateurs, vous devez l’ajouter à la mise en page de la page de l’objet de tâche.

## Créer un champ d’activité personnalisé dans Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. Dans Salesforce, accédez à Configuration.

PICC

1. Saisissez &quot;Activités&quot; dans la zone Recherche rapide .

PICC

1. Cliquez sur **Champs personnalisés d’une activité**.

PICC

1. Cliquez sur **Nouveau**.

PICC

## Créer un champ d’activité personnalisé dans Salesforce Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. Dans Salesforce, cliquez sur l’icône d’engrenage en haut à droite.

PICC

1. Cliquez sur **Configuration**.

PICC

1. Cliquez sur **Object Manager**.

PICC

1. Saisissez Activité dans la zone Recherche rapide , puis cliquez sur le libellé Activité pour ouvrir la configuration de l’objet.

PICC

1. Sur le côté gauche, cliquez sur **Champs et relations**.

PICC

1. Cliquez sur **Nouveau**.

PICC

## Ajout d’un champ d’activité personnalisé à la disposition de la page de tâche dans Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

ÉTAPES

## Ajout d’un champ d’activité personnalisé à la disposition de la page de tâche dans Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

ÉTAPES

>[!MORELIKETHIS]
>
>[Installation des champs d’événement de connexion aux ventes dans l’historique des activités](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
