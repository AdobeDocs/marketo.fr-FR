---
unique-page-id: 2360219
description: Configuration d’une signature DKIM personnalisée - Documents Marketo - Documentation du produit
title: Configuration d’une signature DKIM personnalisée
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: aed161086948aa2cec0199771ba5b3b1491600f9
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Configuration d’une signature DKIM personnalisée {#set-up-a-custom-dkim-signature}

Afin d’assurer une délivrabilité optimale, nous signons automatiquement tout courrier sortant avec une signature DKIM Marketo partagée.

>[!NOTE]
>
>Vous aurez peut-être besoin de l’aide de votre équipe informatique pour accomplir certaines étapes de cet article.

Vous pouvez personnaliser la signature DKIM pour refléter le ou les domaines de votre choix. Voici comment.

1. Accédez au **Administration** .

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >Si vous configurez une signature DKIM personnalisée à l’ancienne, elle continuera à fonctionner et devrait s’afficher ici.

1. Cliquez sur **Email**.

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. Cliquez sur le bouton **SPF/DKIM** , puis **Ajouter un domaine**.

   ![](assets/set-up-a-custom-dkim-signature-3.png)

1. Saisissez le domaine que vous utiliserez dans les emails Marketo comme Adresse de l’expéditeur. Choisissez un sélecteur et une taille de clé. Cliquez sur **Ajouter** une fois terminé.

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   >[!TIP]
   >
   >* Nous vous recommandons une taille de clé de 2048.
   >* Si vous utilisez un autre domaine dans votre adresse de l’expéditeur, nous utiliserons la signature DKIM partagée par Marketo.

   <table> 
   <tr>
   <td width="20%"><b>Sélecteur</b></td>
   <td>Chaîne/identifiant unique utilisé pour localiser la partie clé publique de l’enregistrement DKIM. Il peut s’agir d’une chaîne arbitraire ou d’un identifiant unique pour séparer et identifier l’objectif de cette clé/enregistrement DKIM.</td>
   </tr>
   <tr> 
   <td width="20%"><b>Taille de clé</b></td>
   <td>Le niveau de sécurité avec lequel vous souhaitez que votre signature DKIM soit cryptée.</td>
   </tr>
   </tbody>
   </table>

1. Envoyez la variable **Enregistrement d’hôte** et **Valeur TXT** à votre service informatique. Demandez-leur de créer l’enregistrement à votre place et de s’assurer qu’il se propage à tous les serveurs de noms associés au domaine d’ . La vérification DKIM Marketo requiert que la clé DKIM soit propagée à tous les serveurs de noms associés au domaine signé DKIM.

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. Une fois qu’ils ont confirmé avoir créé l’enregistrement, revenez à Marketo, sélectionnez votre domaine, puis cliquez sur **Vérifier le DNS**.

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >Si la confirmation échoue et que votre service informatique a correctement créé l’enregistrement, il peut s’agir d’une propagation DNS. Veuillez réessayer ultérieurement.

   >[!CAUTION]
   >
   >La modification/suppression de l’enregistrement DNS correspondant entraîne une délivrabilité endommagée. Veillez à supprimer l’entrée dans Marketo avant d’effectuer des modifications DNS.

   Cela vous aidera tout à fait dans la délivrabilité de vos emails. Vous devriez obtenir la validation que l’enregistrement est présent et correct.
