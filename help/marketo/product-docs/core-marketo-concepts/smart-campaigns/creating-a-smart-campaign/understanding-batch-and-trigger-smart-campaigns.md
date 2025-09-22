---
unique-page-id: 2953132
description: Présentation des campagnes intelligentes par lots et de déclenchement - Documents Marketo - Documentation du produit
title: Présentation des campagnes intelligentes par lots et à déclencheur
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 6%

---

# Présentation des campagnes intelligentes par lots et à déclencheur {#understanding-batch-and-trigger-smart-campaigns}

Il existe deux types de campagnes intelligentes : Lot et Déclencheur.

## Campagne par lot {#batch-campaign}

>[!NOTE]
>
>**Définition**
>
>Une campagne par lots se lance à une heure spécifique et affecte simultanément un ensemble spécifique de personnes. Par exemple, l’envoi d’un e-mail à toutes les personnes en Californie.

Les campagnes par lots n’auront que des filtres dans la section de liste dynamique (c’est-à-dire aucun déclencheur).

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

Cliquez sur l’onglet **[!UICONTROL Planning]** pour confirmer que la campagne intelligente est définie sur « Lot ».

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**Campagnes intelligentes par lots**

* Peut être planifié pour des périodicités, telles que quotidiennes, hebdomadaires et mensuelles. Vous pouvez également les faire exécuter une seule fois.
* Sont visibles dans la [vue de planning du programme](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md){target="_blank"}. Tout ce qui suit une étape « Attente » dans la campagne intelligente ne sera pas inclus dans la vue.

<br> 

## Campagne à déclencheur {#trigger-campaign}

>[!NOTE]
>
>**Définition**
>
>Une campagne Trigger affecte une personne à la fois en fonction d’un événement déclenché. Un exemple de déclencheur serait de cliquer sur un lien dans un e-mail.

Si une campagne dynamique utilise au moins un déclencheur dans la section Liste dynamique , le mode est automatiquement défini sur Déclenché.

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

Cliquez sur l’onglet **[!UICONTROL Planning]** pour confirmer que la campagne intelligente est définie sur « Déclenchée ».

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**Déclencher des campagnes**

* Ne peut pas être planifié pour des récurrences. Ils peuvent uniquement être définis sur actif ou inactif.
* Vous pouvez définir plusieurs déclencheurs. Cependant, si un déclencheur est déclenché, les actions de campagne s’exécutent.

>[!TIP]
>
>Utilisez le [journal d’activité](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"} pour voir ce qui s’est produit étape par étape dans vos campagnes intelligentes. Le journal des activités se trouve dans le dernier onglet de la page des détails d’une personne.
