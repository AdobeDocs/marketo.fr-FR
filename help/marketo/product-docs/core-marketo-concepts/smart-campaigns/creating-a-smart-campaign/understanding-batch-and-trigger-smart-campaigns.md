---
unique-page-id: 2953132
description: Présentation des campagnes dynamiques par lot et déclencheur - Documentation sur le marketing - Documentation sur les produits
title: Présentation des campagnes dynamiques par lot et déclencheur
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---


# Présentation des campagnes dynamiques par lot et déclencheur {#understanding-batch-and-trigger-smart-campaigns}

Il existe deux types de campagnes intelligentes : Lot et Déclencheur.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Campaign Batch Smart {#batch-smart-campaign}

>[!NOTE]
>
>**Définition**
>
>Une campagne par lot démarre à un moment donné et affecte un groupe de personnes en même temps. Un exemple serait l&#39;envoi d&#39;un courriel à toutes les personnes en Californie.

Les campagnes dynamiques par lot ne comportent que des filtres dans la section des listes dynamiques (c’est-à-dire qu’aucun déclencheur).

![](assets/batch-filter.png)

Cliquez sur l’onglet **Planifier** pour confirmer que la campagne dynamique est définie sur &quot;Lot&quot;.

![](assets/batch-c4.png)

**Batch Smart Campaigns**

* Peut être planifié pour des récurrences, telles que quotidiennes, hebdomadaires et mensuelles. Vous pouvez également les faire exécuter une seule fois.
* Sont visibles sur la vue [de](../../../../product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md)Planning du programme.\
   *Notez que tout élément après une étape &quot;Attendre&quot; dans la campagne intelligente ne sera pas inclus dans la vue.

<br> 

## Trigger Smart Campaign {#trigger-smart-campaign}

>[!NOTE]
>
>**Définition**
>
>Une campagne intelligente de déclenchement affecte une personne à la fois en fonction d’un événement déclenché. Un exemple de déclencheur consiste à cliquer sur un lien dans un courrier électronique.

Si une campagne intelligente utilise au moins un déclencheur dans la section liste intelligente, le mode est automatiquement défini sur déclenché.

![](assets/trigger.png)

Cliquez sur l’onglet **Planifier** pour confirmer que la campagne dynamique est définie sur &quot;Déclenché&quot;.

![](assets/trigger2.png)

**Déclencher des campagnes dynamiques**

* Impossible de planifier les répétitions. Ils ne peuvent être définis que sur principal ou inactif.
* Vous pouvez définir plusieurs déclencheurs. Cependant, si un déclencheur est déclenché, les actions de campagne s&#39;exécuteront.

## Regardez une vidéo sur la création de campagnes par courriel déclenchées. {#watch-a-video-on-creating-triggered-email-campaigns}

`<iframe width="630" height="470" src="//play.vidyard.com/6zNazwTgt2LNeCjPAt3W9K.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

>[!TIP]
>
>Utilisez le journal [des](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) activités pour déterminer les étapes successives de vos campagnes intelligentes. Le journal des activités se trouve dans le dernier onglet de la page des détails d’une personne.

