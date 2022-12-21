---
unique-page-id: 2359545
description: Définition des critères de gagnant de test A/B - Documents Marketo - Documentation du produit
title: Définition des critères de gagnant de test A/B
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
source-git-commit: 67ae4605d541a475b42a5094a5588c469a9d975d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 3%

---

# Définition des critères de gagnant de test A/B {#define-the-a-b-test-winner-criteria}

When [ajout d’un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;} dans votre programme de messagerie, vous devrez sélectionner un type de test, [Planification du test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}, puis définissez les critères de gagnant. Voici comment décider quel email gagne.

>[!PREREQUISITES]
>
>[Ajout d’un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;}

## Critères pour gagner {#winner-criteria}

1. La valeur par défaut **Critères de gagnant** sont répertoriées en premier.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>Ouvertures</b></td>
   <td>Une ouverture s’enregistre lorsque des images sont téléchargées dans un email. Même si vous n’incluez pas d’image, Marketo insère par défaut un seul pixel de suivi dans tous les emails de HTML.</td>
   </tr>
   <tr>
   <td><b>Clics</b></td>
   <td>Par défaut, le suivi des liens dans les emails est intégré dans les liens. Il permet de savoir qui a cliqué sur un lien, combien de liens ont été cliqués, etc.</td>
   </tr>
   <tr>
   <td><b>Clic pour ouverture %</b></td>
   <td>Pourcentage d'emails ouverts ayant fait l'objet d'un clic sur un lien dans l'email. Cela mesure la pertinence et le contexte d’un email en prenant le nombre de clics uniques divisé par le nombre d’ouvertures uniques, puis en le multipliant par 100 pour l’afficher en pourcentage.</td>
   </tr>
   <tr>
   <td><b>Évaluation de l’engagement</b></td>
   <td>Le <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">score d'engagement</a> vous aide à déterminer l’efficacité de votre contenu.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Si vous sélectionnez Score d’engagement , le test doit s’exécuter pendant au moins 24 heures. En savoir plus sur [compréhension du score d’engagement](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target=&quot;_blank&quot;}.

1. Vous pouvez également personnaliser vos critères en sélectionnant Conversion personnalisée et en cliquant sur Modifier.

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >La conversion personnalisée vous permet de sélectionner n’importe quel événement comme conversion à l’aide de déclencheurs et de filtres.

1. Une fenêtre s’ouvre. Recherchez le déclencheur de votre choix et faites-le glisser dans la zone de travail.

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. Définissez le déclencheur.

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketo n’autorise que les déclencheurs/filtres pour les personnes qui ont reçu l’e-mail de ce programme de messagerie. Il n’est donc pas nécessaire d’ajouter un filtre &quot;A été envoyé par e-mail&quot;. De plus, lorsque vous utilisez un déclencheur/filtre lié à un email, veillez à utiliser &quot;is any&quot; comme opérateur.

1. Cliquez sur **Fermer**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Fantastique ! Il est maintenant temps de décider comment le gagnant est déterminé.

## Déclarer gagnant {#declare-winner}

1. Sélectionnez l’une des deux options disponibles.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Si vous effectuez une **Date/heure** Test A/B, vous pouvez uniquement choisir **Manuel**.

   Une fois le test A/B terminé, Marketo peut envoyer automatiquement l’e-mail gagnant à l’heure planifiée, ou vous pouvez consulter les résultats et décider de l’envoi de l’e-mail.

1. Automatique est formidable et est l’option par défaut. Cliquez simplement sur **Suivant**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Choix **Manuel** envoie le test et attend que vous déclariez gagnant. Vous recevrez un rapport des résultats.

Mot clé! Maintenant, allons [Planification du test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}.
