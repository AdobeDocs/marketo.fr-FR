---
unique-page-id: 7514918
description: Présentation du désabonnement - Documents Marketo - Documentation du produit
title: Comprendre le désabonnement
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 2%

---

# Comprendre le désabonnement {#understanding-unsubscribe}

Il existe en fait plusieurs types différents de désabonnements intégrés dans Marketo. Ils sont tous représentés par des champs sur l’objet person, tout comme First Name.

Tous ces champs sont intégrés à votre abonnement Marketo. Ils sont tous de type booléen (case à cocher). Ils peuvent être utilisés dans les étapes de flux Forms ou [Modifier la valeur de données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

## Désabonné {#unsubscribed}

Elle est utilisée sur la page de désabonnement standard. Si une personne coche cette case ou clique sur le lien de désabonnement dans un email, elle ne recevra plus d’e-mails marketing. Ils recevront toutefois [e-mails opérationnels](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing interrompu {#marketing-suspended}

Ce champ est défini par l’utilisateur pour placer des personnes sur un désabonnement temporaire. Les personnes ne peuvent atteindre cet état que si elles sont modifiées manuellement ou si une étape de flux de valeur de données de modification est utilisée.

## E-mail interrompu {#email-suspended}

Ce statut bloque une personne dans les messages pendant 24 heures après un hard bounce. Au bout de 24 heures, la personne sera à nouveau en mesure de recevoir un courrier.

>[!NOTE]
>
>L’email Suspendu restera coché même une fois la période de 24 heures terminée. Vous pouvez donc vous référer aux personnes qui ont été marquées comme telles historiquement. Pour savoir si la personne est envoyée par courrier, il vous suffit de calculer 24 heures après le moment de suspension de l&#39;email.

## Figurant sur la liste de blocage {#blocklisted}

[Utilisez-le pour des personnes comme des concurrents](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Toute personne qui souhaite recevoir des **non** emails—opérationnel, marketing, etc. Ils n&#39;ont rien !

![](assets/image2015-5-18-12-3a6-3a40.png)
