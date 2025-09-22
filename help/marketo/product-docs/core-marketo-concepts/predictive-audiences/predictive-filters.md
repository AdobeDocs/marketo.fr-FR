---
description: Filtres Prédictifs - Documents Marketo - Documentation Du Produit
title: Filtres prédictifs
exl-id: 27736b80-cd8b-455d-9d73-c17d492d0906
feature: Predictive Audiences
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 3%

---

# Filtres prédictifs {#predictive-filters}

Dans le cadre des audiences prédictives, Marketo propose un groupe de filtres basés sur l’IA/ML dans les listes intelligentes des campagnes intelligentes.

![Image Un](assets/predictive-filters-1.png)

>[!NOTE]
>
>Les filtres « Probablement présent » et « Probablement inscrit » ne peuvent être utilisés que dans les programmes d’événement. Les options « Probabilité de désabonnement », « Ressemblance des membres du programme » et « Ressemblance des membres de la liste dynamique » peuvent être utilisées dans tous les types de programme.

## Probabilité de participation {#likelihood-to-attend}

Ce filtre permet de réduire efficacement votre audience. Vous pouvez ainsi cibler et inviter les prospects qui ont une probabilité plus élevée d’**assister** à votre webinaire ou événement. Notez que votre « Programme de participation probable » sera votre programme d’événement actuel.

![Image 2](assets/predictive-filters-2.png)

## Probabilité d’inscription {#likelihood-to-register}

Tout comme le filtre _Probabilité d’assister_, utilisez ce filtre pour limiter votre audience et cibler les prospects qui ont une probabilité plus élevée de **s’inscrire** à votre webinaire ou votre événement.

![Image trois](assets/predictive-filters-3.png)

## Probabilité de désinscription {#likelihood-to-unsubscribe}

Cette option filtre l’audience en fonction de la probabilité faible ou élevée de se désabonner au cours des deux prochaines semaines. Vous pouvez l’utiliser pour cibler différemment et plus efficacement les prospects à forte fatigue. Le seuil de désabonnement est dynamique et piloté par un modèle d’IA qui prend en compte plusieurs attributs, notamment le délai dans la base de données et les activités de prospect.

![Image 4](assets/predictive-filters-4.png)

>[!NOTE]
>
>Les filtres Probabilité d’assister à la session/de s’inscrire/de se désabonner doivent être utilisés conjointement avec d’autres filtres standard.

## Ressemblance des membres de programme/Ressemblance des membres de liste dynamique {#lookalike-of-members}

Ces deux filtres vous aident à élargir votre audience actuelle en ciblant des prospects supplémentaires similaires aux membres d’un autre programme ou d’une liste dynamique. Les filtres semblables prennent en compte plus de 50 facteurs, notamment les attributs du prospect, l’activité des e-mails, l’activité web et l’engagement.

Cliquez sur **[!UICONTROL Ajouter une contrainte]** pour choisir les critères de succès pour les membres du ou des programmes sélectionnés.

Cliquez sur l’icône **+** pour ajouter facilement plusieurs programmes/listes dynamiques à un filtre.

![Image 5](assets/predictive-filters-5.png)

## Éléments à noter {#things-to-note}

* Vous pouvez appliquer des filtres prédictifs à une campagne dynamique même si le programme parent est créé avant l’activation des filtres prédictifs.
* Les filtres prédictifs ne sont pas disponibles pour les campagnes de déclenchement.
* Le clonage ou le déplacement de campagnes contenant des filtres prédictifs n’est pas pris en charge.
* Vous pouvez utiliser jusqu’à 5 filtres prédictifs dans une liste dynamique.
* Si Marketo Engage rencontre une erreur dans l’évaluation des filtres prédictifs, l’exécution de la campagne s’interrompt automatiquement et vous recevez une notification dans le centre de notifications Marketo.
* Les filtres prédictifs ont actuellement une limite d’entrée de 1 million de personnes qualifiées.
* Vous pouvez avoir jusqu’à 50 programmes actifs avec des filtres prédictifs.
