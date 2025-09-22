---
unique-page-id: 2359545
description: Définir les critères de gagnant du test A/B - Documents Marketo - Documentation du produit
title: Définir les critères de sélection du gagnant du test A/B
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 22%

---

# Définir les critères de sélection du gagnant du test A/B {#define-the-a-b-test-winner-criteria}

Lors de l’[ajout d’un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"} à votre programme d’e-mail, vous devez sélectionner un type de test, [planifier le test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}, puis définir les critères du gagnant. Voici comment choisir l’e-mail qui l’emportera.

>[!PREREQUISITES]
>
>[Ajouter un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## Critères pour gagner {#winner-criteria}

1. Les options par défaut **[!UICONTROL Critères du gagnant]** sont répertoriées en premier.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>[!UICONTROL Opens]</b></td>
   <td>Une ouverture s’enregistre lorsque des images sont téléchargées dans un e-mail. Même si vous n’incluez pas d’image, Marketo insère par défaut un seul pixel de tracking dans tous les emails HTML.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Clics]</b></td>
   <td>Par défaut, le tracking est intégré aux liens des e-mails. Vous pouvez ainsi voir qui a cliqué sur quel lien, combien de liens au total ont fait l’objet d’un clic, etc.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Cliquez pour ouvrir] %</b></td>
   <td>Pourcentage d’e-mails qui ont été ouverts et dans lesquels un lien a fait l’objet d’un clic. Cela permet de mesurer la pertinence et le contexte d’un e-mail en divisant le nombre de clics uniques par le nombre d’ouvertures uniques, puis en multipliant cette valeur par 100 pour l’afficher en pourcentage.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Engagement Score]</b></td>
   <td>Le <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank"> score d’engagement </a> vous aide à déterminer l’efficacité de votre contenu.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Si vous choisissez le score d’engagement , le test doit durer au moins 24 heures. En savoir plus sur la [compréhension du score d’engagement](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

1. Vous pouvez également personnaliser vos critères en sélectionnant **[!UICONTROL Conversion personnalisée]** et en cliquant sur **[!UICONTROL Modifier]**.

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >La conversion personnalisée vous permet de choisir n’importe quel événement en tant que conversion à l’aide de déclencheurs et de filtres.

1. Une fenêtre s’ouvre. Recherchez le déclencheur de votre choix et faites-le glisser dans la zone de travail.

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. Définissez le déclencheur.

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >Marketo autorise uniquement les déclencheurs/filtres pour les personnes à qui cet e-mail a été envoyé à partir de ce programme d’e-mail. Il n’est donc pas nécessaire d’ajouter un filtre « E-mail envoyé ». De plus, lors de l’utilisation d’un déclencheur/filtre lié aux e-mails, veillez à utiliser « is any » comme opérateur.

1. Cliquez sur **[!UICONTROL Fermer]**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Fantastique ! Il est maintenant temps de décider comment le gagnant est déterminé.

## Déclarer gagnant {#declare-winner}

1. Sélectionnez l’une des deux options disponibles.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Si vous effectuez un test A/B **Date/Heure**, vous pouvez uniquement choisir **[!UICONTROL Manuel]**.

   Une fois le test A/B terminé, Marketo peut envoyer automatiquement l’e-mail gagnant à l’heure planifiée. Vous pouvez également consulter les résultats et décider quel e-mail sera envoyé quand.

1. Automatique est génial et est l&#39;option par défaut. Cliquez simplement sur **[!UICONTROL Suivant]**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Choisir **[!UICONTROL Manuel]** enverra le test et attendra que vous déclariez un gagnant. Vous recevrez un rapport des résultats.

Parfait ! Maintenant, [planifier le test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}.
