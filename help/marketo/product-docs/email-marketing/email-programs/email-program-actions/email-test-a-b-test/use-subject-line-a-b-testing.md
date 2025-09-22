---
unique-page-id: 2359494
description: Utiliser Les Tests A/B « Ligne D’Objet » - Documents Marketo - Documentation Du Produit
title: Utiliser le test A/B « ligne d’objet »
exl-id: 99c2415e-886b-44fa-ba96-5d4ec371753e
feature: Email Programs, A/B Testing
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 5%

---

# Utiliser le test A/B « ligne d’objet » {#use-subject-line-a-b-testing}

Vous pouvez facilement tester A/B vos e-mails. L’un des tests les plus courants est le test **[!UICONTROL Objet]**.

>[!PREREQUISITES]
>
>[Ajouter un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Sous la mosaïque **[!UICONTROL E-mail]**, une fois votre adresse e-mail sélectionnée, cliquez sur **[!UICONTROL Ajouter un test A/B]**.

![](assets/image2014-9-12-15-3a6-3a2.png)

1. La fenêtre de l’éditeur de test s’ouvre. Saisissez une ou plusieurs nouvelles lignes d&#39;objet.

   >[!NOTE]
   >
   >L’option **A** sera préremplie avec les informations contenues dans l’e-mail sélectionné.

   ![](assets/image2014-9-12-15-3a9-3a14.png)

   >[!TIP]
   >
   >Vous pouvez cliquer sur **+** pour ajouter d&#39;autres lignes d&#39;objet.

1. Utilisez le curseur pour choisir le pourcentage de l’audience qui doit recevoir votre test A/B, puis cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2014-9-12-15-3a10-3a4.png)

   >[!CAUTION]
   >
   >**Nous vous recommandons d’éviter de définir la taille de l’échantillon sur 100 %**. Si vous utilisez une liste statique, définir la taille de l’échantillon sur 100 % enverrait l’e-mail à tous les membres de l’audience et le gagnant n’irait à personne. Si vous utilisez une liste dynamique, la définition de la taille de l’échantillon sur 100 % envoie l’e-mail à toutes les personnes de l’audience _à ce moment-là_. Et lorsque le programme de messagerie s’exécutera à nouveau à une date ultérieure, toutes les nouvelles personnes qui remplissent les critères de la liste dynamique recevront également le message électronique, car elles sont désormais incluses dans l’audience.

   >[!NOTE]
   >
   >Les différentes variations d’objet prennent des parties paires de la taille d’échantillon de test sélectionnée.

   On y est presque. Maintenant, nous devons [définir les critères de gagnant du test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
