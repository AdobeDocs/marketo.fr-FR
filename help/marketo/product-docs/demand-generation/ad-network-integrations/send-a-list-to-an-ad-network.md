---
description: Envoyer une liste à un réseau publicitaire - Documents Marketo - Documentation du produit
title: Envoi d’une liste à un réseau publicitaire
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Envoi d’une liste à un réseau publicitaire {#send-a-list-to-an-ad-network}

Découvrez comment envoyer une liste statique à LinkedIn, Facebook ou Google.

## Comment envoyer une liste {#how-to-send-a-list}

1. Dans Marketo Engage, sélectionnez votre liste, puis cliquez sur le bouton **[!UICONTROL Actions de liste]** , puis sélectionnez **[!UICONTROL Envoyer au réseau publicitaire]**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Choisissez entre LinkedIn, Facebook ou Google (les autres options ne sont pas disponibles pour l’instant). Dans cet exemple, nous choisissons **[!UICONTROL LinkedIn]**. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Cliquez sur le bouton **[!UICONTROL Audience]** et sélectionnez l’audience souhaitée.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Si vous avez besoin de vérifier, vous pouvez voir l&#39;audience de destination vers laquelle une liste est synchronisée à partir de l&#39;onglet Statut .

1. Sélectionnez le type push de votre choix, puis cliquez sur **[!UICONTROL Mettre à jour]**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Si vous sélectionnez &quot;Activer la synchronisation continue de l’audience&quot;, Marketo met la liste à jour dans le réseau publicitaire sélectionné au fur et à mesure que la liste change dans votre instance Marketo. Nous ajoutons tous deux _et_ supprimer des personnes de l’audience si elles sont ajoutées/supprimées de la liste statique ;

1. Et c&#39;est tout ! Cliquez sur **[!UICONTROL OK]** pour quitter.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## Questions fréquentes {#faq}

**Une seule liste statique peut-elle être synchronisée avec plusieurs audiences publicitaires ?**

Non, une liste ne peut être synchronisée qu’avec une seule audience de destination.

**Si j’active la synchronisation continue avec une audience de publicité existante, l’audience existante sera-t-elle remplacée ?**

Non, l’audience existante sera ajoutée, et non remplacée.
