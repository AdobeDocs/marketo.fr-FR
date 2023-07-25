---
unique-page-id: 2359504
description: Utiliser le test A/B "From Address" - Documents Marketo - Documentation du produit
title: Utiliser le test A/B "A partir de l’adresse"
exl-id: 83e2994b-39ec-4c88-87b0-8f2501ea2bf1
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Utiliser le test A/B &quot;A partir de l’adresse&quot; {#use-from-address-a-b-testing}

Vous pouvez facilement A/B tester vos emails. Un test intéressant est le suivant : **Adresse de l’expéditeur** test. Voici comment le mettre en place.

>[!PREREQUISITES]
>
>[Ajout d’un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. Sous , **Email** avec votre email sélectionné, cliquez sur **Ajout d’un test A/B**.

   ![](assets/image2014-9-12-15-3a32-3a8.png)

1. Une nouvelle fenêtre s’ouvre, sélectionnez **Adresse de l’expéditeur** pour **Type de test**.

   ![](assets/image2014-9-12-15-3a32-3a22.png)

1. Si vous disposez d’informations de test précédentes (comme un test d’objet), vous pouvez cliquer en toute sécurité sur **Réinitialiser le test**.

   ![](assets/image2014-9-12-15-3a32-3a28.png)

1. Saisissez la seconde **Adresse de l’expéditeur** informations que vous souhaitez tester.

   >[!NOTE]
   >
   >Choix A : prérenseignera les informations contenues dans l’email sélectionné.

   ![](assets/image2014-9-12-15-3a32-3a34.png)

   >[!TIP]
   >
   >Vous pouvez cliquer sur le bouton **+** pour ajouter autant d’adresses de départ que vous le souhaitez.

1. Utilisez le curseur pour choisir le pourcentage d’audience souhaité dans votre test A/B, puis cliquez sur **Suivant**.

   ![](assets/image2014-9-12-15-3a33-3a41.png)

   >[!NOTE]
   >
   >Les différentes variations seront envoyées en parts égales de la taille de l’échantillon de test sélectionné.

   >[!CAUTION]
   >
   >**Nous vous recommandons d’éviter de définir la taille de l’échantillon sur 100 %.**. Si vous utilisez une liste statique, la définition de la taille de l’échantillon à 100 % envoie l’email à tous les membres de l’audience et le gagnant n’envoie personne. Si vous utilisez une **smart** liste, la définition de la taille d’échantillon à 100 % envoie l’email à tous les membres de l’audience _à ce moment-là_. Lorsque le programme de messagerie s’exécute à nouveau à une date ultérieure, toutes les nouvelles personnes qui remplissent les critères pour la liste dynamique recevront également l’email puisqu’elles sont désormais incluses dans l’audience.

   OK, nous y sommes presque. Maintenant nous devons [définir les critères de réussite du test A/B ;](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
