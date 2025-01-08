---
description: Promotion d’un webinaire interactif - Documents Marketo - Documentation du produit
title: Promouvoir un webinaire interactif
feature: Interactive Webinars
exl-id: d26f91ce-3a95-4247-9a52-085260bb15e8
source-git-commit: 75035e6ae7989aaf3ed6cedd7fdab42c79ab8f37
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Promouvoir un webinaire interactif {#promoting-an-interactive-webinar}

La promotion d’un webinaire interactif est similaire à la promotion d’un webinaire partenaire via Launchpoint. Lors de la création d’un programme d’événement de webinaire interactif, vous pouvez ajouter des membres en exécutant une campagne ou en important des membres dans le programme. Pour vérifier les membres qui ont été ajoutés au programme d’événement de webinaires interactifs, cliquez sur l’onglet **Membres**.

![](assets/promoting-an-interactive-webinar-1.png)

Une fois les membres ajoutés ou importés, vous pouvez créer une campagne par e-mail dans le programme d’événement de webinaire interactif pour envoyer une invitation à tous les membres du programme et modifier leur statut en « invité » une fois l’e-mail envoyé.

>[!NOTE]
>
>Si vous souhaitez ajouter un co-hôte ou un présentateur en tant que membre de l’audience au programme d’événement de webinaire interactif, vous devez utiliser un ID d’e-mail différent pour eux, sinon ils recevront l’erreur « cet e-mail est déjà enregistré ».

L’e-mail peut contenir des détails spécifiques sur le programme et inclure une URL de page de destination qui redirigerait le destinataire vers une page spécifique où des informations supplémentaires sur le webinaire (par exemple, le contenu, les informations du présentateur, etc.) peuvent être ajoutées. Cette page de destination peut être créée en tant que ressource locale dans le programme d’événement de webinaires interactifs.

Vous pouvez demander à vous inscrire à ce webinaire en activant un formulaire sur la page de destination et en liant les clics du formulaire à l’activation de l’inscription dans le programme d’événement de webinaire interactif. Une campagne peut ensuite être créée qui utilise les envois de formulaire comme déclencheur et modifie le statut du programme de « invité » en « enregistré ».

>[!NOTE]
>
>La transition de « invité » à « enregistré » n’est pas automatique dans les webinaires interactifs, car plusieurs déclencheurs peuvent créer cette transition.

Une fois qu’un membre a obtenu le statut d’inscription au programme dans un programme d’événement de webinaire interactif, une inscription au webinaire créé dans Adobe Connect est automatiquement effectuée. Les données d’enregistrement telles que le prénom, le nom et l’ID d’e-mail sont ensuite transférées vers Adobe Connect. Cela signifie qu’une fois que l’utilisateur rejoint le webinaire en tant que participant, les informations sont disponibles pour le présentateur ou l’hôte pendant le webinaire.

Quelques minutes après l’enregistrement, l’URL du webinaire du membre est renseignée dans l’onglet Membres . Si vous ne parvenez pas à localiser la colonne pour l’URL du webinaire, assurez-vous que cette colonne a été ajoutée à votre vue. Il s’agit d’une URL personnalisée permettant à chaque membre enregistré de participer au webinaire à une heure planifiée sans nécessiter d’authentification. Les jetons échangés en interne prennent en charge l’authentification des membres.

Vous pouvez utiliser le `{{member.webinar url}}` [jeton](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} pour inclure l’URL du webinaire aux membres individuels d’une campagne par e-mail afin de communiquer qu’ils ont été enregistrés à l’événement et d’utiliser l’URL de recrutement pour accéder au webinaire à l’heure planifiée. Des jetons de calendrier peuvent être utilisés dans la même campagne par e-mail pour vous assurer que le planning du webinaire peut être ajouté aux calendriers des membres.

Des liens sont disponibles sur le côté droit de l’onglet Aperçu de votre programme d’événement pour créer une page de destination ainsi qu’une campagne par e-mail. Le reste des promotions liées à un événement restent identiques aux webinaires des partenaires qui utilisent l’intégration de Launchpoint.

![](assets/promoting-an-interactive-webinar-2.png)

Les webinaires interactifs vous permettent de demander à vous inscrire avant, pendant ou après un webinaire. Dans tous les cas, il vous suffit de partager l’URL du webinaire avec le prospect. Cliquer sur le lien avant que le webinaire ne commence les envoie vers une page de destination précédant le webinaire. Cliquez dessus pendant le webinaire pour accéder au webinaire en cours. Cliquez dessus après le webinaire pour accéder à un enregistrement du webinaire.

## Jetons de webinaires interactifs {#interactive-webinars-tokens}

Utilisez des jetons pour promouvoir les webinaires interactifs dans les e-mails et les pages de destination sans avoir à ajouter manuellement les détails du webinaire. Cela améliore l’efficacité globale, car toutes les modifications apportées aux métadonnées du webinaire (telles que le titre du webinaire, la date de début, etc.) sont automatiquement répercutées dans vos ressources.

![](assets/promoting-an-interactive-webinar-3.png)

**Liste des jetons**

* program.webinarCapacity
* program.webinarDuration
* program.webinarEndDate
* program.webinarEndTime
* program.webinarGenericURL
* program.webinarLanguage
* program.webinarStartDate
* program.webinarStartTime
* program.webinarTimezone
* program.webinarTitle
