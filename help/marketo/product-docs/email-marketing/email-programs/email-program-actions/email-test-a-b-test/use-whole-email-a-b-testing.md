---
unique-page-id: 2359502
description: Utiliser le test A/B "Entier Email" - Documents Marketo - Documentation du produit
title: Utiliser le test A/B "E-mail entier"
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Utiliser le test A/B &quot;E-mail entier&quot; {#use-whole-email-a-b-testing}

Vous pouvez facilement A/B tester vos emails. Un grand test est le suivant : **Courrier électronique complet** test. Voici comment le mettre en place.

>[!PREREQUISITES]
>
>[Ajout d’un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Sous la mosaïque Email , lorsque votre email est sélectionné, cliquez sur **Ajout d’un test A/B**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. Une nouvelle fenêtre s’ouvre. Cliquez sur le bouton **Type de test** et sélectionnez **Emails complets**.

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. Si vous disposez d’informations de test précédentes (comme un test d’objet), vous pouvez cliquer en toute sécurité sur **Réinitialiser le test**.

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. Sélectionnez votre premier email.

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. Cliquez sur **Ajouter** pour appliquer l’email.

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >Vous pouvez ajouter plusieurs emails. Si vous en ajoutez trop, toutefois, cela peut ralentir considérablement le processus de test.

1. Sélectionnez votre deuxième email.

   [](assets/image2014-9-12-15-3a23-3a49.png)

1. Cliquez sur **Ajouter** pour appliquer le deuxième email. Faites glisser le curseur pour choisir le pourcentage de l’audience qui doit recevoir votre test A/B, puis cliquez sur **Suivant**.

   [](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >Les différentes variations seront envoyées en parts égales de la sélection **Test Sample Size**.

   >[!CAUTION]
   >
   >**Nous vous recommandons d’éviter de définir la taille de l’échantillon sur 100 %.**. Si vous utilisez une liste statique, la définition de la taille de l’échantillon à 100 % envoie l’email à tous les membres de l’audience et le gagnant n’envoie personne. Si vous utilisez une **smart** liste, la définition de la taille d’échantillon à 100 % envoie l’email à tous les membres de l’audience _à ce moment-là_. Lorsque le programme de messagerie s’exécute à nouveau à une date ultérieure, toutes les nouvelles personnes qui remplissent les critères pour la liste dynamique recevront également l’email puisqu’elles sont désormais incluses dans l’audience.

   D&#39;accord, nous y sommes presque. Maintenant nous devons [définir les critères de réussite du test A/B ;](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
