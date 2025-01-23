---
description: Rendre une campagne marketing visible dans les actions Sales Insight - Documents Marketo - Documentation du produit
title: Rendre une campagne marketing visible dans les actions Sales Insight
exl-id: 223baca3-159e-4f0d-b26f-f4c924a39fc3
feature: Sales Insight Actions
source-git-commit: 696353c74fd14fe72699fb53a87cfed5e9c42d51
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Rendre une campagne marketing visible dans les actions Sales Insight {#make-a-marketing-campaign-visible-in-sales-insight-actions}

Les campagnes ne peuvent être partagées que si elles sont rendues visibles.

Grâce aux actions Sales Insight, les utilisateurs auront accès à une nouvelle application de vente appelée toutapp.com. Cette application leur offre un nouvel ensemble de fonctionnalités d’action, mais hérite également de la fonctionnalité _Ajouter à une campagne marketing_ disponible dans la version principale de Sales Insights. Gardez cela à l’esprit, car selon l’emplacement où vous souhaitez que les utilisateurs accèdent à la fonctionnalité Ajouter à Marketing Campaign (toutapp.com ou l’expérience du package MSI SFDC), vos campagnes Marketo doivent être configurées différemment. Voir la remarque à l’étape 4 pour en savoir plus.

1. Sélectionnez (ou créez) la campagne que vous souhaitez partager.

   ![](assets/make-a-marketing-campaign-visible-sia-1.png)

1. Cliquez sur l’onglet **Liste dynamique**.

   ![](assets/make-a-marketing-campaign-visible-sia-2.png)

1. Ajoutez le déclencheur _La campagne est demandée_.

   ![](assets/make-a-marketing-campaign-visible-sia-3.png)

1. Pour la source, choisissez « is » **API de service web**.

   ![](assets/make-a-marketing-campaign-visible-sia-4.png)

   >[!NOTE]
   >
   >Si vous souhaitez afficher la campagne marketing aux utilisateurs qui utilisent _Ajouter à la campagne marketing_ à partir de l’application web toutapp.com (cela inclut également si l’application web est incorporée dans le CRM via l’objet Boîte d’envoi des ventes Marketo), définissez-la sur « API de service web ». Si vous souhaitez que la campagne marketing s’affiche lorsqu’un utilisateur utilise les actions du panneau MSI dans Salesforce sur le prospect, le contact, la page de compte ou les boutons d’action en bloc dans les vues de liste de prospects et de contacts, mettez-la à jour sur « Informations commerciales »

1. Cliquez sur l’onglet **Flux**.

   ![](assets/make-a-marketing-campaign-visible-sia-5.png)

1. Ajoutez l’action de flux _Moment intéressant_.

   ![](assets/make-a-marketing-campaign-visible-sia-6.png)

1. Pour Type, sélectionnez **Web**.

   ![](assets/make-a-marketing-campaign-visible-sia-7.png)

1. Dans la zone _Description_, écrivez un message à votre équipe commerciale. Dans cet exemple, nous utilisons des jetons pour spécifier le formulaire qui a été rempli.

   ![](assets/make-a-marketing-campaign-visible-sia-8.png)

1. Cliquez sur l’onglet **Planifier** et **Activer** la campagne.

   ![](assets/make-a-marketing-campaign-visible-sia-9.png)
