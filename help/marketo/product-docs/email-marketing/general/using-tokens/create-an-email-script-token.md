---
unique-page-id: 1900577
description: Création d’un jeton de script de courrier électronique - Documents marketing - Documentation du produit
title: Création d’un jeton de script de courrier électronique
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# Créer un jeton de script de courrier électronique {#create-an-email-script-token}

Pour les développeurs avancés, vous pouvez utiliser [des scripts Velocity](https://velocity.apache.org/engine/1.7/user-guide.html) dans vos courriels. Voici comment le faire.

1. Accédez à **Activités marketing**.

   ![](assets/ma.png)

1. Recherchez et sélectionnez n’importe quel programme (Événement, Par défaut ou Engagement, etc.).

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. Sous l&#39;onglet **Mes jetons**, faites glisser un jeton **Script de courriel**.

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. Nommez votre jeton de script de courrier électronique et **cliquez pour modifier** son contenu.

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. Utilisez l&#39;arborescence à droite pour faire glisser les jetons **Personne, Opportunité** ou **Objet personnalisé**.

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >Lors de l&#39;accès à un tableau (opportunité ou objet personnalisé), vous êtes limité aux 10 éléments les plus récents associés à la personne.

1. Notez que le jeton est coché/principal après l’avoir fait glisser dans l’éditeur de script.

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >Si vous tapez des jetons en forme libre, veillez à vérifier/activer tous les jetons correspondants dans l&#39;arborescence ou ils seront traités comme du texte brut et ne fonctionneront pas.

1. Écrivez votre script dans Velocity. Voici quelques ressources utiles :

   * [Documentation sur les scripts de courrier électronique destinée aux développeurs du marketing](https://developers.marketo.com/email-scripting/)
   * [Guide de l&#39;utilisateur Velocity](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Guide de référence Velocity](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Outils Velocity Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. Une fois votre script terminé, cliquez sur **Enregistrer**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. Cliquez à nouveau sur **Enregistrer**.

   ![](assets/image2014-9-17-22-3a23-3a13.png)

Vous pouvez désormais utiliser ce jeton dans vos courriels. Il exécute le script chaque fois qu’un courrier électronique est envoyé.

>[!MORELIKETHIS]
>
>[Ajouter un jeton de script de courrier électronique à votre adresse électronique](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
