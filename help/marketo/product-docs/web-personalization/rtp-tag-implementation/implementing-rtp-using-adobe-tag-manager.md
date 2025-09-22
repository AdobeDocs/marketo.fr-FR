---
unique-page-id: 4720218
description: Mise en œuvre du RTP à l’aide d’Adobe Tag Manager - Documents Marketo - Documentation du produit
title: Mise en œuvre de RTP à l’aide d’Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 5%

---

# Mise en œuvre de RTP à l’aide d’Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Pour implémenter votre balise RTP, suivez les instructions d’installation ci-dessous :

1. Connectez-vous à votre compte RTP.

1. Accédez à **[!UICONTROL Paramètres du compte]**.

   a. Si vous avez déjà reçu votre balise JavaScript de l’assistance - passez à l’étape 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. Sous [!UICONTROL Domaine], recherchez le domaine approprié et cliquez sur **[!UICONTROL Générer la balise]**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Connectez-vous à votre compte [!DNL Dynamic Tag Manager] ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Accédez à **[!UICONTROL Tableau de bord ].** Cliquez sur la propriété web correspondante.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Accédez à **[!UICONTROL Règles]**, puis cliquez sur **[!UICONTROL Créer une règle]**.

1. Remplissez les champs suivants

   1. [!UICONTROL Name] : **RTP Marketo**
   1. [!UICONTROL Conditions] (réduire) : règle de déclenchement sur - **[!UICONTROL Haut de la page]**
   1. [!UICONTROL Javascript] (réduire) : cliquez sur **[!UICONTROL Ajouter un nouveau script]**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Appelez la nouvelle balise : **Marketo RTP Tag**

1. Supprimez le code suivant de la balise [!UICONTROL  RTP ]

   * `<script type='text/javascript'>`
   * `</script>`

1. Collez la balise RTP JavaScript.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Veillez à supprimer toutes les balises et à ne laisser que le script lui-même (pas de `<script type='text/javascript'>` , `</script>` )

1. Cliquez sur **[!UICONTROL Enregistrer le code]** dans l’éditeur de scripts et sur **[!UICONTROL Enregistrer la règle]** dans l’éditeur de règles.

1. Dans le panneau Règles, recherchez la règle de chargement de page RTP Marketo et dans la liste déroulante **[!UICONTROL Actions]** sélectionnez **[!UICONTROL Activer les règles]**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **[!UICONTROL Vérifiez]** qu’il apparaît sur toutes les pages, y compris les pages de destination et les sous-domaines.

   Pour ce faire, cliquez avec le bouton droit de la souris sur les pages de votre site web. Accédez à **[!UICONTROL Inspecter l’élément]**, cliquez sur **[!UICONTROL Réseau]**, recherchez : **RTP**.
