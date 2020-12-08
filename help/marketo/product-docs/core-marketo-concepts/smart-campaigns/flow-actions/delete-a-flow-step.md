---
unique-page-id: 1146987
description: Suppression d’une étape de flux - Documents marketing - Documentation du produit
title: Suppression d’une étape de flux
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Suppression d’une étape de flux {#delete-a-flow-step}

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!CAUTION]
>
>La suppression des étapes de flux, *en particulier les étapes* d’attente des principales campagnes intelligentes, peut avoir des résultats inattendus. **Lisez cet article attentivement.**

D&#39;abord, faisons les bases. Voici comment supprimer une étape de flux indésirable d’une campagne intelligente. 1. Dans le flux de campagne dynamique, cliquez sur l’icône X pour supprimer une étape de flux.

![](assets/image2014-9-22-13-3a52-3a20.png)

1. Cliquez sur **Supprimer**.

   ![](assets/image2014-9-22-13-3a55-3a25.png)

   Simple et facile, n&#39;est-ce pas ? La plupart du temps...

   >[!CAUTION]
   >
   >La suppression, l’ajout et le déplacement d’étapes dans une campagne **principale** peuvent avoir des résultats inattendus. Envisagez de créer une nouvelle campagne, de la tester, puis de la changer.

   Des changements peuvent être apportés à une principale campagne, mais peuvent avoir des conséquences imprévues. Voici les détails :

   **Batch Smart Campaigns**

   Si votre campagne :

   1. **Jamais ne courut.** Effectuez toutes les modifications souhaitées. Cela n&#39;affectera personne tant que vous n&#39;aurez pas lancé cette campagne.
   1. **Est une campagne intelligente récurrente.** Les changements affecteront les futurs exécutions, et non les précédentes.
   1. **Déjà exécuté sans attendre les étapes.** Aucune personne ne sera affectée car la campagne est en sommeil après son exécution.
   1. **Est en cours d&#39;exécution en ce moment.** Les modifications peuvent provoquer un comportement inattendu en fonction du timing et des détails de la suppression. Nous vous recommandons vivement de NE PAS modifier une campagne par lot qui s’exécute activement. Pour les cas d’urgence, apprenez à [abandonner une campagne](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md)intelligente en cours d’exécution.

   1. **Déjà exécuté avec des étapes d’attente.** Plusieurs détails sur celui-ci.\
      Lorsqu&#39;une personne entre dans une étape d&#39;attente, elle fait une croix sur la durée et à quelle ÉTAPE DE NOMBRE revenir. Voir l’exemple ci-dessous.

   **Déclencher des campagnes dynamiques**

   1. **Pas d&#39;étapes d&#39;attente.** Si vous supprimez une étape normale, seules les personnes qui parcourront la campagne à l’avenir seront affectées.
   1. **Avec des étapes d&#39;attente.** Voir l’exemple ci-dessous pour les campagnes par lots. La même logique s&#39;applique.

   >[!NOTE]
   >
   >**Exemple**
   >
   >    
   >    
   >1. Une campagne intelligente comporte 3 étapes.
   >
   >   * ÉTAPE 1. Envoyer le courrier électronique n° 1
   >   * ÉTAPE 2. Attendez 1 semaine
   >   * ÉTAPE 3. Envoyer le courrier électronique n° 2
   >
   >1. Les personnes qui atteignent l’ **étape 2** attendront 1 semaine avant de passer à l’ **étape 3**.
   >1. Vous supprimez **l’étape 2** pendant la semaine.
   >1. Les gens continueront à attendre la semaine d&#39;une semaine. (Ils ne reviennent pas automatiquement dans le flux.)
   >1. Quand ils reviendront enfin, ils essaieront d&#39;aller à l&#39; **étape 3**. Ils ne le trouveront pas.
   >1. **IMPORTANT :** Étant donné qu&#39;il n&#39;y a que 2 étapes, les *gens ne recevront pas le courriel 2.*


Apporter des modifications à un Campaign Principal

Comprenez cette fonction et vous maîtriserez les campagnes intelligentes. Ouah !
