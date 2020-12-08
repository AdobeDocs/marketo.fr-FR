---
unique-page-id: 2360219
description: Configurer une signature DKIM personnalisée - Documents marketing - Documentation du produit
title: Configurer une signature DKIM personnalisée
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Configurer une signature DKIM personnalisée {#set-up-a-custom-dkim-signature}

Afin d&#39;assurer une livraison de premier ordre, nous signons automatiquement tous les messages sortants avec une signature partagée de Marketing DKIM.

>[!NOTE]
>
>Vous aurez peut-être besoin de l&#39;aide de votre équipe informatique pour effectuer certaines des étapes de cet article.

Vous pouvez personnaliser la signature DKIM pour refléter le ou les domaines de votre choix. Voici comment.

1. Accédez à la section **Admin** .

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >
   >Si vous configurez une signature DKIM personnalisée à l’ancienne manière, elle continuera à fonctionner et devrait s’afficher ici.

1. Cliquez sur **Courriel**, puis sur l’onglet **DKIM** et enfin sur **Ajouter le domaine**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. Entrez le domaine que vous allez utiliser dans les courriers électroniques de Marketo comme adresse de départ et cliquez sur **Ajouter**.

   >[!TIP]
   >
   >
   >Si vous utilisez un autre domaine dans votre adresse de départ, nous utiliserons la signature DKIM partagée par Marketing Cloud.

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. Envoyez l’enregistrement **** hôte et la valeur **** TXT à votre service informatique. Demandez-leur de créer l’enregistrement pour vous et de s’assurer qu’il se propage à tous les serveurs de noms associés au domaine de départ. La vérification DKIM de Marketo exige que la clé DKIM soit propagée à tous les serveurs de noms associés au domaine signé DKIM.

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. Une fois qu’ils ont confirmé avoir créé l’enregistrement, revenez sur Marketo, sélectionnez votre domaine, puis cliquez sur **Vérifier DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >**Rappel**
   >
   >Si la confirmation échoue et que votre service informatique a créé l&#39;enregistrement correctement, il peut s&#39;agir d&#39;une propagation DNS. Réessayez plus tard.

   >[!CAUTION]
   >
   >
   >La modification/suppression de l&#39;enregistrement DNS correspondant entraînera une délivrabilité endommagée. Veillez à supprimer l’entrée dans Marketo avant d’effectuer des modifications DNS.

   Cela vous aidera à livrer votre courrier électronique. Vous devriez obtenir la validation que l&#39;enregistrement est là et correct.

