---
unique-page-id: 1146987
description: Suppression d’une étape de flux - Documents Marketo - Documentation du produit
title: Suppression d’une étape de flux
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Suppression d’une étape de flux {#delete-a-flow-step}

>[!CAUTION]
>
>Suppression des étapes de flux, _processus d’attente particulièrement_ des campagnes dynamiques actives peuvent avoir des résultats inattendus. Lisez cet article attentivement.

Commençons par parler des bases. Voici comment supprimer une étape de flux indésirable d’une campagne dynamique.

1. Dans la campagne dynamique **[!UICONTROL Flux]**, cliquez sur le **X** pour supprimer une étape de flux.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Cliquez sur **[!UICONTROL Supprimer]**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Simple et facile, n&#39;est-ce pas ? La plupart du temps...

   >[!CAUTION]
   >
   >Suppression, ajout et déplacement d’étapes dans une _active_ campaign peut avoir des résultats inattendus. Envisagez de créer une campagne, de la tester, puis de la changer.

   Des modifications peuvent être apportées à une campagne active, mais peuvent avoir des conséquences imprévues. Voici les détails :

   **Campagnes dynamiques par lots**

   Si votre campagne :

   1. **Jamais couru**. Effectuez toutes les modifications de votre choix. Cela n&#39;affectera personne tant que vous n&#39;aurez pas lancé cette campagne.
   1. **est une campagne dynamique récurrente ;**. Les modifications affecteront les personnes dans les prochaines exécutions, et non les précédentes.
   1. **Déjà en cours d’exécution sans étapes d’attente**.Aucune personne ne sera affectée car la campagne est inactive après avoir été lancée.
   1. **Fonctionne en ce moment**. Les modifications peuvent provoquer un comportement inattendu en fonction du timing et des détails de la suppression. Nous vous recommandons vivement de NE PAS modifier une campagne par lot active. Pour les cas d&#39;urgence, apprenez à [abandon d’une campagne dynamique en cours](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md){target="_blank"}.

   1. **Déjà exécuté avec des étapes d’attente.** Plusieurs détails sur celui-ci.\
      Lorsqu’une personne entre dans une étape d’attente, elle indique la durée à laquelle elle doit revenir, ainsi que l’ÉTAPE NUMÉRO. Voir l’exemple ci-dessous.

   **Déclenchement de campagnes dynamiques**

   1. **Aucune étape d’attente**. Si vous supprimez une étape normale, seules les personnes qui passent par la campagne à l’avenir seront affectées.
   1. **Avec les étapes d’attente**. Voir l’exemple ci-dessous pour les campagnes par lots. La même logique s&#39;applique.

   >[!NOTE]
   >
   >**Exemple**
   >
   >1. Une campagne dynamique comporte 3 étapes.
   >    * ÉTAPE 1. Envoyer un courrier électronique #1
   >    * ÉTAPE 2. Attente 1 semaine
   >    * ÉTAPE 3. Envoyer un courrier électronique #2
   >
   >1. Personnes qui ont frappé **Étape 2** attend 1 semaine avant de passer à **Étape 3**.
   >1. Vous supprimez **Étape 2** pendant la semaine.
   >1. Les utilisateurs continueront à attendre la semaine 1 (ils ne retourneront pas automatiquement dans le flux).
   >1. Quand ils reviendront enfin, ils essaieront d&#39;aller à **Étape 3**. Ils ne le trouveront pas.
   >1. **IMPORTANT :** Comme il n&#39;y a maintenant que 2 étapes, les gens _ne recevra pas de #2 de messagerie_.
