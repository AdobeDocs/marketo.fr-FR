---
unique-page-id: 557339
description: Rechercher et fusionner des personnes en double - Documents Marketo - Documentation du produit
title: Rechercher et fusionner des personnes en double
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Rechercher et fusionner des personnes en double {#find-and-merge-duplicate-people}

Marketo Engage déduplique automatiquement lorsque de nouvelles personnes entrent dans le système. Cependant, votre CRM a peut-être initialement envoyé sur des doublons. Voici comment les fusionner.

>[!CAUTION]
>
>Fusion de personnes permanente, il n&#39;y a pas d&#39;option &quot;Annuler&quot;.

>[!PREREQUISITES]
>
>La recherche et la fusion de doublons impliquent l&#39;utilisation de [listes dynamiques intégrées/système](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md){target="_blank"}.

>[!NOTE]
>
>Marketo ne procède pas automatiquement à la déduplication par rapport à une synchronisation Salesforce ou Microsoft Dynamics, ni lorsque vous saisissez manuellement des personnes.

## Rechercher les doublons {#find-duplicates}

1. Accédez au **[!UICONTROL Base]** zone.

   ![](assets/find-and-merge-duplicate-people-1.png)

   >[!CAUTION]
   >
   >La fusion de personnes dans Marketo peut ne pas fonctionner si vous utilisez un compte de personne Salesforce. Si possible, fusionnez les enregistrements dans Salesforce.

1. Sélectionnez la variable **[!UICONTROL Doublons possibles]** Liste dynamique du système, puis cliquez sur **[!UICONTROL Personnes]** .

   ![](assets/find-and-merge-duplicate-people-2.png)

   >[!NOTE]
   >
   >Vous pouvez également [Recherche de personnes en double avec une logique personnalisée](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md){target="_blank"}.

## Fusionner les personnes manuellement {#merge-people-manually}

>[!CAUTION]
>
>Lors de la fusion de personnes, si la personne perdante possède un objet personnalisé Marketo, elle _not_ être réassocié à la personne gagnante. Reparent l’objet personnalisé avant d’effectuer la fusion.

1. Sélectionnez les doublons en maintenant la touche Ctrl/Cmd enfoncée, puis cliquez sur **[!UICONTROL Fusionner les personnes]**.

   ![](assets/find-and-merge-duplicate-people-3.png)

   >[!TIP]
   >
   >Vous pouvez avoir deux doublons ou plus pour la même personne, en les sélectionnant tous à la fois.

1. Vous verrez les valeurs entre les enregistrements qui _don&#39;t_ correspond à . Sélectionnez la valeur à conserver pour chaque champ. Cliquez sur **[!UICONTROL Fusion]** une fois terminé. Si vous ne souhaitez aucune des valeurs, vous pouvez vérifier **[!UICONTROL Personnalisé]** et saisissez la valeur de votre choix.

   ![](assets/find-and-merge-duplicate-people-4.png)

   >[!NOTE]
   >
   >Lors de la fusion manuelle de personnes, la première personne sélectionnée sera la &quot;gagnante&quot;. Dans l&#39;onglet Personnes, si vous fusionnez des ID d&#39;enregistrement 198 et 199, et que vous cliquez sur 199 en premier, 199 sera l&#39;ID d&#39;enregistrement des personnes fusionnées. Cela s&#39;applique également si plus de deux enregistrements sont fusionnés.

   >[!TIP]
   >
   >La fusion vaut mieux que la suppression. Vous conserverez tous les historiques (visites de page, clics sur les liens, ouvertures d’email, remplissage de formulaires, etc.).

## Effet dans Salesforce {#effect-in-salesforce}

Si vous avez intégré Salesforce, vous trouverez quelques notes sur l’effet de la fusion de Leads dans Salesforce.

* Lorsque vous fusionnez uniquement les pistes ou uniquement les contacts, ils fusionnent selon les règles Salesforce normales.
* Lorsque vous fusionnez les pistes et les contacts, toutes les pistes sont converties en contacts avant la fusion selon les règles Salesforce normales.

Pour plus d’informations sur le comportement de Salesforce lors de la fusion de Leads ou de Contacts, consultez les documents Salesforce suivants :

* [Fusion de pistes en double](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US){target="_blank"}
* [Fusion de contacts en double](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US){target="_blank"}

## Fusion en bloc {#bulk-merging}

Si vous avez trop de doublons à fusionner manuellement, contactez l’équipe Compte d’Adobe (votre gestionnaire de compte) pour discuter de vos options.
