---
description: Découvrez comment envoyer une liste statique à LinkedIn, Facebook ou Google. Utilisez les actions Liste et Envoyer à Ad Network pour choisir les options d’audience et de synchronisation.
title: Envoyer une liste à un réseau publicitaire
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 031eb5f3ff8aac185ce496664f984a4c745c6e44
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 7%

---

# Envoyer une liste à un réseau publicitaire {#send-a-list-to-an-ad-network}

Découvrez comment envoyer une liste statique à [!DNL LinkedIn], [!DNL Facebook] ou Google.

## Comment envoyer une liste {#how-to-send-a-list}

1. Dans Marketo, sélectionnez votre liste, cliquez sur le menu déroulant **[!UICONTROL Actions de liste]**, puis sélectionnez **[!UICONTROL Envoyer au réseau publicitaire]**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Choisissez entre [!DNL LinkedIn], [!DNL Facebook] ou Google (les autres options ne sont pas disponibles pour le moment). Dans cet exemple, nous choisissons **[!DNL LinkedIn]**. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Audience]** et sélectionnez l’audience souhaitée.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Si vous devez vérifier, vous pouvez voir l’audience de destination à laquelle une liste est synchronisée via l’onglet Statut .

1. Choisissez le [!UICONTROL type push] souhaité, puis cliquez sur **[!UICONTROL Mettre à jour]**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Si vous sélectionnez « [!UICONTROL Activer la synchronisation continue des audiences] », Marketo met à jour la liste sur le réseau publicitaire choisi au fur et à mesure que la liste change dans votre instance Marketo. Nous ajoutons **et** supprimons des personnes de l’audience si elles sont ajoutées ou supprimées de la liste statique.

1. Et c&#39;est tout ! Cliquez sur **[!UICONTROL OK]** pour quitter.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## Questions fréquentes {#faq}

**Une seule liste statique peut-elle être synchronisée avec plusieurs audiences publicitaires ?**

Non, une liste ne peut être synchronisée qu’avec une seule audience de destination.

**Si j’active la synchronisation continue avec une audience publicitaire existante, l’audience existante sera-t-elle remplacée ?**

Non, l’audience existante sera ajoutée à , et non remplacée.
