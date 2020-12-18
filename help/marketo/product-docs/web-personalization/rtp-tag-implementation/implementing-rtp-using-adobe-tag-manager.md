---
unique-page-id: 4720218
description: Implémentation de RTP à l’aide d’Adobe Tag Manager - Docs marketing - Documentation du produit
title: Implémentation de RTP à l’aide d’Adobe Tag Manager
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Implémentation de RTP à l&#39;aide de Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Pour mettre en oeuvre votre balise RTP, suivez les instructions d’installation ci-dessous :

1. Connectez-vous à votre compte RTP.
1. Accédez à **Paramètres du compte.**

   Si vous avez déjà reçu votre balise JavaScript de l’assistance - passez à l’étape 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Sous Domaine, recherchez le domaine approprié et cliquez sur **Générer la balise**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Connectez-vous à votre compte Gestionnaire dynamique de balises ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).
1. Accédez au **Tableau de bord.** Cliquez sur la propriété web appropriée.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Accédez à **Règles,** cliquez sur **Créer une règle.**

1. Renseignez les champs suivants

   1. Nom : **Marketo RTP**
   1. Conditions (effondrement) : Déclencher la règle à - **Haut de la page**
   1. Javascript (effondrement) : cliquez sur **Ajouter un nouveau script**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Appelez la nouvelle balise : **Balise Marketo RTP**
1. Supprimez le code suivant de la balise RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Collez la balise JavaScript RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Veillez à supprimer toutes les balises et à ne laisser que le script lui-même (no `<script type='text/javascript'>` , `</script>` ).

1. Cliquez sur **Enregistrer le code** dans l’éditeur de script et **Enregistrer la règle** dans l’éditeur de règles.

1. Dans le panneau Règles, recherchez la règle de chargement de page RTP de Marketo et dans la liste déroulante **Actions** sélectionnez **Activer les règles**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **** Vérifiez qu’il s’affiche sur toutes les pages, y compris les landings page et sous-domaines.

   Vous pouvez le faire en cliquant avec le bouton droit sur les pages de votre site Web. Accédez à **Inspect Element**, cliquez sur **Network, **Search : **RTP**.
