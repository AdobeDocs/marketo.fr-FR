---
unique-page-id: 2953384
description: Activer la synchronisation pour une entité personnalisée - Documents Marketo - Documentation du produit
title: Activation de la synchronisation pour une entité personnalisée
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 79ae0d56dd4bb8bf563c6546cba54b89b5841425
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Activation de la synchronisation pour une entité personnalisée {#enable-sync-for-a-custom-entity}

Si vous avez besoin que les données d’entité personnalisées de Dynamics soient disponibles dans Marketo Engage, voici comment activer la synchronisation pour celle-ci.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>* Lorsque vous activez la synchronisation pour une entité personnalisée, Marketo effectue une synchronisation initiale afin d’importer toutes les données de l’objet personnalisé.
>* La liste marketing et les membres de la liste marketing ne sont _pas pris en charge_ pour le moment.

>[!IMPORTANT]
>
>L’utilisateur de synchronisation Marketo doit disposer d’un accès en lecture à l’objet personnalisé pour le répertorier et y effectuer une synchronisation.

1. Accédez à la section **[!UICONTROL Admin]** .

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Sélectionnez **[!UICONTROL Microsoft Dynamics]** et cliquez sur **[!UICONTROL Désactiver la synchronisation]**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Vous devez désactiver temporairement la synchronisation globale pour activer ou désactiver une entité personnalisée.

1. Sous Gestion de la base de données, cliquez sur **[!UICONTROL Synchronisation des entités Dynamics]**.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Cliquez sur **[!UICONTROL Schéma de synchronisation]**.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Sélectionnez l’entité que vous souhaitez synchroniser et cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Sélectionnez les champs que vous souhaitez synchroniser ou utiliser comme [contraintes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) et/ou déclencheurs (pour les enregistrements ajoutés, _non_ mis à jour) dans les listes dynamiques. Une fois que vous avez terminé, cliquez sur **[!UICONTROL Activer la synchronisation]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Pendant le processus de synchronisation, vous pouvez constater que l’élément &quot;[!UICONTROL Synchronisation des entités dynamiques]&quot; disparaît de l’arborescence de navigation. Ce comportement est attendu et réapparaîtra une fois la synchronisation terminée.

1. L’entité dispose désormais d’une coche verte.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. N’oubliez pas de réactiver la synchronisation globale !

   ![](assets/enable-sync-for-a-custom-entity-8.png)

   >[!NOTE]
   >
   >* Marketo ne prend en charge que les entités personnalisées liées à des entités standard profondes d’un ou deux niveaux.
   >
   >* L’arborescence des objets personnalisés peut afficher plusieurs fois le même objet, en raison de ses connexions directes avec l’un des objets principaux (par exemple, les prospects, les contacts, les comptes ou les connexions indirectes via un objet intermédiaire). Dans ce cas, choisissez l’objet le plus proche de l’objet principal et choisissez un seul. Le choix de plusieurs fois d’un même objet peut entraver la synchronisation de cet objet personnalisé.
