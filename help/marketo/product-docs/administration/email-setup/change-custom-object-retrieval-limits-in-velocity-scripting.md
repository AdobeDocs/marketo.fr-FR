---
description: "Modification des limites de récupération d’objets personnalisés dans [!DNL Velocity Scripting] - Documents Marketo - Documentation du produit"
title: "Modification des limites de récupération d’objets personnalisés dans [!DNL Velocity Scripting]"
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Modifier les limites de récupération d’objets personnalisés dans [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Si vous utilisez [!DNL Velocity Script] pour afficher les données d’objet personnalisé dans les emails, cette fonctionnalité peut être utile. Par défaut, vous êtes autorisé à accéder à 10 objets personnalisés parents à partir du script Velocity. Si vous avez besoin d’accéder à plus d’informations, lisez la suite.

## Présentation [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) est une langue construite sur [!DNL Java] conçu pour modéliser et scripter le contenu des HTMLS. Marketo permet de l’utiliser dans le contexte des emails via l’utilisation de la fonction [jetons de script](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Cela permet notamment d’accéder aux données stockées dans des objets personnalisés.

Vous pouvez référencer des objets personnalisés parents et enfants directement connectés au prospect ou au contact, mais pas des objets personnalisés de troisième niveau. Pour chaque objet personnalisé, les 10 enregistrements les plus récemment mis à jour par personne/contact sont disponibles au moment de l’exécution et sont classés de la mise à jour la plus récente (à 0) à la mise à jour la plus ancienne (à 9).

## Comment modifier la limite {#how-to-change-the-limit}

1. Accédez au **[!UICONTROL Administration]** .

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Dans le [!UICONTROL Limites de récupération d’objets personnalisés] , saisissez une nouvelle [!UICONTROL Limite de récupération parente] et cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>Le [!UICONTROL Limite de récupération parente] doit être comprise entre 10 et 100. Le [!UICONTROL Limite de récupération des enfants] est définie automatiquement. Pour ce faire, divisez 1 000 par la valeur [!UICONTROL Limite de récupération parente]. Par exemple, si vous définissez la limite Parent sur 50, la limite Enfant devient 20 (1 000 ÷ 50 = 20).

Beau ! Vous pouvez désormais accéder à d’autres objets personnalisés à partir de [!DNL Velocity script].
