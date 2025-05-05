---
unique-page-id: 2359502
description: Utiliser le test A/B "Entier Email" - Documents Marketo - Documentation du produit
title: Utiliser le test A/B "E-mail entier"
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Utiliser le test A/B &quot;E-mail entier&quot; {#use-whole-email-a-b-testing}

Vous pouvez facilement A/B tester vos emails. Un bon test est le test **Entier Email**. Voici comment le mettre en place.

>[!PREREQUISITES]
>
>[Ajout d’un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Sous la mosaïque Email , avec votre email sélectionné, cliquez sur **Ajouter un test A/B**.

![](assets/image2014-9-12-15-3a22-3a12.png)

1. Une nouvelle fenêtre s’ouvre. Cliquez sur la liste déroulante **Type de test** et sélectionnez **Courriers électroniques complets**.

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

   [&#128279;](assets/image2014-9-12-15-3a23-3a49.png)

1. Cliquez sur **Ajouter** pour appliquer le second email. Faites glisser le curseur pour choisir le pourcentage de l’audience qui doit recevoir votre test A/B, puis cliquez sur **Suivant**.

   [&#128279;](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >Les différentes variations seront envoyées en parts égales de la **taille de l’échantillon de test** sélectionné.

   >[!CAUTION]
   >
   >**Nous vous recommandons d’éviter de définir la taille de l’échantillon sur 100 %**. Si vous utilisez une liste statique, la définition de la taille de l’échantillon à 100 % envoie l’email à tous les membres de l’audience et le gagnant n’envoie personne. Si vous utilisez une liste **smart**, la définition de la taille d’échantillon à 100 % envoie le courrier électronique à toutes les personnes de l’audience _à cette heure_. Lorsque le programme de messagerie s’exécute à nouveau à une date ultérieure, toutes les nouvelles personnes qui remplissent les critères pour la liste dynamique recevront également l’email puisqu’elles sont désormais incluses dans l’audience.

   D&#39;accord, nous y sommes presque. Maintenant, nous devons [définir les critères de gagnant du test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
