---
unique-page-id: 10098134
description: Ajouter un Programme à un flux de Programme d’engagement - Documents marketing - Documentation du produit
title: Ajouter un Programme à un flux de Programme d’engagement
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Ajouter un Programme à un flux de Programme d’engagement {#adding-a-program-to-an-engagement-program-stream}

## Pourquoi utiliser un programme imbriqué dans un flux de programme d’engagement ? {#why-use-a-nested-program-in-an-engagement-program-stream}

Il est facile d’ajouter un courriel à un flux dans un programme d’engagement, et ça fonctionne bien. Cependant, si vos besoins commerciaux sont plus complexes, il peut être logique de placer le courriel dans un programme. Par exemple, vous pouvez souhaiter :

* Envoyer un courrier électronique à un sous-groupe de personnes dans le flux
* Envoyer *différents* messages électroniques à des sous-groupes dans le flux
* Inclure des landings page, des formulaires ou d’autres ressources dans la culture
* Activer l’attribution multipoint
* Ajouter des étapes de flux supplémentaires, telles que les courriers électroniques d’alerte

## Que se passe-t-il lorsque vous utilisez un programme dans un flux ? {#what-happens-when-you-use-a-program-in-a-stream}

Lors de l’utilisation d’un programme imbriqué, la décision d’envoyer un courrier électronique à une personne repose sur l’appartenance au programme et l’identifiant de programme.

* Si vous n&#39;êtes pas membre d&#39;un programme, vous recevrez un courriel qui fait partie du programme une fois.
* Si vous êtes membre du programme, vous ne recevrez pas le courriel
* Si vous n’êtes plus membre mais que vous avez reçu le courriel plus tôt par ce programme, vous ne recevrez pas le courriel.

Lorsque vous utilisez un programme dans un flux, cela n’a pas d’importance si vous avez déjà reçu ce message. Tant que le courrier électronique n’a pas été envoyé avant *dans ce programme* spécifique, vous pouvez le recevoir à nouveau.

Il peut être difficile de mélanger des courriels et des programmes dans un programme d&#39;engagement. Vous pouvez utiliser l&#39;un ou l&#39;autre.

>[!TIP]
>
>Veillez à utiliser un filtre Programme **** membre d’engagement dans votre liste dynamique.

## Qu&#39;arrive-t-il aux personnes qui ne répondent pas aux critères de liste intelligente ? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Dans le événement où une personne est filtrée hors de la liste intelligente de la campagne intelligente d’un programme imbriqué, elle ne passe pas à l’élément de contenu suivant pendant la diffusion en cours. Ils passeront à l’élément de contenu suivant dans le flux pour la diffusion *suivante* .

## Que contient un programme imbriqué ? {#what-does-a-nested-program-contain}

Un programme imbriqué bien conçu contient des courriels, des rapports et des campagnes intelligentes. Il est logique de les garder ensemble.

L’e-mail que vous utilisez peut résider dans le programme, dans un autre programme ou même dans Design Studio. L&#39;endroit où il habite dépendra de la façon dont vous voulez l&#39;utiliser.

Le rapports change avec l’emplacement du courrier électronique. Ainsi, par exemple, si le courrier électronique se trouve dans Design Studio, dans le rapport Performance du courrier électronique, toutes les mesures sont affichées sur une seule ligne : les différentes distributions sont combinées. Cependant, dans le rapport Performance du flux d’engagement, les différentes émissions s’affichent séparément.

>[!CAUTION]
>
>Si vous souhaitez renvoyer quelque chose, il est plus sûr de créer un nouveau programme et une campagne intelligente.

>[!MORELIKETHIS]
>
>* [Ajouter du contenu à un flux](add-content-to-a-stream.md)
>* [Présentation des Programmes](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

>



