---
unique-page-id: 1146987
description: Suppression d’une étape de flux - Documents Marketo - Documentation du produit
title: Supprimer une étape de flux
exl-id: 039a1e80-48cc-47f9-9e1a-459f89bf0730
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 2%

---

# Supprimer une étape de flux {#delete-a-flow-step}

>[!CAUTION]
>
>La suppression d’étapes de flux, _en particulier d’étapes d’attente_ dans les campagnes dynamiques actives, peut avoir des résultats inattendus. Lisez attentivement cet article.

Commençons par les principes de base. Voici comment supprimer une étape de flux indésirable d’une campagne dynamique.

1. Dans le **[!UICONTROL Flux]** de campagne intelligente, cliquez sur l’icône **X** pour supprimer une étape de flux.

   ![](assets/delete-a-flow-step-1.png)

1. Cliquez sur **[!UICONTROL Supprimer]**.

   ![](assets/delete-a-flow-step-2.png)

   >[!CAUTION]
   >
   >La suppression, l’ajout et le déplacement d’étapes dans une campagne _active_ peuvent avoir des résultats inattendus. Envisagez de créer une campagne, de la tester, puis de changer de campagne.

   Des modifications peuvent être apportées à une campagne active, mais elles peuvent avoir des conséquences imprévues. Voici les détails :

   **Campagnes intelligentes par lots**

   Si votre campagne :

   1. **Jamais couru**. Apportez toutes les modifications souhaitées. Cela n’affectera personne tant que vous n’aurez pas exécuté cette campagne.
   1. **Est une campagne intelligente récurrente**. Les modifications affecteront les personnes lors des exécutions suivantes, et non lors des exécutions précédentes.
   1. **Déjà exécutée SANS étapes d’attente**.Aucune personne ne sera affectée, car la campagne est inactive après l’exécution.
   1. **Est en cours d’exécution**. Les modifications peuvent provoquer un comportement inattendu en fonction du timing et des détails de la suppression. Nous vous recommandons vivement de NE PAS modifier une campagne par lots en cours d’exécution. Pour les cas d’urgence, découvrez comment [abandonner une campagne intelligente en cours d’exécution](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/abort-a-smart-campaign.md){target="_blank"}.

   1. **Déjà exécuté avec étapes d’attente.** Plusieurs détails sur celui-ci.
Lorsqu’une personne passe à une étape d’attente, elle note la durée et l’ÉTAPE NUMÉRIQUE à laquelle revenir. Voir l’exemple ci-dessous.

   **Déclencher des campagnes intelligentes**

   1. **Aucune étape d’attente**. Si vous supprimez une étape normale, seules les personnes qui exécuteront ultérieurement la campagne seront affectées.
   1. **Avec étapes d’attente**. Voir l’exemple ci-dessous pour les campagnes par lots. La même logique s’applique.

   >[!NOTE]
   >
   >**Exemple**
   >
   >1. Une campagne intelligente se compose de 3 étapes.
   >    * ÉTAPE 1. Envoyer un e-mail #1
   >    * ÉTAPE 2. Attendre 1 semaine
   >    * ÉTAPE 3. Envoyer un e-mail #2
   >
   >1. Les personnes qui atteignent **Étape 2** attendront 1 semaine avant de passer à **Étape 3**.
   >1. Vous supprimez **étape 2** au cours de la semaine.
   >1. Les personnes continueront à attendre pendant 1 semaine (elles ne reviennent pas automatiquement dans le flux).
   >1. Lorsqu’ils reviendront enfin, ils essaieront d’aller à **Étape 3**. Ils ne le trouveront pas.
   >1. **IMPORTANT :** comme il n’y a désormais que 2 étapes, les personnes _ne recevront pas de #2 par e-mail_.
