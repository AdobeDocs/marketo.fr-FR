---
description: Présentation du suivi des objectifs et des inscriptions prévues - Documents Marketo - Documentation du produit
title: Comprendre le suivi des objectifs et les inscriptions prévues
hide: true
hidefromtoc: true
source-git-commit: ab20d9683aa5987778970fd32793dc0f3056c84b
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---

# Comprendre le suivi des objectifs et les inscriptions prévues {#understanding-goal-tracking-and-projected-registrations}

Après [définition des objectifs d’événement](/help/marketo/product-docs/marketo-sky/setting-event-goals.md) et envoyer des invitations par le biais d’un [campagne dynamique](/help/sky/create-a-smart-campaign.md), voici comment suivre la progression de votre objectif et comprendre les prédictions de Marketo.

>[!NOTE]
>
>Lorsqu’un programme d’événement est créé dans l’expérience Marketo Classic, la date de début de l’événement est actuellement définie par défaut sur la date de création de l’événement. Étant donné que les inscriptions prévues prennent en compte le temps qui précède la date de début d’un événement, ces chiffres peuvent ne pas être précis si la date de début et la date de création sont identiques (sauf si elles sont définies intentionnellement).

## Suivi des objectifs et enregistrements prévus {#goal-tracking-and-projected-registrations}

1. Vous trouverez les détails du suivi des objectifs dans la variable **[!UICONTROL Rapports]** de votre programme d’événements. Dans cet exemple particulier, il y a jusqu’à présent 150 membres enregistrés par rapport à un objectif de 200 (75 %).

   ![Image 1](assets/understanding-goal-tracking-and-projected-registrations-1.png)

Vous verrez également votre **[!UICONTROL Prévu]** inscriptions. Passez la souris sur l’icône d’information pour afficher une ventilation de ce nombre par segment Probabilité .

