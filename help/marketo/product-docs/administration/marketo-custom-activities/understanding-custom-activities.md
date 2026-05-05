---
unique-page-id: 10100266
description: Présentation des activités personnalisées pour le suivi des actions de personnes spécifiques à l’entreprise, en quoi elles diffèrent des objets personnalisés et la configuration en deux étapes de la création de l’activité et de l’implémentation de l’API.
title: Présentation des activités personnalisées
exl-id: 0bb74d9d-3a9d-4ef7-8c8c-2de36cd6190b
feature: Custom Activities
source-git-commit: 7fe6ed8b9fcb1aacf0e651a11ab90eaf0ae07937
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 8%

---

# Présentation des activités personnalisées {#understanding-custom-activities}

Suivez une action spécifique à votre entreprise, avec des activités personnalisées, entreprise par une personne.

## Que sont les activités ? {#what-are-activities}

Il existe plusieurs façons d’interagir avec votre organisation. Ils peuvent visiter le site Web de votre entreprise, assister à l&#39;un de vos salons professionnels ou cliquer sur un lien dans un courriel qui leur a été envoyé. Ces actions sont des activités, et quelle que soit l’action qu’elles entreprennent, Marketo la capture afin que votre équipe marketing puisse mieux comprendre comment leur envoyer des communications pertinentes et en temps opportun.

## Activités personnalisées {#custom-activities}

Les activités personnalisées vous permettent de suivre une activité qui n’est pas liée à un formulaire Marketo, un e-mail ou une page de destination. Pour savoir quand quelqu’un dépose un chèque, utilisez une activité personnalisée. Pour savoir quand quelqu’un participe à un webinaire, utilisez une activité personnalisée.

>[!NOTE]
>
>Les activités personnalisées diffèrent des objets personnalisés. Utilisez des objets personnalisés lorsque la valeur peut changer (par exemple, la « couleur de la voiture » passe de bleu à rouge). Utilisez des activités personnalisées lors du suivi des moments qui se sont produits et dont les détails ne peuvent pas changer (par exemple, « voiture achetée »).

## Champs {#fields}

Vous pouvez ajouter [champs supplémentaires](/help/marketo/product-docs/administration/marketo-custom-activities/add-edit-delete-marketo-custom-activity-fields.md) que vous souhaitez associer à votre activité. Comme le champ principal, ils peuvent être utilisés comme critères de filtrage dans une liste dynamique.

## Prise en main {#getting-started}

Les activités personnalisées fonctionnent comme les activités standard. Cependant, leur configuration est un processus en deux étapes.

Étape 1 : [création d’une activité personnalisée](/help/marketo/product-docs/administration/marketo-custom-activities/create-a-custom-activity.md) dans votre compte Marketo

Étape 2 : l’employé de votre entreprise qui travaille avec l’API Marketo peut alors commencer la mise en œuvre. Vous trouverez plus d’informations ici : [API d’activité personnalisée](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/addCustomActivityUsingPOST)
