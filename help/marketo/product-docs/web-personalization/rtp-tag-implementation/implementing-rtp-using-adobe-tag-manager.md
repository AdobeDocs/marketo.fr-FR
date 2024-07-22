---
unique-page-id: 4720218
description: Mise en oeuvre de la procédure RTP à l’aide d’Adobe Tag Manager - Documents Marketo - Documentation du produit
title: Mise en oeuvre de la procédure RTP à l’aide d’Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Mise en oeuvre de la procédure RTP à l’aide d’Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous :

1. Connectez-vous à votre compte RTP.

1. Accédez à **Paramètres du compte**.

   a. Si vous avez déjà reçu votre balise JavaScript de la part de l’assistance, passez à l’étape 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer la balise**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Connectez-vous à votre compte Gestionnaire dynamique de balises ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Accédez à **Tableau de bord.** Cliquez sur la propriété web appropriée.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Accédez à **Rules**, cliquez sur **Create New Rule**.

1. Remplissez les éléments suivants :

   1. Nom : **Marketo RTP**
   1. Conditions (réduction) : règle de déclenchement à - **Haut de la page**
   1. Javascript (réduire) : cliquez sur **Ajouter un nouveau script**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Appelez la nouvelle balise : **Marketo RTP Tag**

1. Supprimer le code suivant de la balise RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Collez la balise JavaScript RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Veillez à supprimer toutes les balises et à ne laisser que le script lui-même (non `<script type='text/javascript'>` , `</script>` ).

1. Cliquez sur **Enregistrer le code** dans l’éditeur de script et **Enregistrer la règle** dans l’éditeur de règles.

1. Dans le panneau Règles, recherchez la règle de chargement de page HTTP Marketo et, dans la liste déroulante **Actions**, sélectionnez **Activer les règles**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Vérifiez qu’il apparaît sur toutes les pages, y compris les landing pages et les sous-domaines.**

   Pour ce faire, cliquez avec le bouton droit de la souris sur les pages de votre site web. Accédez à **Inspect Element**, cliquez sur **Network**, Search: **RTP**.
