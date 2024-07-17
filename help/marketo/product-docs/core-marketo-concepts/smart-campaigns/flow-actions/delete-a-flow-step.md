---
unique-page-id: 1146987
description: Suppression d’une étape de flux - Documents Marketo - Documentation du produit
title: Suppression d’une étape de flux
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Suppression d’une étape de flux {#delete-a-flow-step}

>[!CAUTION]
>
>La suppression des étapes de flux, _en particulier les étapes d’attente_ des campagnes dynamiques actives, peut avoir des résultats inattendus. Lisez cet article attentivement.

Commençons par parler des bases. Voici comment supprimer une étape de flux indésirable d’une campagne dynamique.

1. Dans la campagne dynamique **[!UICONTROL Flux]**, cliquez sur l’icône **X** pour supprimer toute étape de flux.

   ![](assets/delete-a-flow-step-1.png)

1. Cliquez sur **[!UICONTROL Supprimer]**.

   ![](assets/delete-a-flow-step-2.png)

   >[!CAUTION]
   >
   >La suppression, l’ajout et le déplacement d’étapes dans une campagne _active_ peuvent avoir des résultats inattendus. Envisagez de créer une campagne, de la tester, puis de la changer.

   Des modifications peuvent être apportées à une campagne active, mais peuvent avoir des conséquences imprévues. Voici les détails :

   **Campagnes dynamiques par lots**

   Si votre campagne :

   1. **Ne s’est jamais exécuté**. Effectuez toutes les modifications de votre choix. Cela n&#39;affectera personne tant que vous n&#39;aurez pas lancé cette campagne.
   1. **Est une campagne dynamique récurrente**. Les modifications affecteront les personnes dans les prochaines exécutions, et non les précédentes.
   1. **Déjà en cours d’exécution SANS attendre les étapes**. Aucune personne ne sera affectée car la campagne est dormante après son exécution.
   1. **Fonctionne en ce moment**. Les modifications peuvent provoquer un comportement inattendu en fonction du timing et des détails de la suppression. Nous vous recommandons vivement de NE PAS modifier une campagne par lot active. Pour les cas d’urgence, découvrez comment [abandonner une campagne dynamique en cours d’exécution](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md){target="_blank"}.

   1. **Déjà exécuté AVEC des étapes d’attente.** Plusieurs détails sur celui-ci.\
      Lorsqu’une personne entre dans une étape d’attente, elle indique la durée à laquelle elle doit revenir, ainsi que l’ÉTAPE NUMÉRO. Voir l’exemple ci-dessous.

   **Déclencher des campagnes dynamiques**

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
   >1. Les personnes qui ont appuyé sur **Étape 2** attendront 1 semaine avant de passer à l’ **Étape 3**.
   >1. Vous supprimez **Etape 2** pendant la semaine.
   >1. Les utilisateurs continueront à attendre la semaine 1 (ils ne retourneront pas automatiquement dans le flux).
   >1. Quand ils reviendront enfin, ils essaieront d&#39;aller à l&#39;**Étape 3**. Ils ne le trouveront pas.
   >1. **IMPORTANT :** Comme il n&#39;y a que 2 étapes, les personnes _ne recevront pas d&#39;email #2_.
