---
unique-page-id: 1900597
description: Définissez une Audience en important une Liste - Documents marketing - Documentation du produit
title: Définition d’une Audience en important une Liste
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Définissez une Audience en important une Liste {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[Créer un courriel pour un Programme de courriel](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Une fois que vous avez créé un programme de messagerie, vous voudrez lui indiquer à qui envoyer le message. Pour ce faire, [créez une liste intelligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) ou importez une liste. Voici comment y parvenir en important une liste.

>[!NOTE]
>
>La définition de votre audience ne fonctionnera que si le programme de messagerie n&#39;est pas approuvé.
>
>Tous les champs Date/Heure importés sont traités comme Heure centrale. Si vous avez des champs Date/Heure dans un fuseau horaire différent, vous pouvez utiliser une formule Excel pour le transformer en Heure centrale (Amérique/Chicago).

1. Accédez à **Activités marketing**.

   ![](assets/login-marketing-activities-1.png)

   Sélectionnez votre programme de messagerie, puis cliquez sur Importer la Liste sous le volet Audience.
   ![](assets/importlist.png)

1. La fenêtre d&#39;importation de liste s&#39;ouvre, cliquez sur **Parcourir** et sélectionnez le fichier à importer. Une fois que vous avez sélectionné votre liste de personnes, cliquez sur Suivant.
1. ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Assurez-vous que la liste est codée en UTF-8, UTF-16, Shift-JIS ou EUC-JP et qu’elle ne dépasse pas 50 Mo de taille de fichier.

   Vérifiez que les champs de votre fichier sont correctement mappés et cliquez sur Suivant.
   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo se souviendra des mappages pour les prochaines importations !

1. Saisissez un **nom** pour votre liste et cliquez sur **Importer**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Une fois l’importation terminée, revenez à l’onglet programme principal. Vous verrez combien de personnes seront admissibles.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Définition**
>
>Avez-vous remarqué le numéro bloqué ? Ce numéro est un sous-ensemble des personnes qualifiées et représente les personnes qui ne peuvent pas être envoyées par courriel car elles sont :
>
>* Non abonné
>* Marketing suspendu
>* Placé sur la liste bloquée
>* Adresse électronique non valide
>* Courrier électronique vide

>
>
Cliquez sur le numéro pour obtenir une liste détaillée des personnes bloquées dans les envois.
>
>Utilisez le bouton ![—](assets/image2014-10-23-16-3a32-3a36-1.png) de la mosaïque **Audience** pour déterminer le nombre de personnes qualifiées pour recevoir le courriel en fonction de critères de liste intelligente. Soustrayez le nombre bloqué du nombre de personnes pour obtenir le nombre total de personnes qui recevront le courriel.

>[!TIP]
>
>Vous n&#39;avez pas à attendre la fin de l&#39;importation de liste. Tu peux continuer à travailler si tu veux.

Fantastique ! Il est maintenant temps de choisir un courriel existant ou de créer un nouveau courriel à envoyer à ces personnes.

>[!NOTE]
>
>**Articles connexes**
>
>* [Choisir un courriel existant](../../../../product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [Créer un courriel pour un Programme de courriel](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

>



