---
unique-page-id: 3571848
description: Microsoft Dynamics Sync -Sync - Synchronisation des pistes - Documents marketing - Documentation du produit
title: Microsoft Dynamics Sync - Sync piste
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---


# Microsoft Dynamics Sync : Synchronisation des pistes {#microsoft-dynamics-sync-lead-sync}

Marketo to Dynamics sync est très puissant. Voici les détails :

## Comment les détails sont-ils synchronisés entre les deux systèmes ? {#how-are-details-kept-in-sync-between-the-two-systems}

La synchronisation est bidirectionnelle. Si vous apportez des modifications à une piste dans Dynamics ou à une personne dans Marketo, votre mise à jour sera répercutée dans les deux systèmes.

>[!NOTE]
>
>Les suppressions ne sont pas toujours synchronisées automatiquement dans les deux directions. Voir [Suppression d&#39;une piste ou d&#39;un contact](http://docs.marketo.com/x/agO1Ag).

## Que se passe-t-il si des modifications sont apportées au même champ dans les deux systèmes en même temps ? (Collision de données) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Bien que cela soit rare, Marketo gagnera pour les gens (pistes) et Dynamics gagnera pour les contacts. Cela est dû au fait que nous considérons le service marketing comme faisant autorité pour les gens, alors que le système officiel d&#39;enregistrement des contacts se trouve dans le service des ventes (CRM).

## Puis-je créer un prospect dans Dynamics à l&#39;aide de Marketo ? {#can-i-create-a-lead-in-dynamics-using-marketo}

Oui, utilisez l&#39;action de flux [Synchroniser la personne avec Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) . Cela créera une piste dans Dynamics si elle n&#39;existe pas. Si la piste existe, l&#39;étape de flux n&#39;effectue aucune action.

>[!NOTE]
>
>Lors de l&#39;utilisation de l&#39;action de flux &quot;Synchroniser la personne avec Microsoft&quot; (dans une campagne de déclenchement uniquement), le prospect/contact est créé en temps réel dans Dynamics.

## Puis-je forcer manuellement la synchronisation d&#39;une personne de Marketo vers une piste dans Dynamics ? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Non, la synchronisation en arrière-plan automatisée est le seul moyen de synchroniser les mises à jour entre Marketing et Dynamics. L&#39;action de flux [Synchroniser la personne avec Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) ne forcera pas la synchronisation du prospect.

## Quels champs seront synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) lors de la configuration.

## Marketo respectera-t-il les règles de validation Dynamics ? {#will-marketo-respect-the-dynamics-validation-rules}

Oui. La synchronisation échoue si le format des données est incorrect ou si les informations de champ requises sont manquantes. Marketo consigne le résultat dans le journal des Activités de la personne si cela se produit.

