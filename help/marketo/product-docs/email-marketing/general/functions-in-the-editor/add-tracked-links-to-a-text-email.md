---
unique-page-id: 1900589
description: Ajout de liens suivis à un e-mail texte - Documents Marketo - Documentation du produit
title: Ajout de liens suivis à un e-mail texte
exl-id: 10b4e029-de23-4054-83f7-b68fea68c838
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Ajout de liens suivis à un e-mail texte {#add-tracked-links-to-a-text-email}

>[!PREREQUISITES]
>
>* [Créer un e-mail texte uniquement](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-a-text-only-email.md)
>* [Modifier des éléments dans un e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/edit-elements-in-an-email.md)

Les liens d’e-mail texte peuvent être suivis dans Marketo. Voyons comment ça fonctionne.

1. Sélectionnez votre e-mail et cliquez sur **Modifier le brouillon**.

1. Sélectionnez votre e-mail et cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/one-9.png)

1. Double-cliquez sur la zone modifiable à laquelle vous souhaitez ajouter le lien.

   ![](assets/two-8.png)

1. Saisissez l’URL entre doubles crochets, comme suit : `[[www.domain.com/path/page.html]]`.

   ![](assets/three-8.png)

   >[!CAUTION]
   >
   >Si un e-mail a été envoyé il y a plus de 365 jours **et que personne n’a cliqué sur l’un de ses liens au cours des 180 derniers jours** Marketo Engage élague l’itinéraire vers l’URL de notre base de données, ce qui entraîne la rupture du lien. Si vous avez besoin que le lien soit permanent, n’utilisez pas le suivi.

1. Fermez l’éditeur et n’oubliez pas d’approuver le brouillon.

   ![](assets/four-6.png)

>[!NOTE]
>
>La fonctionnalité de classe mktNoTok ne fonctionne pas avec les liens trackables dans les emails texte. Uniquement pour les e-mails HTML.
