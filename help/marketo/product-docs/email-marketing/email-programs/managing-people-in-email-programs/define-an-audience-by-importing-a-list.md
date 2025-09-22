---
unique-page-id: 1900597
description: Définir une audience en important une liste - Documents Marketo - Documentation du produit
title: Définir une audience en important une liste
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 14%

---

# Définir une audience en important une liste {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[Créer un e-mail pour un programme de messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Une fois que vous avez créé un programme de messagerie, vous pouvez lui indiquer à qui envoyer l’e-mail. Vous pouvez le faire en [créant une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) ou en important une liste. Pour ce faire, importez une liste.

>[!NOTE]
>
>La définition de votre audience ne fonctionne que lorsque le programme de messagerie n’est pas approuvé.
>
>Tous les champs de date et d’heure importés sont traités comme des champs d’heure du Centre. Si vous avez des champs de date/heure dans un autre fuseau horaire, vous pouvez utiliser une formule Excel pour les transformer en heure du Centre (Amérique/Chicago).

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Sélectionnez votre programme de messagerie, puis cliquez sur **[!UICONTROL Importer la liste]** sous la mosaïque **[!UICONTROL Audience]**.

   ![](assets/importlist.png)

1. La fenêtre d’importation de liste s’ouvre, cliquez sur **[!UICONTROL Parcourir]** et sélectionnez le fichier à importer. Une fois la liste des personnes sélectionnée, cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Assurez-vous que la liste est codée au format UTF-8, UTF-16, Shift-JIS ou EUC-JP et que la taille du fichier ne dépasse pas 50 Mo.

1. Vérifiez que les champs de votre fichier sont correctement mappés et cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo se souviendra des mappages pour les importations futures !

1. Saisissez un **[!UICONTROL Nom]** pour votre liste, puis cliquez sur **[!UICONTROL Importer]**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Une fois l’importation terminée, revenez à l’onglet principal du programme. Vous verrez combien de personnes seront admissibles.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Définition**
>
>Avez-vous remarqué le numéro bloqué ? Ce numéro est un sous-ensemble des personnes qualifiées et représente les personnes qui ne peuvent pas recevoir cet e-mail car elles sont :
>
>* Désabonné ou désabonnée
>* Marketing interrompu
>* Figurant sur la liste bloquée
>* E-mail non valide
>* Empty Email
>
>Cliquez sur le numéro pour obtenir une liste détaillée des personnes bloquées dans le publipostage.
>
>Utilisez le bouton ![-](assets/image2014-10-23-16-3a32-3a36-1.png) sur la mosaïque **[!UICONTROL Audience]** pour voir combien de personnes ont rempli les critères de réception de l’e-mail en fonction des critères de liste dynamique. Soustrayez le nombre Bloqué du nombre Personnes pour obtenir le nombre total de personnes qui recevront l’e-mail.

>[!TIP]
>
>Il n’est pas nécessaire d’attendre la fin de l’import de la liste. Tu peux continuer à travailler si tu veux.

Fantastique ! Il est maintenant temps de choisir un e-mail existant ou de créer un e-mail à envoyer à ces personnes.

>[!MORELIKETHIS]
>
>* [Choisir un e-mail existant](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [Créer un e-mail pour un programme de messagerie](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)
