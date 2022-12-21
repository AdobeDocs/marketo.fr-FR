---
unique-page-id: 7514918
description: Présentation du désabonnement - Documents Marketo - Documentation du produit
title: Comprendre le désabonnement
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 2%

---

# Comprendre le désabonnement {#understanding-unsubscribe}

Il existe en fait plusieurs types différents de désabonnements intégrés dans Marketo. Ils sont tous représentés par des champs sur l’objet person, tout comme First Name.

>[!NOTE]
>
>Marketo est en train de modifier des termes tels que Liste bloquée et Liste autorisée pour Placer sur la liste bloquée et Placer sur la liste autorisée dans notre produit. Au cours de cette mise à jour, il se peut que les anciens termes apparaissent dans les captures d’écran de l’interface utilisateur et de la documentation, ainsi que les nouveaux termes dans le texte de la documentation. Nous nous excusons pour toute confusion.

Tous ces champs sont intégrés à votre abonnement Marketo. Ils sont tous de type booléen (case à cocher). Ils peuvent être utilisés dans Forms ou [Modifier la valeur des données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) étapes de flux.

## Désabonné {#unsubscribed}

Elle est utilisée sur la page de désabonnement standard. Si une personne coche cette case ou clique sur le lien de désabonnement dans un email, elle ne recevra plus d’e-mails marketing. Ils recevront toutefois la contribution [e-mails opérationnels](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing interrompu {#marketing-suspended}

Ce champ est défini par l’utilisateur pour placer des personnes sur un désabonnement temporaire. Les personnes ne peuvent atteindre cet état que si elles sont modifiées manuellement ou si une étape de flux de valeur de données de modification est utilisée.

## E-mail interrompu {#email-suspended}

Ce statut bloque une personne dans les messages pendant 24 heures après un hard bounce. Au bout de 24 heures, la personne sera de nouveau en mesure de lui envoyer un courrier.

>[!NOTE]
>
>L’email Suspendu restera coché même une fois la période de 24 heures terminée. Vous pouvez donc vous référer aux personnes qui ont été marquées comme telles historiquement. Pour savoir si la personne est envoyée, il vous suffit de calculer 24 heures après le moment de suspension de l&#39;email.

## Figurant sur la liste de blocage {#blocklisted}

[Utilisez-le pour des personnes comme des concurrents](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Tous ceux que vous souhaitez recevoir **non** emails : opérationnels, marketing, etc. Ils n&#39;ont rien !

![](assets/image2015-5-18-12-3a6-3a40.png)
