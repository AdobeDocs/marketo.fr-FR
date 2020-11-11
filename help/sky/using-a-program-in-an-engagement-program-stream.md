---
title: utilisation-d'un programme-dans-un-programme-flux
description: Utilisation d’un Programme dans un flux de Programme d’engagement
translation-type: tm+mt
source-git-commit: 73df78512226c6c57625a73f14ba8b00bea195bd
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# Utilisation d’un Programme dans un flux de Programme d’engagement

## Pourquoi utiliser un programme imbriqué dans un flux de programme d’engagement ?

Il est facile d’ajouter un courriel à un flux dans un programme d’engagement, et ça fonctionne bien. Cependant, si vos besoins commerciaux sont plus complexes, il peut être logique de placer le courriel dans un programme. Par exemple, vous pouvez souhaiter :

* Envoyer un courrier électronique à un sous-groupe de personnes dans le flux
* Envoyer _différents_ messages électroniques à des sous-groupes dans le flux
* Inclure des landings page, des formulaires ou d’autres ressources dans le programme d’engagement
* Activer l’attribution multipoint
* Ajouter des étapes de flux supplémentaires, telles que les courriers électroniques d’alerte

## Que se passe-t-il lorsque vous utilisez un programme dans un flux ?

Lors de l’utilisation d’un programme imbriqué, la décision d’envoyer un courrier électronique à une personne repose sur l’appartenance au programme et l’identifiant de programme.

* Si vous n&#39;êtes pas membre du programme, vous recevrez un jour un courriel faisant partie du programme.
* Si vous êtes membre du programme, vous ne recevrez pas le courriel
* Si vous n’êtes plus membre mais que vous avez déjà reçu le courriel plus tôt par ce programme, vous ne recevrez pas le courriel.

Lorsque vous utilisez un programme dans un flux, cela n’a pas d’importance si vous avez déjà reçu ce message. Tant que le courrier électronique n’a pas été envoyé avant _dans ce programme_ spécifique, vous pouvez le recevoir à nouveau.

Il peut être difficile de mélanger des courriels et des programmes dans un programme d&#39;engagement. Vous pouvez utiliser l&#39;un ou l&#39;autre.

>[!TIP]
>
>Veillez à utiliser un filtre Programme Membre de l’engagement dans votre liste dynamique.

## Qu&#39;arrive-t-il aux personnes qui ne répondent pas aux critères de liste intelligente ?

Dans le événement où une personne est filtrée hors de la liste intelligente de la campagne intelligente d’un programme imbriqué, elle ne passe pas à l’élément de contenu suivant pendant la diffusion en cours. Ils passeront à l’élément de contenu suivant dans le flux pour la diffusion _suivante_ .

## Que contient un programme imbriqué ?

Un programme imbriqué bien conçu contient des courriels, des rapports et des campagnes intelligentes. Il est logique de les garder ensemble.

L’e-mail que vous utilisez peut résider dans le programme, dans un autre programme ou même dans Design Studio. L&#39;endroit où il vit dépend de la façon dont vous voulez l&#39;utiliser.

Le rapports change avec l’emplacement du courrier électronique. Ainsi, par exemple, si le courrier électronique se trouve dans Design Studio, dans le rapport Performance du courrier électronique, toutes les mesures sont affichées sur une seule ligne : les différentes distributions sont combinées. Cependant, dans le rapport Performance du flux d’engagement, les différentes émissions s’affichent séparément.

>[!CAUTION]
>
>Si vous souhaitez renvoyer quelque chose, il est plus sûr de créer un nouveau programme et une campagne intelligente.
