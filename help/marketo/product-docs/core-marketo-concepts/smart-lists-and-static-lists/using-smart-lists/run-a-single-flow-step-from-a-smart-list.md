---
unique-page-id: 557322
description: Exécution d’une étape de flux unique à partir d’une liste dynamique - Documents Marketo - Documentation du produit
title: Exécution d’une seule étape de flux à partir d’une liste dynamique
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
source-git-commit: e0106eddf3ed6ecd2d9d90147a56258f61958665
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Exécution d’une seule étape de flux à partir d’une liste dynamique {#run-a-single-flow-step-from-a-smart-list}

Si vous souhaitez exécuter une étape de flux unique, vous pouvez utiliser une seule étape de flux dans une liste dynamique au lieu de créer une campagne dynamique complète.

>[!PREREQUISITES]
>
>[Créer une liste dynamique](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Accédez à **[!UICONTROL Activités marketing]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-1.png)

1. Sélectionnez une liste ou une liste dynamique contenant des personnes, puis accédez à l’onglet **[!UICONTROL Personnes]** .

   ![](assets/run-a-single-flow-step-from-a-smart-list-2.png)

   >[!TIP]
   >
   >Les listes statiques et les listes dynamiques disposent de cette fonctionnalité.

1. Cliquez sur **[!UICONTROL Sélectionner tout]**. Vous pouvez également utiliser **Ctrl/Cmd** et cliquer pour sélectionner quelques enregistrements manuellement.

   ![](assets/run-a-single-flow-step-from-a-smart-list-3.png)

   >[!NOTE]
   >
   >Si les résultats s’étendent sur plusieurs pages, cliquez sur **[!UICONTROL Sélectionner tout]** pour sélectionner toutes les personnes sur toutes les pages.

1. Sous **[!UICONTROL Actions de personne]**, sélectionnez l’étape de flux de votre choix. Dans cet exemple, nous utiliserons [Modifier la valeur des données](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}.

   ![](assets/run-a-single-flow-step-from-a-smart-list-4.png)

1. Recherchez et sélectionnez un **[!UICONTROL attribut]**. Dans cet exemple, nous prendrons toutes les personnes qui ont un état &quot;Californie&quot; et le remplacerons par &quot;CA&quot;.

   ![](assets/run-a-single-flow-step-from-a-smart-list-5.png)

1. Saisissez une nouvelle valeur. Cliquez sur **[!UICONTROL Exécuter maintenant]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-6.png)

1. Si vous modifiez les valeurs des données d’un grand nombre de personnes, vous devrez peut-être confirmer la modification en saisissant le nombre. Cliquez Sur **[!UICONTROL Aller Pour Ça]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-7.png)

Super travail ! L’état de l’étape de flux unique s’affiche dans le coin supérieur droit.

![](assets/run-a-single-flow-step-from-a-smart-list-8.png)

Lorsque la liste est terminée, actualisez-la pour afficher les informations mises à jour.
