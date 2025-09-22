---
unique-page-id: 10098134
description: Ajout d’un programme à un flux de programmes d’engagement - Documents Marketo - Documentation du produit
title: Ajouter un programme à un flux de programme d’engagement
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 3%

---

# Ajouter un programme à un flux de programme d’engagement {#adding-a-program-to-an-engagement-program-stream}

## Pourquoi utiliser un programme imbriqué dans un flux de programme d’engagement ? {#why-use-a-nested-program-in-an-engagement-program-stream}

Il est facile d’ajouter un e-mail à un flux dans un programme d’engagement, et cela fonctionne correctement. Cependant, si les besoins de votre entreprise sont plus complexes, il peut être logique de placer l’e-mail dans un programme. Par exemple, vous pouvez effectuer les opérations suivantes :

* Envoyer un e-mail à un sous-groupe de personnes dans le flux
* Envoyer des e-mails *différents* aux sous-groupes dans le flux
* Inclure des pages de destination, des formulaires ou d’autres ressources dans le parcours
* Activer l’attribution multipoint
* Ajouter des étapes de flux supplémentaires, telles que des e-mails d’alerte

## Que se passe-t-il lorsque vous utilisez un programme dans un flux ? {#what-happens-when-you-use-a-program-in-a-stream}

Lors de l’utilisation d’un programme imbriqué, la décision d’envoyer un e-mail à une personne est basée sur l’appartenance au programme et l’ID de programme.

* Si vous n’êtes pas membre d’un programme, vous recevrez tous les e-mails qui font partie du programme une fois
* Si vous êtes membre du programme, vous ne recevrez pas l’e-mail
* Si vous n’êtes plus membre, mais que vous avez reçu l’e-mail plus tôt par le biais de ce programme, vous ne recevrez pas l’e-mail

Lorsque vous utilisez un programme dans un flux, peu importe si vous avez déjà reçu cet e-mail spécifique. Tant que l’e-mail n’a pas été envoyé avant *dans ce programme spécifique*, vous pouvez le recevoir à nouveau.

Il peut s’avérer difficile de mélanger des e-mails et des programmes dans un programme d’engagement. Vous pouvez utiliser l&#39;un ou l&#39;autre.

>[!TIP]
>
>Veillez à utiliser un filtre **[!UICONTROL Membre du programme d’engagement]** dans votre liste dynamique.

## Qu&#39;arrive-t-il aux personnes qui ne répondent pas aux critères de la liste dynamique? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Dans le cas où une personne est exclue de la liste dynamique de la campagne dynamique d’un programme imbriqué, elle ne passe pas au contenu suivant pendant le cast actuel. Ils passeront au contenu suivant du flux pour le cast *suivant*.

## Que contient un programme imbriqué ? {#what-does-a-nested-program-contain}

Un programme imbriqué bien conçu contient des e-mails, des rapports et des campagnes intelligentes. C&#39;est logique de les garder ensemble.

L’e-mail que vous utilisez peut résider dans le programme, dans un autre programme ou même dans le [!UICONTROL Design Studio]. L’endroit où elle vivra dépendra de la manière dont vous l’utiliserez.

Reporting des modifications avec l’emplacement des e-mails. Ainsi, par exemple, si l’e-mail se trouve dans le [!UICONTROL Design Studio], dans le rapport Performance de l’e-mail, toutes les mesures sont affichées sur une ligne - les différents conversions sont combinées. Cependant, dans le rapport de performances du flux d’engagement, les différents envois s’affichent séparément.

>[!CAUTION]
>
>Si vous souhaitez renvoyer quelque chose, il est préférable de créer un nouveau programme et une campagne intelligente.

>[!MORELIKETHIS]
>
>* [Ajouter du contenu à un flux](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Présentation des programmes](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
