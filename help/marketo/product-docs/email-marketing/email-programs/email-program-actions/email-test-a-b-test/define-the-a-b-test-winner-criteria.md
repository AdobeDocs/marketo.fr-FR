---
unique-page-id: 2359545
description: Définir les critères de gagnant du test A/B - Documents marketing - Documentation du produit
title: Définition des critères de gagnant de test A/B
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Définir les critères de gagnant du test A/B {#define-the-a-b-test-winner-criteria}

Lorsque [vous ajoutez un test A/B](add-an-a-b-test.md) à votre programme de messagerie, vous devez sélectionner un type de test, [planifier le test A/B](schedule-the-a-b-test.md), puis définir les critères gagnants. Voici comment décider quel email gagne.

>[!PREREQUISITES]
>
>* [Ajouter un test A/B](add-an-a-b-test.md)

>



## Critères de gagnant {#winner-criteria}

1. Les options **Critères de gagnant** par défaut sont répertoriées en premier.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   | **Ouvre** | Un enregistrement ouvert s’enregistre lorsque des images sont téléchargées dans un courrier électronique. Même si vous n’incluez pas d’image, Marketo insère par défaut un pixel de suivi dans tous les courriers électroniques HTML. |
   |---|---|
   | **Clics** | Par défaut, le suivi des liens dans les courriels est intégré dans ces derniers, ce qui vous permet de savoir qui a cliqué sur un lien, combien de liens au total ont cliqué, etc. |
   | **Cliquez pour ouvrir le %** | Pourcentage de courriers électroniques ouverts et sur lesquels un lien a été cliqué dans le courrier électronique. Cela mesure la pertinence et le contexte d’un courriel en prenant le nombre de clics uniques divisé par le nombre d’ouvertures uniques, puis en le multipliant par 100 pour l’afficher sous forme de pourcentage. |
   | **Note d’engagement** | Le [score d&#39;engagement](http://docs.marketo.com/display/DOCS/Understanding+the+Engagement+Score) vous aide à déterminer l&#39;efficacité de votre contenu. |

   >[!TIP]
   >
   >Si vous sélectionnez Note d’engagement, le test doit s’exécuter pendant au moins 24 heures. En savoir plus sur [la compréhension du score d&#39;engagement](../../../../../product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md).

   Vous pouvez également personnaliser vos critères en sélectionnant Conversion personnalisée et en cliquant sur Modifier.
   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >La conversion personnalisée vous permet de sélectionner n’importe quel événement comme conversion en utilisant des déclencheurs et des filtres.

   Une fenêtre s&#39;ouvre. Recherchez le déclencheur de votre choix et faites-le glisser dans la trame.
   ![](assets/image2014-9-12-15-3a52-3a18.png)

   >[!NOTE]
   >
   >**Plongée profonde**
   >
   >
   >En savoir plus sur [les listes dynamiques et les listes statiques](http://docs.marketo.com/display/docs/smart+lists+and+static+lists).

   Définissez le déclencheur.
   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!NOTE]
   >
   >Marketo n&#39;autorisera que les déclencheurs pour les personnes qui ont reçu le courrier électronique de ce programme électronique. Il n’est pas nécessaire d’ajouter un filtre &quot;Courrier électronique envoyé&quot;.

   Cliquez sur Fermer.
   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Super ! Il est maintenant temps de décider comment le gagnant est déterminé.

## Déclarer le gagnant {#declare-winner}

1. Choisissez l’une des deux options disponibles.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >
   >Si vous effectuez un test A/B **Date/Heure**, vous pouvez uniquement choisir **Manuel**.

   Une fois le test A/B terminé, Marketo peut envoyer automatiquement le courriel gagnant à l’heure planifiée, ou vous pouvez consulter les résultats et décider de l’envoi du courriel au moment de l’envoi.

1. Automatique est génial et est l&#39;option par défaut. Cliquez simplement sur **Suivant**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Si vous choisissez **Manuel**, le test sera envoyé et vous attendrez que vous déclariez gagnant. Vous recevrez un rapport des résultats.

   [planification du test A/B](schedule-the-a-b-test.md)

Parfait ! Maintenant, allons-y.