---
unique-page-id: 2953373
description: Configuration de la désinscription des pieds de page dans Marketo Sales Insight - Marketo Docs - Documentation sur les produits
title: Configuration de la désinscription des pieds de page dans Marketing Cloud Sales Insight
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Configuration de la désinscription des pieds de page dans Marketing Cloud Sales Insight {#configure-unsubscribe-footers-in-marketo-sales-insight}

Les courriels de vente placent automatiquement le pied de page de désabonnement en bas. Cependant, vous pouvez ajuster les paramètres en fonction de vos besoins.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>**Définition**
>
>**Les** courriels de vente sont ceux envoyés par Sales Insight (ils ne comprennent pas ceux envoyés par le module externe Marketo Outlook).

1. Accédez à la zone **Admin**.

   ![](assets/one-1.png)

1. Cliquez sur **Sales Insight**, puis **Modifier les paramètres**.

   ![](assets/two-1.png)

   Il existe plusieurs options. Commençons par examiner les types de courriels pour lesquels vous pouvez modifier les paramètres.

   ![](assets/three-1.png)

   * **Aucun modèle**  - Composé manuellement par l&#39;utilisateur commercial.
   * **Courrier électronique**  standard - Courriers électroniques basés sur un modèle.
   * **Courrier électronique**  opérationnel - Courriels qui ignorent les limites de désabonnement, de suspension de marketing et de communication (ils envoient quoi que ce soit).

   Vous avez la possibilité de définir un comportement différent pour chaque type.

   >[!CAUTION]
   >
   >**Respecter les paramètres** de désabonnement : les prospects désabonnés ne recevront PAS de courrier électronique même si le courrier publié est &quot;opérationnel&quot;
   >
   >**Ignorer les paramètres** de désabonnement : les pistes désabonnées recevront le courriel

1. Effectuez les modifications souhaitées, puis cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Les deux dernières options vous permettent d’inclure ou d’exclure de manière dynamique le pied de page de désabonnement en fonction du nombre de destinataires (supérieur à 1 ou supérieur à 5).

   ![](assets/four-1.png)

Oh ! Un peu compliqué, mais assez flexible, non ?
