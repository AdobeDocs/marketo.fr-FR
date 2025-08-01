---
description: Service d’étape de flux - Documents Marketo - Documentation du produit
title: Étape de déroulement du service
exl-id: 81367562-8b27-4ec5-8a9b-b02083a2e999
feature: Smart Campaigns
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1233'
ht-degree: 0%

---

# Étape de déroulement du service {#flow-step-service}

Les étapes de flux en libre-service constituent une structure et un ensemble de fonctionnalités pour la création, la publication et l’intégration de services web dans les campagnes intelligentes Adobe Marketo Engage. Ce guide est destiné aux utilisateurs finaux de Marketo Engage qui souhaitent installer et utiliser des services qui ont déjà été créés et publiés. Pour plus d’informations sur la création et la publication de votre propre service, reportez-vous au référentiel [[!DNL GitHub]  de l’interface du fournisseur de services](https://github.com/adobe/Marketo-SSFS-Service-Provider-Interface){target="_blank"}. Une implémentation de table de recherche de preuve de concept est disponible [ici](https://github.com/adobe/mkto-flow-lookup){target="_blank"}.

## Intégration et gestion des services {#onboarding-and-managing-services}

L’installation d’une étape de flux personnalisé nécessite des autorisations d’administrateur dans Marketo. Outre l’URL d’installation, tous les autres aspects d’un service peuvent être modifiés après l’intégration initiale en accédant à l’écran des détails du service à partir de la grille des fournisseurs de services.

## URL d’installation {#installation-url}

Pour commencer l’installation, vous devez d’abord obtenir l’URL du document OpenAPI qui définit votre service. Votre fournisseur de services doit être en mesure de vous fournir cette adresse et dispose généralement d’une URL se terminant par `/openapi.json`. Les URL complètes ressembleront à `https://www.example.com/OpenAPI.json`. Une fois que vous disposez de cette URL, accédez au menu [!UICONTROL Fournisseurs de services] dans votre section [!UICONTROL Admin].

Cliquez sur **[!UICONTROL Suivant]** pour accéder à la section Saisie des informations d’identification de service.

![](assets/flow-step-service-1.png)

## Saisir les informations d’identification de service {#enter-service-credentials}

Pour accéder au service en cours d’installation, Marketo doit disposer d’informations d’identification d’API valides. Ces informations d’identification doivent vous être fournies par votre fournisseur de services. Les services disposent de trois options d’authentification différentes. Vous pouvez donc voir l’une des trois invites d’informations d’identification différentes : **Clé API** qui n’a qu’un champ d’entrée, **Authentification de base** qui nécessite un nom d’utilisateur et un mot de passe et qui peut également nécessiter un champ appelé Domaine, et **OAuth2** qui utilise l’octroi _Informations d’identification client_, qui nécessite un _Identifiant client_ et _Secret client_.

Lorsque vous enregistrez vos informations d’identification, Marketo tente d’appeler le point d’entrée de statut du service pour vérifier qu’elles sont valides. Si les informations d’identification fournies ne sont pas valides, une erreur s’affiche pour l’indiquer.

>[!CAUTION]
>
>Si un fournisseur de services est créé et supprimé, vous ne pourrez plus réutiliser son nom de fournisseur de services, d’API, de déclencheur ou de filtre.

## Guide D’Intégration (Facultatif) {#onboarding-guide}

Certains fournisseurs de services incluent une étape facultative Guide d’intégration . Cette étape comprend toutes les instructions supplémentaires pour terminer l’intégration du service qui sont spécifiques à ce service.

## Appariement des champs {#field-mapping}

Pour recevoir ou renvoyer des données d’un champ de prospect spécifique, ce champ doit être mappé. Bien que le mappage soit une étape obligatoire lors de l’intégration, vous pouvez toujours revenir pour modifier les mappages ultérieurement. Deux types de mappages sont configurés dans des écrans distincts : **Champs sortants**, qui sont envoyés au service lorsque Marketo appelle l’étape de flux, et **Champs entrants** qui sont des champs pouvant recevoir des données du service lorsqu’il renvoie des données à Marketo.

>[!NOTE]
>
>En mappant un champ sortant, vous donnez à Marketo l’autorisation de transmettre des données de ce champ liées aux prospects traités par le service associé. Assurez-vous que vous disposez de la capacité juridique et de l’autorité appropriées pour transmettre ces données à votre fournisseur de services, car ces champs peuvent inclure des informations d’identification personnelle couvertes par les lois sur la confidentialité, la protection et la location des données.

Les mappages de champs facultatifs peuvent être désactivés sans perturber votre service, mais les mappages requis peuvent ne pas être complètement supprimés ou désactivés.

## Mappages pilotés par les services {#service-driven-mappings}

Les services qui disposent d’un ensemble fixe d’entrées et de sorties, comme une étape de flux d’enregistrement d’événement, utilisent les **Mappages pilotés par les services**. Pour ce type de mappage, le fournisseur de services fournit un type de données et une astuce sous la forme d’un nom d’API. Si le conseil correspond au nom de l’API d’un champ de prospect existant, ce champ est automatiquement renseigné dans la section de mappage. Pour les champs sans conseil correspondant, vous devez renseigner manuellement le mappage à partir de la liste des champs avec le type de données correspondant. Les mappages obligatoires doivent être renseignés pour terminer l’intégration.

![](assets/flow-step-service-2.png)

## Mappages pilotés par l’utilisateur {#user-driven-mappings}

Les services qui n’ont pas d’ensemble fixe d’entrées et de sorties, comme un service de formatage de date, utilisent les **mappages pilotés par l’utilisateur**. Cela signifie que chaque champ entrant et sortant doit être configuré par un administrateur.

![](assets/flow-step-service-3.png)

## Champs sortants {#outgoing-fields}

Les champs sortants sont ceux qui sont envoyés au service d’étape de flux lorsque cette étape de flux est utilisée dans une campagne intelligente.

## Champs entrants {#incoming-fields}

Les champs entrants sont ceux dans lesquels le service d’étape de flux est autorisé à écrire des données.

## Options De Configuration (Facultatif) {#configuration-options}

Certains services disposent d’options de configuration globale facultatives ou obligatoires. Si des options sont requises, une valeur doit être définie pour toutes les options requises avant d’enregistrer ou de terminer l’intégration. Les paramètres dont les noms sont en italique sont envoyés au service appelé en tant qu’en-têtes.

![](assets/flow-step-service-4.png)

## Retrait d’un service {#retiring-a-service}

Pour faciliter les transitions vers de nouvelles versions ou des versions alternatives d’un service, sans interrompre l’utilisation active, les services peuvent être retirés du menu Fournisseurs de services. **Retrait d’un service** supprime l’étape de flux correspondante de la palette de flux de campagne intelligente afin qu’aucune nouvelle utilisation de celle-ci ne puisse être créée. Dans la plupart des cas, vous devriez avoir un service de remplacement prêt à remplacer le service existant lorsque vous choisissez de retirer un service.

## Obsolescence de service {#service-deprecation}

Parfois, les fournisseurs de services devront abandonner les services d’étape de flux dans le cadre du cycle de vie normal des logiciels. Lorsqu’un fournisseur de services l’annonce, la date d’obsolescence et le message sont renseignés dans la vue grille des fournisseurs de services. Si vous continuez à utiliser un service qui a été abandonné, il peut y avoir une interruption du service s’il ne répond plus de la manière prévue ou s’il cesse d’accepter des requêtes provenant de campagnes dynamiques Marketo. Vous devez donc prêter une attention particulière aux notifications d’obsolescence de service que vous recevez et prendre les mesures appropriées pour supprimer ou remplacer les étapes du service qui sont toujours en cours d’utilisation.

## Utilisation d’étapes de flux tierces et personnalisées {#using-third-party-and-custom-flow-steps}

Les étapes de flux installées peuvent être utilisées de la même manière que les étapes de flux standard. Tous les paramètres de flux définis par le service sont présentés aux utilisateurs finaux.

## Actualisation des listes de sélection {#refreshing-picklists}

Marketo actualisera les choix de la liste de sélection pour les services tous les soirs, mais il y a des moments où vous aurez besoin que de nouveaux choix soient disponibles, tels que la création de campagnes. Vous pouvez les actualiser facilement à partir de n’importe quelle instance de votre étape de flux à l’aide du bouton d’actualisation ou en accédant au menu [!UICONTROL Admin] > [!UICONTROL Fournisseurs de services] et en cliquant sur [!UICONTROL Actualiser la liste de sélection] une fois que vous avez sélectionné votre service.

## Vérification des champs entrants {#checking-incoming-fields}

Vous pouvez vérifier quels champs entrants sont configurés pour une étape de flux donnée en pointant sur son icône d’info-bulle. Cela s’avère utile pour déterminer les champs qui peuvent changer lorsqu’un prospect y circule, afin que vous puissiez configurer des choix lors des étapes suivantes à l’aide de ces champs.

![](assets/flow-step-service-5.png)

## Champs entrants et modifications de la valeur des données {#incoming-fields-and-data-value-changes}

Contrairement à la plupart des autres étapes de flux, celles implémentées avec le framework SSFS peuvent réécrire des données dans les champs de prospect mappés par un administrateur et enregistrer ces modifications en tant qu’activités de changement de valeur de données.  Lorsqu’une étape de flux écrit des données de cette manière, toutes ces modifications sont effectuées avant que la campagne intelligente ne passe aux étapes suivantes, de sorte que toute donnée écrite puisse être fiable dans les choix d’étape de flux suivants.

## Journaux et statistiques du service {#service-logs-and-statistics}

Chaque service d’étape de flux est associé à plusieurs types de journalisation pour surveiller l’intégrité et résoudre les problèmes liés à l’intégration.

## Service Statistics {#service-statistics}

Le journal des statistiques du service agrège les résultats des appels et des rappels pour chaque service. Ils sont regroupés par heure, niveau (bloc ou enregistrement) et code, et fournissent les nombres et le message de journal le plus récent pour chaque code reçu. Ce tableau de bord est principalement conçu pour faciliter la surveillance de l’intégrité des services.
