---
unique-page-id: 1147066
description: Remplacer les restrictions sur les personnes dans une Campaign intelligente - Docs marketing - Documentation sur les produits
title: Remplacer les restrictions de personne dans une Campaign dynamique
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Remplacer les restrictions de personne dans une Campaign dynamique {#override-person-restrictions-in-a-smart-campaign}

Marketo vous permet de définir le nombre maximum* *de personnes pouvant bénéficier d’une campagne intelligente ; cela vous permet d’éviter d’envoyer par courrier électronique l’intégralité de votre base de données. Si vous voulez *remplacer* cette limite, voici comment.

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>**Conditions préalables**
>
>Veillez à [activer les restrictions de personnes pour les campagnes](../../../../product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) dynamiques dans l’administration de Marketing Cloud.

1. Dans Activités marketing, accédez à votre campagne** **intelligente et cliquez sur **Planifier**.

   ![](assets/one.png)

   Dans Paramètres Smart Campaign, cliquez sur Modifier.
   ![](assets/two.png)

   >[!NOTE]
   >
   >La limite par défaut est celle définie dans Admin.

1. Saisissez une nouvelle limite, puis cliquez sur **Enregistrer.**

   ![](assets/three.png)

   La campagne intelligente ne s’exécute pas si le nombre de personnes admissibles dépasse la limite définie.

   >[!CAUTION]
   >
   >Soyez prudent avec cette fonction afin de ne pas inclure accidentellement trop de personnes.

