---
title: compréhension-objectif-suivi-et-projections-inscriptions
description: Comprendre le suivi des objectifs et les inscriptions prévues
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---


# Comprendre le suivi des objectifs et les inscriptions prévues

<br> 

Après avoir [défini des objectifs](/help/sky/setting-event-goals.md)de événement et envoyé des invitations par le biais d’une campagne [](/help/sky/create-a-smart-campaign.md)intelligente, voici comment suivre la progression de votre objectif et comprendre les prédictions de Marketo.

>[!NOTE]
>
>Lorsqu’un programme de événement est créé dans l’expérience Marketo Classic, la date de début de événement est actuellement définie par défaut sur la date de création du événement. Étant donné que les inscriptions prévues tiennent compte du temps écoulé avant la date du début du événement, ces chiffres peuvent ne pas être exacts si la date du début et la date de création sont identiques (sauf si elles sont définies intentionnellement).

## Suivi des objectifs et inscriptions prévues

1. Vous trouverez les détails du suivi des objectifs dans l’onglet **[!UICONTROL Rapports]** de votre programme de événement. Dans cet exemple particulier, il y a 150 membres enregistrés jusqu&#39;à présent contre un objectif de 200 (75 %).

   ![Image un](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-1.png)

Vous verrez également vos inscriptions **[!UICONTROL projetées]** . Passez la souris sur l’icône d’informations pour afficher la ventilation de ce nombre par segment de probabilité.

