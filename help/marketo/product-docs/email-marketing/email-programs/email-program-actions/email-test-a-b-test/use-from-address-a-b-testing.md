---
unique-page-id: 2359504
description: Découvrez comment exécuter des tests A/B depuis l’adresse. Testez différentes adresses d'expéditeur et choisissez un gagnant par performance.
title: Utiliser les tests AB « Adresse d’expédition »
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
TQID: 'https://experienceleague.adobe.com/rerG-Wyn1X53QQBDXFwyg74uEOznGcYcBis9EwX4vQU'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: 69a7f8d6-582c-5b66-841e-32cf07fd164c
    internal-label: A/B Testing
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: c0f0afc1-a5a8-4b01-8b43-cc38f9169499
    internal-label: Email programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 2%
---
# Utiliser Le Test A/B « [!UICONTROL Adresse De L’Expéditeur] » {#use-from-address-a-b-testing}

Vous pouvez facilement tester A/B vos e-mails. Un test intéressant est le test **[!UICONTROL Adresse d’origine]**. Voici comment le configurer.

>[!PREREQUISITES]
>
>[Ajouter un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Sous la mosaïque **[!UICONTROL E-mail]**, une fois votre e-mail sélectionné, cliquez sur **[!UICONTROL Ajouter un test A/B]**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Une nouvelle fenêtre s’ouvre. Sélectionnez **[!UICONTROL Adresse de l’expéditeur]** pour **[!UICONTROL Type de test]**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Si vous disposez d’informations de test précédentes (comme un test du sujet), vous pouvez cliquer en toute sécurité sur **[!UICONTROL Réinitialiser le test]**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Saisissez la deuxième information **[!UICONTROL Adresse de l&#39;expéditeur]** que vous souhaitez tester.

   >[!NOTE]
   >
   >L’option A sera préremplie avec les informations contenues dans l’e-mail sélectionné.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Vous pouvez cliquer sur le **+** pour ajouter autant d&#39;adresses d&#39;expédition que vous le souhaitez.

1. Utilisez le curseur pour choisir le pourcentage d’audience souhaité dans votre test A/B, puis cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Les différentes variations sont envoyées à des parties égales de la taille d’échantillon de test choisie.

   >[!CAUTION]
   >
   >**Nous vous recommandons d’éviter de définir la taille de l’échantillon sur 100 %**. Si vous utilisez une liste statique, la définition de la taille de l’échantillon sur 100 % envoie l’e-mail à tous les membres de l’audience et le gagnant n’est attribué à personne. Si vous utilisez une liste **intelligente**, la définition de la taille de l’échantillon sur 100 % envoie l’e-mail à toutes les personnes de l’audience _à ce moment-là_. Lorsque le programme de messagerie s’exécutera à nouveau à une date ultérieure, toutes les nouvelles personnes qui remplissent les critères de la liste dynamique recevront également le message électronique, car elles sont désormais incluses dans l’audience.

   OK, on y est presque. Maintenant, nous devons [définir les critères de gagnant du test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
