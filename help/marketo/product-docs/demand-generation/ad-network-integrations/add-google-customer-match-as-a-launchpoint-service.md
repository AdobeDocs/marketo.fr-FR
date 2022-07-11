---
unique-page-id: 12980661
description: Ajout de la correspondance client Google en tant que service LaunchPoint - Documents Marketo - Documentation du produit
title: Ajout de la correspondance client Google en tant que service LaunchPoint
exl-id: c780bde0-3044-4c89-a2ac-88398cbc3425
source-git-commit: fb4e51a45fafaad547a641c6df5bb48cf536490d
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 2%

---

# Ajout de la correspondance client Google en tant que service LaunchPoint {#add-google-customer-match-as-a-launchpoint-service}

Avec cette intégration, vous pouvez envoyer une audience Marketo à Google pour qu’elle soit ciblée à l’aide de Google AdWords, ainsi que re-cibler les audiences dans YouTube, Search et Gmail.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Accédez à **Administration**.

   ![](assets/admin.png)

1. Cliquez sur **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Sélectionner **Nouveau** then **Nouveau service**.

   ![](assets/image2014-12-5-14-3a37-3a33.png)

1. Saisissez un **Nom d’affichage** et sélectionnez **Correspondance client Google** de la **Service** menu déroulant. Cliquez sur **Créer**.

   ![](assets/chooseservice.png)

1. Pour connecter un compte Google AdWords, cliquez sur **Autoriser**.

   ![](assets/authorizeaccount-1.png)

1. Google s’ouvre dans un nouvel onglet. À partir de là, connectez-vous à votre compte Google AdWords.

   >[!CAUTION]
   >
   >Pour que Marketo puisse envoyer des audiences sur plusieurs comptes AdWords, l’utilisateur Google que vous autorisez aux étapes suivantes doit avoir accès à _all_ de ces comptes.

   ![](assets/chooseaccount.png)

1. Vérifiez les autorisations demandées, puis cliquez sur **Autoriser**.

   ![](assets/reviewpermissions.png)

1. Votre compte Google AdWords est maintenant connecté à Marketo. Cliquez sur **Créer**.

   ![](assets/authorizesuccess.png)

   Super ! Les audiences mappées Google sont désormais répertoriées comme un service LaunchPoint dans l’onglet Services installés .

>[!NOTE]
>
>L’intégration de la correspondance client Google ne peut accueillir qu’un seul compte de gestionnaire et tous les sous-comptes de ce compte de gestionnaire. Plusieurs comptes de gestionnaire ne sont pas pris en charge.
