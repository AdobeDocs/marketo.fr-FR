---
unique-page-id: 1147352
description: Envoyer un exemple de courrier électronique - Documents Marketo - Documentation du produit
title: Envoyer un exemple de courrier électronique
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Envoyer un exemple de courrier électronique {#send-a-sample-email}

Il est rapide et facile d&#39;envoyer des exemples d&#39;un email. Pour envoyer un email de contenu dynamique, voir [Prévisualisation d’un email avec du contenu dynamique](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>Vous devez avoir la variable **Accès à la base de données - Exécuter des actions de flux unique** autorisation d’envoyer des exemples d’emails.

## Envoyer un exemple de courrier électronique {#send-a-sample-email-1}

1. Recherchez et sélectionnez votre email. Cliquez sur le bouton **Actions de courrier électronique** et sélectionnez **Envoyer un exemple**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >My Tokens correspond à la valeur appropriée au programme de l’email.

1. Saisissez une ou plusieurs adresses email pour la diffusion. Pour plusieurs adresses électroniques, séparez-les par des virgules. Cliquez sur **Envoyer** une fois terminé.

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >Si vous saisissez plusieurs adresses email, elles seront toutes visibles par chaque destinataire. Le premier renseigné sera le destinataire principal et chaque adresse email suivante sera un destinataire CC.

   >[!TIP]
   >
   >Si vous souhaitez résoudre les jetons en tant que personne spécifique, sélectionnez cette personne dans la variable **menu déroulant personne** à l’étape 2.

## Envoyer un exemple de courrier électronique lors de la modification {#send-a-sample-email-while-editing}

1. Recherchez votre email, sélectionnez-le et cliquez sur le bouton **Modifier le brouillon** .

   ![](assets/three-281-29.jpg)

1. Cliquez sur **Actions de courrier électronique**, sélectionnez **Envoyer un exemple**.

   ![](assets/four.png)

1. Saisissez l&#39;adresse email à diffuser et cliquez sur **Envoyer**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Le champ déclencheur ne s&#39;applique qu&#39;aux utilisateurs [script de courrier électronique](https://developers.marketo.com/documentation/velocity-script/).

## Envoi d’un exemple de courrier électronique basé sur un segment {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[Appliquer la segmentation à votre email](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. Recherchez votre email, sélectionnez-le et cliquez sur le bouton **Modifier le brouillon** .

   ![](assets/three-281-29.jpg)

1. Cliquez sur **Aperçu**.

   ![](assets/1.png)

1. Cliquez sur le bouton **Afficher par** et sélectionnez **Segmentation**.

   ![](assets/2.png)

1. Une liste déroulante s’affiche avec les segments disponibles. Cliquez dessus et sélectionnez celui qui vous intéresse.

   ![](assets/3.png)

1. Utilisez les flèches pour faire défiler vos options (dans ce cas, nous avons modifié dynamiquement l’objet).

   ![](assets/4.png)

1. Cliquez sur **Envoyer un exemple** pour recevoir un email de test de votre segment en action.

   ![](assets/5.png)

   >[!TIP]
   >
   >Vous pouvez également envoyer un exemple d’email basé sur un segment en mode d’édition de votre email. Cliquez sur le bouton **Actions de courrier électronique** menu déroulant, sélectionnez **Envoyer un exemple**, puis sélectionnez votre segment.

L’échantillonnage de votre contenu avant le lancement d’une campagne est très important. Mesurez deux fois, coupez une fois !
