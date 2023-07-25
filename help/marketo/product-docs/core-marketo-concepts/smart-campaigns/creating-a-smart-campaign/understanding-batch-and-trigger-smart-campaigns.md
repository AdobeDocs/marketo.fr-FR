---
unique-page-id: 2953132
description: Présentation des campagnes dynamiques par lots et par déclenchement - Documents Marketo - Documentation du produit
title: Présentation des campagnes dynamiques par lots et par déclenchement
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Présentation des campagnes dynamiques par lots et par déclenchement {#understanding-batch-and-trigger-smart-campaigns}

Il existe deux types de campagnes intelligentes : Lot et Déclencheur.

## Campagne dynamique par lots {#batch-smart-campaign}

>[!NOTE]
>
>**Définition**
>
>Une campagne par lots démarre à un moment spécifique et affecte un groupe spécifique de personnes à la fois. Un exemple serait d&#39;envoyer un email à toutes les personnes en Californie.

Les campagnes dynamiques par lots ne comportent que des filtres dans la section Liste dynamique (c’est-à-dire, aucun déclencheur).

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

Cliquez sur le **Planification** confirme que la campagne dynamique est définie sur &quot;Lot&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**Campagnes dynamiques par lots**

* Peuvent être planifiées pour des récurrences, telles que quotidiennes, hebdomadaires et mensuelles. Vous pouvez également les faire exécuter une seule fois.
* sont visibles dans la variable [vue planning du programme](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). Tout ce qui suit une étape &quot;Attente&quot; dans la campagne dynamique ne sera pas inclus dans la vue.

<br> 

## Déclencher une campagne dynamique {#trigger-smart-campaign}

>[!NOTE]
>
>**Définition**
>
>Une campagne dynamique de déclenchement affecte une personne à la fois en fonction d’un événement déclenché. Un exemple de déclencheur consiste à cliquer sur un lien dans un email.

Si une campagne dynamique utilise au moins un déclencheur dans la section de liste dynamique, le mode est automatiquement défini sur déclenché.

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

Cliquez sur le bouton **Planification** confirme que la campagne dynamique est définie sur &quot;Déclenché&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**Déclenchement de campagnes dynamiques**

* Ne peut pas être planifié pour les récurrences. Ils ne peuvent être définis que sur principal ou inactif.
* Vous pouvez définir plusieurs déclencheurs. Toutefois, si un déclencheur est déclenché, les actions de campagne s’exécutent.

>[!TIP]
>
>Utilisez la variable [journal des activités](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) pour voir ce qui s’est produit étape par étape dans vos campagnes intelligentes. Le journal des activités se trouve dans le dernier onglet de la page des détails d’une personne.