![Image 2](assets/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>Les graphiques Participant et Supérieur restent vides jusqu’au jour de l’événement.

1. Cliquez sur le bouton d’activation/désactivation Graphique pour passer à une ventilation de vos membres selon la probabilité d’inscription. Vous verrez les pourcentages d’enregistrement actuels pour chaque segment, par rapport au pourcentage moyen pour ce segment dans vos programmes précédents.

   ![Image trois](assets/understanding-goal-tracking-and-projected-registrations-3.png)

Tous les membres (enregistrés et non encore enregistrés) sont classés en fonction de leur probabilité d’enregistrement. Passez la souris sur l’icône d’information pour voir comment ces catégories de probabilité sont définies.

![Image Quatre](assets/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>Les numéros de prédiction sont mis à jour toutes les 24 heures jusqu’au jour de l’événement. Tous les membres répertoriés comme _Traitement_ sera inclus dans le prochain cycle de calcul.

## Programmes similaires {#similar-programs}

Vous pouvez mieux comprendre votre événement actuel en observant les performances passées de programmes similaires. Cette section vous présente jusqu’à 5 programmes similaires des 6 derniers mois, avec le nombre/pourcentage de membres qui étaient _Inscrits_ ou supérieur.

Dans le calcul de programmes similaires, nous incluons les facteurs suivants, entre autres :

* Type de programme
* Canal programme
* Taille d’audience
* Balises de programme
* Durée de la création de l’événement au début de l’événement
* Durée de l’événement

   ![Image 5](assets/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommandations {#recommendations}

En haut de la page Rapports, vous trouverez des recommandations pilotées par l’IA/ML en fonction de votre progression. Revenez régulièrement pour obtenir des conseils et des informations utiles.

![Image six](assets/understanding-goal-tracking-and-projected-registrations-6.png)

## Prédictions au niveau de la personne {#person-level-predictions}

Cliquez sur le bouton **[!UICONTROL Membres]** pour afficher tous les membres du programme. Passez la souris sur le **[!UICONTROL Probabilité d’enregistrement]** ou **[!UICONTROL Probabilité de présence]** pour afficher les pourcentages et les catégories exacts. Vous pouvez ensuite agir sur les membres d’une catégorie spécifique (par exemple, tous les membres de la catégorie &quot;Moins susceptibles&quot; d’enregistrer) et les cibler spécifiquement pour augmenter éventuellement vos numéros d’inscription.

![Image sept](assets/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>La probabilité individuelle prend en compte plus de 40 facteurs liés à la personne, y compris les attributs de profil, l’activité de la personne et les activités passées d’invité/enregistré/assisté.

## FAQ {#faq}

**Q : Qu’est-ce que le segment ?**

A : L’enregistrement probable est une valeur comprise entre 0 et 100. Chaque personne membre du programme d’événement aura une valeur de probabilité comprise entre 0 et 100.

Nous plaçons les valeurs de probabilité dans trois segments :

* Probabilité d’enregistrement > 50 % = segment hautement probable
* Probabilité d’enregistrer plus de 25 % à &lt;50 % = Segment probable
* Probabilité d’enregistrer &lt;25 % = segment moins probable

Lorsqu’une personne a de la probabilité de s’inscrire, la prédiction tombera dans l’un de ces segments (chaque personne qui est membre d’un programme tombera dans l’un d’entre eux). Par exemple, si un programme d’événement comporte 1 000 membres en fonction des prévisions de probabilité, ces 1 000 seront distribués dans _Très probable_, _Probable_ ou _Moins probable_ segments.

Par conséquent, les personnes qui appartiennent au segment à haut risque auront plus de chances de s’inscrire à l’événement.

Conversion pour s’inscrire = nombre de personnes dans le segment enregistré divisé par le nombre de personnes qui font partie du segment (par exemple, si 100 personnes appartiennent au segment hautement probable et que 60 d’entre elles s’inscrivent, le taux de conversion est de 60 %).

Le % de conversion à enregistrer suit ce modèle : Très probable > Probable > Moins probable.

**Q : Comment utiliser les insights ?**

A : Les bonnes pratiques comportent les éléments suivants :

i. Vous créez un programme, puis une campagne dynamique utilise des filtres prédictifs avec &quot;plus de X&quot;, ce qui entraînerait un certain nombre de personnes (disons 1 000) et vous exécutez la campagne.

ii. Après 24 heures, dans la variable [!UICONTROL Rapports] vous pouvez voir les enregistrements prévus qui sont calculés en fonction de la probabilité d’enregistrer les valeurs de toutes les personnes actuellement invitées.

iii. Si les enregistrements prévus sont inférieurs à l’objectif, vous devez inviter plus de personnes. À ce stade, vous pouvez voir les informations qui vous disent quel seuil a été celui qui a fonctionné dans les programmes précédents.

![Image huit](assets/understanding-goal-tracking-and-projected-registrations-8.png)

iv. Vous pouvez créer une nouvelle campagne dynamique avec ce seuil pour inviter plus de personnes.

v. À tout moment, si vous souhaitez comprendre pourquoi un nombre prévu s’affiche, vous pouvez basculer pour afficher la distribution de l’audience entre les segments, leurs taux de conversion du passé, et appliquer ces taux de conversion à l’audience actuelle (voir la capture d’écran ci-dessous).

**Q : Qu’est-ce que le graphique Segments par enregistrement ?**

A : Trois barres représentent chacune un segment (très probable, probable, moins probable).

**Ligne pointillée violette :** Taux de conversion moyen à l’enregistrement dans ce segment, en fonction des programmes similaires passés.

**Barre bleue :** Pourcentage d’enregistrement de toutes les personnes dans ce segment.

![Image neuf](assets/understanding-goal-tracking-and-projected-registrations-9.png)

Par exemple, supposons que 100 personnes ont une probabilité d’enregistrement supérieure à 50 % et 60 sur ces 100 personnes enregistrées. La conversion est très probablement de 60 %. Ainsi, tous les membres ajoutés au programme ont la probabilité d’enregistrer des valeurs, puis ils sont placés dans des segments et selon le nombre de personnes enregistrées dans chaque taux de conversion de segment est calculé.

**Q : Que signifie &quot;Registered and Higher&quot; ?**

A : Toute personne répertoriée comme enregistrée ou tout autre statut ayant un numéro égal ou supérieur à l’étape.

Vous pouvez créer de nouveaux statuts de progression pour un programme d’événements, mais nous les associons à des statuts standard. Prenons le cas où une personne est déplacée d’une personne invitée à un rappel, ce qui est une étape plus élevée que l’enregistrement. Cette personne sera également considérée comme enregistrée et affichée dans le suivi de l’objectif.

![Image dix](assets/understanding-goal-tracking-and-projected-registrations-10.png)

**Q : Comment sont calculés les inscriptions prévues ?**

A : Voir ci-dessous.

![Image Eleven](assets/understanding-goal-tracking-and-projected-registrations-11.png)
