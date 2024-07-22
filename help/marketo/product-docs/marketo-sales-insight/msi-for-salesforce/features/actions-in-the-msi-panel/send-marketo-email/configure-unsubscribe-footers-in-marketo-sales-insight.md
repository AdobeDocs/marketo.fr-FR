---
unique-page-id: 2953373
description: Configuration des pieds de page de désabonnement dans Marketo Sales Insight - Marketo Docs - Documentation du produit
title: Configuration du désabonnement des pieds de page dans Marketo Sales Insight
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Configuration du désabonnement des pieds de page dans Marketo Sales Insight {#configure-unsubscribe-footers-in-marketo-sales-insight}

Les courriers électroniques de vente placent automatiquement le pied de page de désabonnement en bas de la page. Vous pouvez toutefois ajuster les paramètres en fonction de vos besoins.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>**Définition**
>
>**Les e-mails de vente** sont ceux envoyés par Sales Insight (ils n’incluent pas ceux envoyés par le module externe Marketo Outlook).

1. Accédez à la zone **Admin**.

   ![](assets/one-1.png)

1. Cliquez sur **Sales Insight**, puis **Modifier les paramètres**.

   ![](assets/two-1.png)

   Il existe plusieurs options. Commençons par examiner les types d’emails pour lesquels vous pouvez modifier les paramètres.

   ![](assets/three-1.png)

   * **Aucun modèle** - Composé manuellement par un utilisateur commercial.
   * **Courrier électronique standard** - Courriers électroniques basés sur un modèle.
   * **E-mail opérationnel** : e-mails ignorant les limites de désabonnement, de marketing suspendu et de communication (qu’ils envoient quoi qu’il arrive).

   Vous avez la possibilité de définir un comportement différent pour chaque type.

   >[!CAUTION]
   >
   >**Respecter les paramètres de désabonnement** : les pistes désabonnées ne recevront PAS l’email même si l’email publié est &quot;opérationnel&quot;.
   >
   >**Ignorer les paramètres de désabonnement** : les pistes désabonnées recevront le courrier électronique.

1. Effectuez les modifications de votre choix, puis cliquez sur **Enregistrer**.

   >[!TIP]
   >
   >Les deux derniers choix permettent d&#39;inclure/exclure dynamiquement le pied de page de désabonnement en fonction du nombre de destinataires (supérieur à 1 ou supérieur à 5).

   ![](assets/four-1.png)

Ouf ! Un peu compliqué, mais assez flexible, n&#39;est-ce pas ?
