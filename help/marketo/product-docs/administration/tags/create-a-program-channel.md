---
unique-page-id: 2950682
description: Création d’un canal de programme - Documents Marketo - Documentation du produit
title: Création d’un canal de programme
exl-id: 7b4e15db-c221-45a9-9588-99eb2510cde7
feature: Tags
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Création d’un canal de programme {#create-a-program-channel}

Un programme est une initiative marketing spécifique. Le canal est conçu pour être le mécanisme de diffusion, comme le webinaire, le parrainage ou la publicité en ligne.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

>[!NOTE]
>
>En savoir plus sur [programmes](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md), l’élément le plus important de Marketo.

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/create-a-program-channel-1.png)

1. Cliquez sur **[!UICONTROL Balises]**.

   ![](assets/create-a-program-channel-2.png)

   >[!NOTE]
   >
   >Pourquoi les balises ? Un canal est une manière de décrire un programme, tout comme les autres balises. Le canal a juste des fonctionnalités supplémentaires spéciales.

1. Cliquez sur le signe **+** en regard de [!UICONTROL Canal] pour développer et afficher les canaux existants.

   ![](assets/create-a-program-channel-3.png)

1. Sous **[!UICONTROL New]**, cliquez sur **[!UICONTROL New Channel]**.

   ![](assets/create-a-program-channel-4.png)

   >[!NOTE]
   >
   >**Exemple**
   >
   >Canal : Billboard
   >
   >* Appliquer à : par défaut
   >* Progression : membre, engagé (en cas de doute, cela fonctionne bien)
   >* Succès : engagé
   >
   >Canal : Party
   >
   >* Appliquer à : Événement
   >* Progression : invité, enregistré, sans affichage et assisté
   >* Succès : Atteinte
   >
   >Consultez la section Progressions des canaux existants pour savoir comment les utiliser.

1. Examinons l’exemple du canal Parti. Nommez votre nouveau **Canal** et sélectionnez le type de programme auquel il s’appliquera.

   ![](assets/create-a-program-channel-5.png)

   >[!NOTE]
   >
   >Appliquer à quoi ? Il existe plusieurs types de programmes. Faites correspondre le canal au type approprié. En cas de doute, choisissez **[!UICONTROL Par défaut]**.

   >[!NOTE]
   >
   >Lors de l’utilisation de &quot;[!UICONTROL Event with Webinar]&quot;, les mappages système sont verrouillés (comme requis par les intégrations de webinaires) et ne peuvent pas être modifiés.

1. Saisissez les deux premiers noms d’état du programme, puis cliquez sur **[!UICONTROL Ajouter l’étape]**.

   ![](assets/create-a-program-channel-6.png)

1. Saisissez un autre numéro de programme **[!UICONTROL Status]** et **[!UICONTROL Step]**, puis cliquez sur **[!UICONTROL Add Step]**.

   ![](assets/create-a-program-channel-7.png)

   >[!TIP]
   >
   >Le numéro **[!UICONTROL Step]** est utilisé pour le tri des états du programme. Gardez à l’esprit que les gens ne peuvent pas revenir en arrière dans ces étapes de progression. Ils peuvent uniquement modifier l’état à un état de valeur supérieur ou égal. Utilisez les valeurs égales lorsque les états sont destinés à basculer d’un état à l’autre plutôt qu’à une progression.

1. Saisissez le dernier numéro de programme **[!UICONTROL Status]** et **[!UICONTROL Step]**.

   ![](assets/create-a-program-channel-8.png)

   >[!NOTE]
   >
   >Lors de l’utilisation du type &quot;[!UICONTROL Event]&quot;, le mappage système pour les états Registered, Waitlisted et Attending est requis. Ces états ne peuvent donc pas être masqués.

1. Sélectionnez l’ **[!UICONTROL état d’archivage mobile]** pour **[!UICONTROL Registered]**.

   ![](assets/create-a-program-channel-9.png)

1. Sélectionnez l’ **[!UICONTROL État d’archivage mobile]** pour **[!UICONTROL Participé]**.

   ![](assets/create-a-program-channel-10.png)

   >[!NOTE]
   >
   >Les options **[!UICONTROL État d’archivage mobile]** ne seront disponibles que si le canal sera destiné aux programmes d’événements.

   >[!NOTE]
   >
   >Seules les personnes avec un **[!UICONTROL état d’archivage mobile]** de **[!UICONTROL Registered]** et **[!UICONTROL Attending]** seront visibles dans les [applications d’archivage mobile](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/event-check-in-overview.md).

   >[!TIP]
   >
   >Si une nouvelle personne est créée dans l’application d’enregistrement mobile, elle est définie sur Inscrits dans le programme d’événement. Si une personne est archivée dans l’événement de l’application, elle est définie sur Participé dans le programme d’événements.

1. Sélectionnez l’état du programme **[!UICONTROL Success]**, puis cliquez sur **[!UICONTROL Create]**.

   ![](assets/create-a-program-channel-11.png)

   C&#39;est joli ! Lorsque vous créez un nouveau programme de ce type, ce nouveau canal sera l’un des choix.
