---
title: compréhension-batch-et-trigger-smart-campaigns
description: Présentation des campagnes dynamiques par lot et déclencheur
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Présentation des campagnes dynamiques par lot et déclencheur

<br> 

Il existe deux types de campagnes intelligentes : Lot et Déclencheur.

## Campaign Batch Smart

Une campagne par lot démarre à un moment donné et affecte un groupe de personnes en même temps. Par exemple, vous pouvez envoyer un courriel à toutes les personnes de votre base de données qui vivent en Californie.

Les campagnes dynamiques par lot ne comportent que des filtres dans la section des listes dynamiques (c’est-à-dire qu’aucun déclencheur).

![Image un](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

Cliquez sur l&#39;onglet **[!UICONTROL Planification]** pour confirmer que la campagne dynamique est définie sur &quot;Lot&quot;.

![Image 2](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**Batch Smart Campaigns**

* Peut être planifié pour des récurrences, telles que quotidiennes, hebdomadaires et mensuelles. Vous pouvez également les faire exécuter une seule fois.
* Sont visibles sur la [vue de Planning du programme](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View).
* Tout ce qui suit une étape &quot;Attente&quot; dans la campagne intelligente ne sera pas inclus dans la vue.

## Trigger Smart Campaign

Une campagne intelligente de déclenchement affecte une personne à la fois en fonction d’un événement déclenché. Un exemple de déclencheur consiste à cliquer sur un lien dans un courrier électronique.

Si une campagne intelligente utilise au moins un déclencheur dans la section liste intelligente, le mode est automatiquement défini sur déclenché.

![Image trois](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

Cliquez sur l&#39;onglet **[!UICONTROL Planification]** pour confirmer que la campagne dynamique est définie sur &quot;Déclencheur&quot;.

![Image 4](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**Déclencher des campagnes dynamiques**

* Impossible de planifier les répétitions. Ils ne peuvent être définis que sur principal ou inactif.
* Vous pouvez définir plusieurs déclencheurs. Cependant, si _un déclencheur_ est déclenché, les actions de campagne s&#39;exécuteront.

>[!TIP]
>
>Utilisez le [journal des activités](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person) pour déterminer ce qui s&#39;est passé pas à pas dans vos campagnes dynamiques. Le journal des activités se trouve dans le dernier onglet de la page des détails d’une personne.
