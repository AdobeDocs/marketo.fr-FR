---
unique-page-id: 14352476
description: Champ de type d’Activité sur les Tâches (SFDC) - Documents marketing - Documentation du produit
title: Champ Type d’Activité sur les Tâches (SFDC)
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Champ Type d&#39;Activité sur les Tâches (SFDC) {#activity-type-field-on-tasks-sfdc}

Avec l&#39;aide de Sales Connect, vous pouvez enregistrer vos e-mails et appels en tant qu&#39;activité dans Salesforce. Pour disposer de données importantes dans Salesforce, il est essentiel que le champ Type renseigne la valeur correcte.

>[!NOTE]
>
>La consignation des courriers électroniques via BCC ne se rapporte pas à la liste de sélection Type de Tâche et remplit automatiquement le champ Type en tant que &quot;courriel&quot; puisqu&#39;ils sont envoyés à Salesforce par l&#39;intermédiaire de votre adresse de carte de crédit client.

## Exigences {#requirements}

* Connexion à Salesforce
* Aucune valeur Type par défaut sélectionnée dans la liste de sélection Type de Tâche
* Les appels, réponses et courriers électroniques doivent tous exister sous la liste de sélection Type de Tâche (les questions de mise en majuscule sont importantes).
* Aucune action `Workflows` ou `Triggers` sur la valeur du champ Type

## Configuration {#setup}

Vérifiez d’abord que les valeurs de liste de sélection sont correctes. Vous aurez besoin de l&#39;aide de votre administrateur Salesforce pour apporter des modifications à votre liste de sélection.

1. Accédez à [Salesforce.com](http://Salesforce.com) et cliquez sur Configuration dans le coin supérieur droit.
1. Cliquez sur Personnaliser.
1. Cliquez sur Activités.
1. Cliquez sur Champs de Tâche.
1. Cliquez sur Type.
1. Vous vous trouvez maintenant sur la liste de sélection des types de Tâche. Assurez-vous qu’aucun paramètre par défaut n’est sélectionné.
1. Assurez-vous qu&#39;une valeur Type est répertoriée pour Courriel, Appel et Réponse.

Maintenant que ce champ est en place, vous allez commencer à voir le champ Type renseigner la valeur correspondante pour les courriers électroniques, les appels et les réponses enregistrés. Ces valeurs **not** seront renseignées dans les tâches de rappel de Sales Connect.

>[!NOTE]
>
>Si vous ne voyez pas &quot;Répondre&quot; comme valeur, ajoutez-le en cliquant sur **Nouveau**. &quot;Répondre&quot; n&#39;est pas une valeur standard dans Salesforce.
