---
unique-page-id: 3571848
description: Synchronisation de Microsoft Dynamics - Synchronisation des leads - Documents Marketo - Documentation du produit
title: Synchronisation Microsoft Dynamics - Synchronisation des leads
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Synchronisation des [!DNL Microsoft Dynamics] : synchronisation des leads {#microsoft-dynamics-sync-lead-sync}

La synchronisation de Marketo vers [!DNL Dynamics] est très puissante. Voici les détails :

## Comment les détails sont-ils synchronisés entre les deux systèmes ? {#how-are-details-kept-in-sync-between-the-two-systems}

La synchronisation est bidirectionnelle. Si vous apportez des modifications à un prospect dans [!DNL Dynamics] ou à une personne dans Marketo, vos mises à jour seront répercutées sur les deux systèmes.

>[!NOTE]
>
>Les suppressions ne se synchronisent pas toujours automatiquement dans les deux sens. Voir [Suppression d’un prospect ou d’un contact](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}.

## Que faire si des modifications sont apportées simultanément au même champ dans les deux systèmes ? (Collision de données) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Bien que cela soit rare, Marketo gagnera pour les personnes (prospects) et [!DNL Dynamics] gagnera pour les contacts. En effet, nous considérons que le service marketing fait autorité pour les personnes, alors que le système officiel d’enregistrement des contacts se trouve dans le service des ventes (CRM).

## Puis-je créer un prospect dans [!DNL Dynamics] à l’aide de Marketo ? {#can-i-create-a-lead-in-dynamics-using-marketo}

Oui, utiliser l’action de flux [[!UICONTROL &#x200B; Synchroniser la personne avec Microsoft &#x200B;]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md). Cette opération crée un prospect dans [!DNL Dynamics] si le prospect n’existe pas. Si le prospect existe, l’étape de flux n’effectue aucune action.

>[!NOTE]
>
>Lors de l’utilisation de l’action de flux « [!UICONTROL &#x200B; Synchroniser la personne avec Microsoft &#x200B;] » (dans une campagne de déclenchement uniquement), le prospect/contact est créé en temps réel dans [!DNL Dynamics].

## Puis-je forcer manuellement la synchronisation d’une personne de Marketo avec un prospect dans [!DNL Dynamics] ? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Non, la synchronisation en arrière-plan automatisée est la seule façon de synchroniser les mises à jour entre Marketo et [!DNL Dynamics]. L’action de flux [[!UICONTROL &#x200B; Synchroniser la personne avec Microsoft &#x200B;]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) ne force pas la synchronisation du prospect.

## Quels champs vont être synchronisés avec Marketo ? {#what-fields-will-sync-to-marketo}

Vous pouvez [sélectionner les champs à synchroniser](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} lors de la configuration.

## Marketo respectera-t-il les règles de validation [!DNL Dynamics] ? {#will-marketo-respect-the-dynamics-validation-rules}

Oui. La synchronisation échoue si le format de données est incorrect ou s’il manque des informations de champ requises. Si cela se produit, Marketo consigne les résultats dans le journal d’activité de la personne.
