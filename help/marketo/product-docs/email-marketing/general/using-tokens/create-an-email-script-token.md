---
unique-page-id: 1900577
description: Création d’un jeton de script de courrier électronique - Documents Marketo - Documentation du produit
title: Création d’un jeton de script de courrier électronique
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Création d’un jeton de script de courrier électronique {#create-an-email-script-token}

Pour les développeurs avancés, vous pouvez utiliser des [scripts Velocity](https://velocity.apache.org/engine/1.7/user-guide.html) dans vos emails. Voici comment le faire.

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Recherchez et sélectionnez un programme (événement, valeur par défaut, engagement, etc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Sous l’onglet **Mes jetons**, faites glisser un jeton **Script de l’email**.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Nommez votre jeton de script de courrier électronique et **cliquez pour modifier** son contenu.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Utilisez l’arborescence à droite pour faire glisser des jetons **Person, Opportunity** ou **Custom Object**.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Lors de l’accès à un tableau (opportunité ou objet personnalisé), vous êtes limité aux 10 éléments les plus récents associés à la personne.

1. Notez que le jeton est coché/actif après l’avoir fait glisser dans l’éditeur de script.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Si vous saisissez des jetons en forme libre, assurez-vous de vérifier/activer tous les jetons correspondants dans l’arborescence ou ils seront traités comme du texte brut et ne fonctionneront pas.

1. Écrivez votre script dans Velocity. Voici quelques ressources utiles :

   * [Documentation sur les scripts de courrier électronique des développeurs Marketo](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)
   * [Guide de l’utilisateur Velocity](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Guide de référence Velocity](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Une fois votre script terminé, cliquez sur **Enregistrer**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Cliquez une fois de plus sur **Enregistrer**.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Vous pouvez maintenant utiliser ce jeton dans vos emails. Il exécute le script chaque fois qu’un email est envoyé.

>[!MORELIKETHIS]
>
>[ Ajout d’un jeton de script de courrier électronique à votre adresse électronique](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
