---
unique-page-id: 2359520
description: Utiliser Les Tests A/B « Date/Heure » - Documents Marketo - Documentation Du Produit
title: Utiliser le test A/B « Date/Heure »
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
feature: Email Programs, A/B Testing
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 4%

---

# Utiliser le test A/B « Date/Heure » {#use-date-time-a-b-testing}

Vous pouvez facilement tester A/B vos e-mails. Un test est le test **[!UICONTROL Date/Heure]**. Cette option permet de tester l’heure ou le jour de la semaine où il est préférable d’envoyer des e-mails. Voici comment le configurer.

>[!PREREQUISITES]
>
>[Ajouter un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)
>

1. Sous la mosaïque **[!UICONTROL E-mail]**, cliquez sur **[!UICONTROL Ajouter un test A/B]**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Une nouvelle fenêtre s’ouvre. Sélectionnez **[!UICONTROL Date/Heure]** pour **[!UICONTROL Type de test]**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Si vous disposez d’informations de test précédentes (comme un test du sujet), vous pouvez cliquer en toute sécurité sur **[!UICONTROL Réinitialiser le test]**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Sélectionnez la date de votre première date/heure.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Sélectionnez l’heure de votre première date/heure.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Faites de même pour la deuxième date/heure.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Utilisez le curseur pour choisir le pourcentage d’audience souhaité dans votre test A/B, puis cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >Les différentes variations s&#39;appliqueront à des parties égales de la taille d&#39;échantillon d&#39;essai choisie.

   >[!CAUTION]
   >
   >**Nous vous recommandons d’éviter de définir la taille de l’échantillon sur 100 %**. Si vous utilisez une liste statique, la définition de la taille de l’échantillon sur 100 % envoie l’e-mail à tous les membres de l’audience et le gagnant n’est attribué à personne. Si vous utilisez une liste **intelligente**, la définition de la taille de l’échantillon sur 100 % envoie l’e-mail à toutes les personnes de l’audience _à ce moment-là_. Lorsque le programme de messagerie s’exécutera à nouveau à une date ultérieure, toutes les nouvelles personnes qui remplissent les critères de la liste dynamique recevront également le message électronique, car elles sont désormais incluses dans l’audience.

   D&#39;accord, nous nous rapprochons un peu. Maintenant, nous devons [définir les critères de gagnant du test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
