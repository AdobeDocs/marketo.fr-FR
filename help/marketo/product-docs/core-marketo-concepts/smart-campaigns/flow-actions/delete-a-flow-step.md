---
unique-page-id: 1146987
description: Suppression d’une étape de flux - Documents Marketo - Documentation du produit
title: Suppression d’une étape de flux
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Suppression d’une étape de flux {#delete-a-flow-step}

>[!CAUTION]
>
>Suppression des étapes de flux, _en particulier les étapes d’attente_ des principales campagnes intelligentes peuvent avoir des résultats inattendus. **Lisez cet article attentivement.**

D&#39;abord, faisons les bases. Voici comment supprimer une étape de flux indésirable d’une campagne dynamique. 1. Dans le flux de la campagne dynamique, cliquez sur l’icône X pour supprimer une étape de flux.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Cliquez sur **Supprimer**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Simple et facile, n&#39;est-ce pas ? La plupart du temps...

   >[!CAUTION]
   >
   >Suppression, ajout et déplacement d’étapes dans une **principal** campaign peut avoir des résultats inattendus. Envisagez de créer une campagne, de la tester, puis de la changer.

   Des changements peuvent être apportés à une principale campagne, mais peuvent avoir des conséquences imprévues. Voici les détails :

   **Campagnes dynamiques par lots**

   Si votre campagne :

   1. **Jamais ne courut.** Effectuez toutes les modifications de votre choix. Cela n&#39;affectera personne tant que vous n&#39;aurez pas lancé cette campagne.
   1. **est une campagne dynamique récurrente.** Les modifications affecteront les personnes dans les prochaines exécutions, et non les précédentes.
   1. **Déjà en cours d’exécution SANS étapes d’attente.** Aucune personne ne sera affectée parce que la campagne est inactive après avoir couru.
   1. **Il court en ce moment.** Les modifications peuvent provoquer un comportement inattendu en fonction du timing et des détails de la suppression. Nous vous recommandons vivement de NE PAS modifier une campagne par lot active. Pour les cas d&#39;urgence, apprenez à [abandon d’une campagne dynamique en cours](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md).

   1. **Déjà exécuté avec des étapes d’attente.** Plusieurs détails sur celui-ci.\
      Lorsqu’une personne entre dans une étape d’attente, elle indique la durée à laquelle elle doit revenir, ainsi que l’ÉTAPE NUMÉRO. Voir l’exemple ci-dessous.

   **Déclenchement de campagnes dynamiques**

   1. **Pas d’étapes d’attente.** Si vous supprimez une étape normale, seules les personnes qui passent par la campagne à l’avenir seront affectées.
   1. **Avec des étapes d’attente.** Voir l’exemple ci-dessous pour les campagnes par lots. La même logique s&#39;applique.

   >[!NOTE]
   >
   >**Exemple**
   >
   >1. Une campagne intelligente comporte 3 étapes.
      >    * ÉTAPE 1. Envoyer un courrier électronique #1
      >    * ÉTAPE 2. Attente 1 semaine
      >    * ÉTAPE 3. Envoyer un courrier électronique #2
   >
   >1. Personnes qui ont frappé **Étape 2** attend 1 semaine avant de passer à **Étape 3**.
   >1. Vous supprimez **Étape 2** pendant la semaine.
   >1. Les gens continueront à attendre la semaine. (Ils ne reviennent pas automatiquement dans le flux.)
   >1. Quand ils reviendront enfin, ils essaieront d&#39;aller à **Étape 3**. Ils ne le trouveront pas.
   >1. **IMPORTANT :** Comme il n’y a maintenant que 2 étapes, la variable *Les gens ne recevront pas de #2 d&#39;email.*


Modifications apportées à une campagne Principale

Comprenez cette fonctionnalité et vous maîtriserez les campagnes intelligentes.
