---
unique-page-id: 2359494
description: Utiliser le test A/B "Objet" - Documents Marketo - Documentation du produit
title: Utiliser le test A/B "Objet"
exl-id: 99c2415e-886b-44fa-ba96-5d4ec371753e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Utiliser le test A/B &quot;Objet&quot; {#use-subject-line-a-b-testing}

Vous pouvez facilement A/B tester vos emails. L’un des tests les plus courants est le suivant : **Objet** test.

>[!PREREQUISITES]
>
>[Ajout d’un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Sous la mosaïque Email , avec votre email sélectionné, cliquez sur Ajouter un test A/B.

![](assets/image2014-9-12-15-3a6-3a2.png)

1. La fenêtre de l’éditeur de test s’ouvre. Entrez un ou plusieurs nouveaux objets.

   >[!NOTE]
   >
   >Choix **A** prérenseignera les informations contenues dans l’email sélectionné.

   ![](assets/image2014-9-12-15-3a9-3a14.png)

   >[!TIP]
   >
   >Vous pouvez cliquer sur le bouton **+** pour ajouter d’autres objets.

1. Utilisez le curseur pour choisir le pourcentage de l’audience qui doit recevoir votre test A/B, puis cliquez sur **Suivant**.

   ![](assets/image2014-9-12-15-3a10-3a4.png)

   >[!CAUTION]
   >
   >**Nous vous recommandons d’éviter de définir la taille de l’échantillon sur 100 %.**. Si vous utilisez une liste statique, la définition de la taille de l’échantillon à 100 % enverrait l’email à tous les membres de l’audience et le gagnant ne serait envoyé à personne. Si vous utilisez une liste dynamique, définir la taille de l’échantillon sur 100 % enverrait l’email à tous les membres de l’audience. _à ce moment-là_. Et lorsque le programme de messagerie s’exécute à nouveau à une date ultérieure, toutes les nouvelles personnes qui remplissent les critères pour la liste dynamique recevront également l’email puisqu’elles sont désormais incluses dans l’audience.

   >[!NOTE]
   >
   >Les différentes variations d’objet prennent même certaines parties de la taille d’échantillon de test sélectionnée.

   D&#39;accord, nous y sommes presque. Maintenant nous devons [définir les critères de réussite du test A/B ;](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
