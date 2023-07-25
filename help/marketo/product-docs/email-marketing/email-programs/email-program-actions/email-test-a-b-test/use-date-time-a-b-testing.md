---
unique-page-id: 2359520
description: Utiliser le test A/B "Date/Heure" - Documents Marketo - Documentation du produit
title: Utiliser le test A/B "Date/Heure"
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
feature: Email Programs, A/B Testing
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Utiliser le test A/B &quot;Date/Heure&quot; {#use-date-time-a-b-testing}

Vous pouvez facilement A/B tester vos emails. Un test est le suivant : **Date/heure** test. Ceci teste l’heure ou le jour de la semaine idéal pour envoyer des emails. Voici comment le mettre en place.

>[!PREREQUISITES]
>
>[Ajout d’un test A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)
>

1. Sous , **Email** mosaïque, cliquez sur **Ajout d’un test A/B**.

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. Une nouvelle fenêtre s’ouvre. Sélectionner **Date/heure** pour **Type de test**.

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. Si vous disposez d’informations de test précédentes (comme un test d’objet), vous pouvez cliquer en toute sécurité sur **Réinitialiser le test**.

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. Sélectionnez la date de votre première date/heure.

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. Sélectionnez l’heure de votre première date/heure.

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. Faites de même pour votre deuxième date/heure.

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. Utilisez le curseur pour choisir le pourcentage d’audience souhaité dans votre test A/B, puis cliquez sur **Suivant**.

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >Les différentes variations s’appliquent à des portions égales de la taille d’échantillon de test choisie.

   >[!CAUTION]
   >
   >**Nous vous recommandons d’éviter de définir la taille de l’échantillon sur 100 %.**. Si vous utilisez une liste statique, la définition de la taille de l’échantillon à 100 % envoie l’email à tous les membres de l’audience et le gagnant n’envoie personne. Si vous utilisez une **smart** liste, la définition de la taille d’échantillon à 100 % envoie l’email à tous les membres de l’audience _à ce moment-là_. Lorsque le programme de messagerie s’exécute à nouveau à une date ultérieure, toutes les nouvelles personnes qui remplissent les critères pour la liste dynamique recevront également l’email puisqu’elles sont désormais incluses dans l’audience.

   Bon, on est à un pas de plus. Maintenant nous devons [définir les critères de réussite du test A/B ;](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md).
