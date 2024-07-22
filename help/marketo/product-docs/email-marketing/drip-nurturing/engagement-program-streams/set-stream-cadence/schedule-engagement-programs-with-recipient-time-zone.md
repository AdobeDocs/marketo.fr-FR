---
unique-page-id: 12982909
description: Planification des programmes d’engagement avec fuseau horaire du destinataire - Documents Marketo - Documentation du produit
title: Planification des programmes d’engagement avec fuseau horaire des destinataires
exl-id: 818615be-3c7e-4051-adc7-2341783484b9
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 1%

---

# Planification des programmes d’engagement avec fuseau horaire des destinataires {#schedule-engagement-programs-with-recipient-time-zone}

Lorsque vous planifiez un flux de programme d’engagement et que le fuseau horaire des destinataires est actif, la diffusion du programme commencera à s’exécuter à minuit dans le premier fuseau horaire (UTC +14:00). Nous vous demandons de programmer la première diffusion **au moins 25 heures** à l’avenir, car il peut y avoir des personnes qui remplissent les critères pour la diffusion dans chaque fuseau horaire à travers le monde. Le démarrage du traitement à cette heure dans le premier fuseau horaire garantit que nous délivrerons l&#39;email à la date et à l&#39;heure planifiées de chaque destinataire.

1. Dans votre programme d’engagement, accédez à l’onglet **Flux** et cliquez sur le planning de cadence d’un flux pour le modifier.

   ![](assets/image2017-12-5-13-3a36-3a21.png)

1. [Définissez vos paramètres de cadence](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md) comme vous le feriez normalement, puis cochez la case **Fuseau horaire du destinataire** . N&#39;oubliez pas que votre première diffusion doit avoir lieu au moins 25 heures plus tard. Cliquez sur **Enregistrer**.

   ![](assets/image2017-12-5-13-3a50-3a32.png)

1. Notez que si le fuseau horaire du destinataire est actif, le planning de cadence n’affiche pas de fuseau horaire spécifique, puisqu’il peut y avoir plusieurs fuseaux horaires. L’heure s’affiche uniquement.

   ![](assets/image2017-12-5-13-3a56-3a21.png)

>[!MORELIKETHIS]
>
>* [Comprendre le fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Définir l’cadence de diffusion](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)
