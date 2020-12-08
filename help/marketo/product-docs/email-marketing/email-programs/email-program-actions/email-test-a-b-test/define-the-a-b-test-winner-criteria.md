---
unique-page-id: 2359545
description: Définir les critères de gagnant du test A/B - Documents marketing - Documentation du produit
title: Définition des critères de gagnant de test A/B
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# Définition des critères de gagnant de test A/B {#define-the-a-b-test-winner-criteria}

Lorsque vous [ajoutez un test](add-an-a-b-test.md) A/B à votre programme de messagerie, vous devez sélectionner un type de test, [planifier le test](schedule-the-a-b-test.md)A/B, puis définir les critères gagnants. Voici comment décider quel email gagne.

>[!NOTE]
>
>**Conditions préalables**
>
>* [Ajouter un test A/B](add-an-a-b-test.md)

>



## Critères de gagnant {#winner-criteria}

1. Les options de critères **** gagnants par défaut sont répertoriées en premier.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   | **Ouvre** | Un enregistrement ouvert s’enregistre lorsque des images sont téléchargées dans un courrier électronique. Même si vous n’incluez pas d’image, Marketo insère par défaut un pixel de suivi dans tous les courriers électroniques HTML. |
   |---|---|
   | **Clics** | Par défaut, le suivi des liens dans les courriels est intégré dans ces derniers, ce qui vous permet de savoir qui a cliqué sur un lien, combien de liens au total ont cliqué, etc. |
   | **Cliquez pour ouvrir le %** | Pourcentage de courriers électroniques ouverts et sur lesquels un lien a été cliqué dans le courrier électronique. Cela mesure la pertinence et le contexte d’un courriel en prenant le nombre de clics uniques divisé par le nombre d’ouvertures uniques, puis en le multipliant par 100 pour l’afficher sous forme de pourcentage. |
   | **Note d’engagement** | Le score [d’](http://docs.marketo.com/display/DOCS/Understanding+the+Engagement+Score) engagement vous permet de déterminer l’efficacité de votre contenu. |

   >[!TIP]
   >
   >Si vous sélectionnez Note d’engagement, le test doit s’exécuter pendant au moins 24 heures. En savoir plus sur la [compréhension de la note](../../../../../product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md)d’engagement.

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
   >En savoir plus sur les listes [intelligentes et les listes](http://docs.marketo.com/display/docs/smart+lists+and+static+lists)statiques.

   Définissez le déclencheur.
   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!NOTE]
   >
   >Marketo n&#39;autorisera que les déclencheurs pour les personnes qui ont reçu le courrier électronique de ce programme électronique. Il n’est pas nécessaire d’ajouter un filtre &quot;Courrier électronique envoyé&quot;.

   Cliquez sur Fermer.
   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Super ! Il est maintenant temps de décider comment le gagnant est déterminé.

## Déclarer gagnant {#declare-winner}

1. Choisissez l’une des deux options disponibles.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >
   >Si vous effectuez un test A/B **Date/Heure** , vous pouvez uniquement choisir **Manuel**.

   Une fois le test A/B terminé, Marketo peut envoyer automatiquement le courriel gagnant à l’heure planifiée, ou vous pouvez consulter les résultats et décider de l’envoi du courriel au moment de l’envoi.

1. Automatique est génial et est l&#39;option par défaut. Cliquez simplement sur **Suivant**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Le **guide** de sélection envoie le test et attend que vous déclariez gagnant. Vous recevrez un rapport des résultats.

   [planification du test A/B](schedule-the-a-b-test.md)

Parfait ! Maintenant, allons-y.