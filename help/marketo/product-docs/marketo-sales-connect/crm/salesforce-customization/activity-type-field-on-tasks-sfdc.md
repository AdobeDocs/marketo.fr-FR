---
unique-page-id: 14352476
description: Champ Type d’activité sur les tâches (SFDC) - Documents Marketo - Documentation du produit
title: Champ Type d’activité sur les tâches (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Champ Type d’activité sur les tâches (SFDC) {#activity-type-field-on-tasks-sfdc}

Avec l’aide de Sales Connect, vous pouvez enregistrer vos emails et vos appels en tant qu’activité dans Salesforce. L’un des éléments essentiels pour disposer de données importantes dans Salesforce est de faire renseigner la valeur correcte dans le champ Type.

>[!NOTE]
>
>La journalisation des emails via Cci ne se tourne pas vers la liste de sélection Type de tâche et remplit automatiquement le champ Type en tant qu’&quot;email&quot; puisqu’ils sont envoyés à Salesforce par l’intermédiaire de votre adresse en Cci.

## Exigences {#requirements}

* Connexion à Salesforce
* Aucune valeur Type par défaut sélectionnée dans le sélecteur Type de tâche
* L’appel, la réponse et l’e-mail doivent tous exister sous la liste de sélection Type de tâche (ce qui est important en termes de casse).
* Pas de workflows ou de déclencheurs qui agissent sur la valeur du champ Type

## Configuration {#setup}

Vérifiez d’abord que les valeurs correctes de liste de sélection sont en place. Vous aurez besoin de l’aide de votre administrateur Salesforce pour apporter des modifications à votre liste de sélection.

1. Accédez à [Salesforce.com](https://salesforce.com) et cliquez sur Configuration dans le coin supérieur droit.
1. Cliquez sur Personnaliser.
1. Cliquez sur Activités.
1. Cliquez sur Champs de la tâche.
1. Cliquez sur Type.
1. Vous vous trouvez maintenant sur la liste de sélection du type de tâche. Assurez-vous qu’aucun paramètre &quot;Par défaut&quot; n’est sélectionné.
1. Assurez-vous qu’une valeur Type est répertoriée pour Email, Call et Reply.

Maintenant que ce paramètre est en place, le champ Type commence à renseigner la valeur correspondante pour les emails, les appels et les réponses consignés. Ces valeurs seront _not_ renseignées dans les tâches de rappel de Sales Connect.

>[!NOTE]
>
>Si vous ne voyez pas &quot;Répondre&quot; comme valeur, ajoutez-la en cliquant sur **Nouveau**. &quot;Reply&quot; n’est pas une valeur standard dans Salesforce.
