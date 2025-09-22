---
unique-page-id: 1147091
description: Présentation De L’Appartenance À Un Programme - Documents Marketo - Documentation Du Produit
title: Présentation de l’appartenance à un programme
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 3%

---

# Présentation de l’appartenance à un programme {#understanding-program-membership}

>[!NOTE]
>
>**Définition :** un membre est une personne qui possède un statut dans un programme.

## Comment les personnes deviennent membres d’un programme {#how-people-become-members-of-a-program}

1. Une personne remplit un [formulaire sur une page de destination](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} dans le programme.

   * La personne aura automatiquement le premier statut dans la progression.

1. Vous [importez des membres dans le programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md){target="_blank"} à partir d’un fichier CSV.

   * La personne aura automatiquement le premier statut dans la progression.

1. Vous utilisez l’étape de flux [modifier le statut du programme](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}.
1. Une personne s’inscrit ou assiste à un [webinaire synchronisé avec un programme d’événement](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md){target="_blank"}.
1. Une personne est [créée à l’aide de l’application d’archivage Marketo iPad](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md){target="_blank"}.
1. Une personne est ajoutée à une campagne SFDC, qui est [synchronisée avec le programme](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}.

>[!NOTE]
>
>Pour un programme de messagerie, une personne n’est ajoutée à l’abonnement que lorsque l’e-mail est envoyé.

## Statuts du programme {#program-statuses}

Les statuts de programme sont les étapes que les personnes suivent dans un programme (par exemple, Invité, Confirmation de participation, Pas d&#39;affichage). Ces étapes sont définies par le [canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>Une personne ne peut pas revenir à un statut de programme antérieur. La progression du statut est à sens unique.

## Statuts de réussite {#success-statuses}

L&#39;objectif d&#39;un programme est de créer une interaction significative avec la personne ou le prospect. La réussite est marquée lorsqu’une personne atteint le statut qui permet d’atteindre cet objectif.

>[!NOTE]
>
>Dans le cas d’un webinaire, l’inscription n’est pas une interaction significative si les personnes ne regardent pas réellement le webinaire. La participation est une réussite dans ce cas.

## Programme d’acquisition {#acquisition-program}

Lorsqu’un nouveau nom apparaît dans le système en tant que membre du programme, Marketo définit automatiquement ce programme comme une « acquisition ». Cela établit le crédit pour [attribution Première touche](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Utilisation de balises dans un programme](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/use-tags-in-a-program.md){target="_blank"}
>* [Créer un rapport sur le rendement du programme](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md){target="_blank"}
