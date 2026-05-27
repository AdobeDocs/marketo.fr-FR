---
unique-page-id: 2360219
description: Découvrez comment configurer une signature DKIM personnalisée pour votre domaine dans Marketo. Ajoutez un domaine dans Admin et utilisez le service informatique pour publier l’enregistrement DNS.
title: Configurer une signature DKIM personnalisée
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
TQID: https://experienceleague.adobe.com/ln23WoloRVzBoC8CXFsm90LqYV5FDJzbII8UItp3xDc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 434
ht-degree: 4%

---

# Configurer une signature DKIM personnalisée {#set-up-a-custom-dkim-signature}

Pour garantir une délivrabilité optimale, Marketo signe automatiquement tous les e-mails sortants avec une signature DKIM partagée.

>[!NOTE]
>
>Vous aurez peut-être besoin de l’aide de votre équipe informatique pour suivre certaines des étapes décrites dans cet article.

Vous pouvez personnaliser la signature DKIM pour refléter le ou les domaines de votre choix.

1. Accédez à la section **[!UICONTROL Admin]**.

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >Si vous configurez une signature DKIM personnalisée à l’aide de la méthode héritée, elle continuera à fonctionner et devrait s’afficher ici.

1. Cliquez sur **E-mail**.

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. Cliquez sur l’onglet **SPF/DKIM**, puis **Ajouter un domaine**.

   ![](assets/set-up-a-custom-dkim-signature-3.png)

1. Saisissez le domaine que vous utiliserez dans les e-mails Marketo comme adresse d’expédition. Choisissez un sélecteur et une taille de clé. Cliquez sur **Ajouter** lorsque vous avez terminé.

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   <table>
   <tr>
   <td width="20%"><b>Sélecteur</b></td>
   <td>Chaîne/identifiant unique utilisé pour localiser la partie clé publique de l’enregistrement DKIM. Il peut s’agir d’une chaîne arbitraire ou d’un identifiant unique permettant de séparer et d’identifier l’objectif de cette clé/de cet enregistrement DKIM.</td>
   </tr>
   <tr>
   <td width="20%"><b>Longueur de clé</b></td>
   <td>Niveau de sécurité avec lequel vous souhaitez que votre signature DKIM soit chiffrée.</td>
   </tr>
   </tbody>
   </table>

   <p>

   >[!TIP]
   >
   >* Une taille de clé de 2048 est recommandée.
   >* Si vous utilisez un autre domaine dans votre adresse d’expédition, Marketo utilisera la signature DKIM partagée.

   >[!IMPORTANT]
   >
   >Si vous devez mettre à jour le sélecteur DKIM ou la taille de chiffrement DKIM pour votre domaine, vous devez supprimer l’enregistrement existant et republier l’enregistrement nouvellement généré avec les nouvelles valeurs.
   >
   >Dans ce cas, DKIM ne sera pas signé pour votre domaine tant que votre nouvel enregistrement n’aura pas été publié et validé par notre système. Planifiez votre modification en conséquence, car il peut s’écouler entre 24 et 48 heures avant que le nouvel enregistrement DKIM ne soit complètement propagé sur Internet.

1. Envoyez les **[!UICONTROL enregistrement hôte]** et **[!UICONTROL valeur TXT]** à votre service informatique. Demandez-leur de créer l’enregistrement pour vous et assurez-vous qu’il se propage à tous les serveurs de noms associés au domaine de l’expéditeur. La vérification du DKIM Marketo nécessite que la clé DKIM soit propagée à tous les serveurs de noms associés au domaine signé par DKIM.

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. Après avoir confirmé la création de l’enregistrement, revenez à Marketo, sélectionnez votre domaine et cliquez sur **[!UICONTROL Vérifier le DNS]**.

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >Si la confirmation échoue et que votre service informatique a créé l’enregistrement correctement, cela peut être une question de propagation DNS. Veuillez réessayer ultérieurement.

   >[!CAUTION]
   >
   >La modification/suppression de l’enregistrement DNS correspondant aura une incidence négative sur la délivrabilité. Supprimez l’entrée dans Marketo avant d’apporter des modifications DNS.

   Cela améliorera la délivrabilité de vos e-mails. Vous devriez obtenir la validation que l&#39;enregistrement est là et correct.
