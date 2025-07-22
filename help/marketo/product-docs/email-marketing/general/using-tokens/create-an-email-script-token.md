---
unique-page-id: 1900577
description: Création d’un jeton de script de courrier électronique - Documents Marketo - Documentation du produit
title: Créer un jeton de script d’e-mail
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Créer un jeton de script d’e-mail {#create-an-email-script-token}

Pour les développeurs avancés, vous pouvez utiliser des scripts [Velocity](https://velocity.apache.org/engine/1.7/user-guide.html) dans vos e-mails. Voici comment procéder.

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/ma.png)

1. Recherchez et sélectionnez un programme (Événement, Par défaut ou Engagement, etc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Sous l’onglet **[!UICONTROL Mes jetons]**, faites glisser un jeton **[!UICONTROL Script d’e-mail]**.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Nommez votre jeton de script de messagerie et **[!UICONTROL Cliquez pour modifier]** son contenu.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Utilisez l’arborescence de droite pour faire glisser des jetons **[!UICONTROL Personne]**, **[!UICONTROL Opportunité]** ou **[!UICONTROL Objet personnalisé]**.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Lors de l’accès à un tableau (opportunité ou objet personnalisé), vous êtes limité aux 10 éléments les plus récents associés à la personne.

1. Notez que le jeton devient coché/actif après l’avoir fait glisser dans l’éditeur de script.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Si vous saisissez des jetons à structure libre, veillez à vérifier/activer tous les jetons correspondants dans l’arborescence ou ils seront traités comme du texte brut et ne fonctionneront pas.

1. Écrivez votre script dans Velocity. Voici quelques ressources utiles :

   * [Documentation Sur Les Scripts De Messagerie Pour Les Développeurs Marketo](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)
   * [Guide de l’utilisateur Velocity](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Guide de référence Velocity](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Outils Velocity Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Une fois votre script terminé, cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Cliquez encore une fois sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Vous pouvez maintenant utiliser ce jeton dans vos e-mails. Il exécute le script chaque fois qu’un e-mail est envoyé.

>[!MORELIKETHIS]
>
>[Ajouter un jeton de script d’e-mail à votre e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