![Image 2](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>Le graphique Participé et Supérieur reste vide jusqu’au jour du événement.

1. Cliquez sur la bascule Graphique pour passer à une ventilation de vos membres selon la probabilité d&#39;inscription. Vous verrez les pourcentages d&#39;inscription actuels pour chaque segment, par rapport au pourcentage moyen pour ce segment dans les derniers programmes.

   ![Image trois](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-3.png)

Tous les membres (inscrits et non encore inscrits) sont classés selon leur probabilité d&#39;inscription. Passez la souris sur l’icône d’informations pour voir comment ces catégories de probabilité sont définies.

![Image 4](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>Les numéros de prédiction sont mis à jour toutes les 24 heures jusqu&#39;au jour du événement. Tous les membres répertoriés comme _Traitement_ seront inclus dans le prochain cycle de calcul.

## Programmes similaires

Vous pouvez obtenir des informations sur votre événement actuel en observant comment des programmes similaires se sont comportés dans le passé. Cette section vous montre jusqu&#39;à 5 programmes similaires des 6 derniers mois, avec le nombre/pourcentage de membres _enregistrés_ ou plus.

Dans le calcul de programmes similaires, nous incluons les facteurs suivants, entre autres :

* Type de programme
* Canal programme
* Taille de l&#39;Audience
* Balises de programme
* Durée entre la création de événement et le début de événement
* Durée du événement

   ![Image 5](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommendations

En haut de la page Rapports, vous trouverez des recommandations pilotées par IA/ML en fonction de votre progression. Consultez régulièrement le site pour obtenir des conseils et des renseignements utiles !

![Image six](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-6.png)

## prédictions au niveau de la personne

Cliquez sur l&#39;onglet **[!UICONTROL Membres]** pour vue tous les membres de votre programme. Passez la souris sur les **[!UICONTROL barres Probabilité]** d&#39; **[!UICONTROL inscription ou Probabilité de]** participationpour afficher les pourcentages et les catégories exacts. Vous pouvez ensuite agir sur les membres d&#39;une catégorie particulière (par exemple, tous les membres du groupe &quot;Moins susceptibles&quot; d&#39;enregistrer la catégorie) et, plus précisément, les cibles à augmenter éventuellement vos numéros d&#39;inscription.

![Image sept](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>La probabilité individuelle tient compte de plus de 40 facteurs liés à la personne, y compris les attributs de profil, l&#39;activité de la personne et les activités précédentes invitées/enregistrées/assistées.

## FAQ

**Q : Quel est le segment ?**

A : L’enregistrement est susceptible d’être effectué sur une valeur comprise entre 0 et 100. Chaque personne qui est membre du programme de événement obtiendra une valeur de probabilité comprise entre 0 et 100.

Les valeurs de probabilité sont regroupées en trois segments :

* Probabilité d&#39;inscription > 50 % = segment hautement probable
* Probabilité d&#39;inscription > 25 % à &lt;50 % = Segment probable
* Probabilité d&#39;inscription &lt; 25 % = segment moins probable

Lorsqu&#39;une personne a la probabilité de s&#39;inscrire, la prédiction tombera dans l&#39;un de ces segments (chaque personne qui est membre d&#39;un programme tombera dans l&#39;un d&#39;eux). Par exemple, si un programme de événement compte 1000 membres sur la base des prévisions de probabilité, ces 1000 seront répartis dans des segments _hautement probables_, _probables_ ou _moins probables_ .

Par conséquent, les personnes qui entrent dans le segment à haut risque auront plus de chances de s&#39;inscrire au événement.

Conversion pour s’inscrire = Nombre de personnes dans le segment enregistrées divisé par le nombre de personnes qui entrent dans le segment (par exemple, si 100 personnes entrent dans le segment Très probables et 60 d’entre elles s’inscrivent, le taux de conversion est de 60 %).

Le % de conversion à enregistrer suit ce modèle : Très probable > Probable > Moins probable.

**Q : Comment utiliser les statistiques ?**

A : Les meilleures pratiques comportent les éléments suivants :

i. Vous créez un programme, puis un Campaign intelligent utilise des filtres prédictifs avec &quot;plus de X&quot;, ce qui entraînerait un certain nombre de personnes (disons 1000) et vous exécutez la campagne.

ii. Au bout de 24 heures, dans l’onglet [!UICONTROL Rapports] , vous pouvez afficher les inscriptions prévues qui sont calculées en fonction de la probabilité d’enregistrer les valeurs de toutes les personnes actuellement invitées.

iii. Si les inscriptions prévues sont inférieures à l’objectif, vous devrez inviter plus de personnes. A ce stade, vous pouvez voir les informations qui vous disent quel était le seuil qui a fonctionné dans les programmes précédents.

![Image huit](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-8.png)

iv. Vous pouvez créer une Campaign intelligente avec ce seuil pour inviter davantage de personnes.

v. À tout moment, si vous souhaitez comprendre pourquoi un nombre prévu s’affiche, vous pouvez basculer pour afficher la répartition des audiences entre les segments, leurs taux de conversion du passé, et appliquer ces taux de conversion à l’audience actuelle (voir capture d’écran ci-dessous).

**Q : Quel est le graphique Segments par inscription ?**

A : Trois barres, chacune représentant un segment (Hautement Probable, Probable, Moins Probable).

**Ligne en pointillé violet :** Taux moyen de conversion à l’inscription dans ce segment, en fonction des programmes similaires précédents.

**Barre bleue :** Pourcentage d&#39;inscription de toutes les personnes de ce segment.

![Image neuf](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-9.png)

Par exemple, disons que 100 personnes ont une probabilité d&#39;inscription > 50 % et 60 sur ces 100 personnes enregistrées. Il est très probable que la conversion soit de 60 %. Ainsi, tous les membres ajoutés au programme ont la probabilité d&#39;enregistrer des valeurs, puis ils sont placés dans des segments et selon le nombre de personnes enregistrées dans chaque taux de conversion de segment est calculé.

**Q : Que signifie &quot;Enregistré et supérieur&quot; ?**

A : Toute personne inscrite sur la liste, ou tout autre statut ayant un numéro égal ou supérieur.

Vous pouvez créer de nouveaux états de progression pour un programme de événement, mais nous les mappons avec des états standard. Prenons le cas où une personne est déplacée d&#39;une invitation à un rappel, ce qui représente une étape supérieure à l&#39;enregistrement. Cette personne sera également considérée comme enregistrée et indiquée dans le suivi des objectifs.

![Image dix](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-10.png)

**Q : Comment les inscriptions prévues sont-elles calculées ?**

A : Voir ci-dessous.

![Image onze](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-11.png)
