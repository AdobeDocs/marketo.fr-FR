---
unique-page-id: 2359418
description: Importation d’une liste de personnes - Documents Marketo - Documentation du produit
title: Importation d’une liste de personnes
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 5%

---

# Importation d’une liste de personnes {#import-a-list-of-people}

## Mission : Importez dans votre base de données une feuille de calcul contenant les participants aux salons professionnels. {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configuration et ajout d’une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

Dans ce tutoriel, vous apprendrez à importer dans Marketo des personnes à partir d’un fichier de feuille de calcul.

## Étape 1 : Téléchargement et modification d’une feuille de calcul {#step-download-and-edit-a-spreadsheet}

1. Pour commencer, téléchargez notre fichier de feuille de calcul pratique ([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}) à votre ordinateur.

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >Lors de l&#39;import d&#39;une date, utilisez le format suivant : **9/21/20** (Mois/Jour/Année).

   >[!NOTE]
   >
   >Les champs Date/Heure importés sont traités comme heure centrale. Si des champs Date/Heure se trouvent dans un fuseau horaire différent, vous pouvez utiliser une formule Excel pour les transformer en heure normale du Centre (Amérique/Chicago).

1. Ajoutez vos propres prénom, nom, véritable adresse email (afin que vous puissiez recevoir les messages de support que vous enverrez lors de la prochaine mission) et le titre de la tâche. Enregistrez le fichier sur votre ordinateur.

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >Marketo **not** prennent en charge les adresses électroniques contenant des emojis.

## Étape 2 : Créer un programme {#step-create-a-program}

1. Accédez au **[!UICONTROL Activités marketing]** zone.

   ![](assets/import-a-list-of-people-3.png)

1. Sélectionnez votre **Formation** , puis sous **[!UICONTROL Nouveau]** click **[!UICONTROL Nouveau programme]**.

   ![](assets/import-a-list-of-people-4.png)

1. **Nom** le programme &quot;Mon programme de commerce&quot; et sélectionnez &quot;Événement&quot; pour le **[!UICONTROL Type de programme]**.

   ![](assets/import-a-list-of-people-5.png)

1. Sélectionner **[!UICONTROL Commerce]** pour le **[!UICONTROL Canal]** et cliquez sur **[!UICONTROL Créer]**.

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>Les programmes d’événement se produisent à des dates spécifiques. En savoir plus sur [**Événements**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}.

## Étape 3 : Importation de votre feuille de calcul dans Marketo {#step-import-your-spreadsheet-into-marketo}

1. Dans **Mon programme de commerce**, cliquez sur **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouvelle ressource locale]**.

   ![](assets/import-a-list-of-people-7.png)

1. Sélectionner **[!UICONTROL Liste]**.

   ![](assets/import-a-list-of-people-8.png)

1. **Nom** Dans la liste &quot;Trafic des participants&quot;, cliquez sur **[!UICONTROL Créer]**.

   ![](assets/import-a-list-of-people-9.png)

1. Dans votre **[!UICONTROL Traiter les participants]** liste, cliquez sur **[!UICONTROL Actions de liste]** et sélectionnez **[!UICONTROL Liste d’importation]**.

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >Si vous utilisez votre propre fichier CSV, assurez-vous qu’il est codé au format UTF-8, UTF-16, Shift-JIS ou EUC-JP.

   >[!NOTE]
   >
   >La taille des fichiers CSV est limitée à 100 Mo.

1. **[!UICONTROL Parcourir]** au **tradeshow-attendees.csv** fichier de feuille de calcul sur votre ordinateur, puis cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >En mode d’importation de liste, en sélectionnant **[!UICONTROL Ignorer les nouvelles personnes et les mises à jour]** signifie que vous n’affecterez pas les enregistrements de personne existants ni n’enregistrez aucune activité. Utilisez ce mode si vous souhaitez obtenir une liste statique rapide et préfiltrée des personnes existantes à utiliser dans vos activités marketing. La sélection de ce mode permet d’effectuer les opérations suivantes :
   >
   > * Ignorer la création d’une nouvelle personne
   > * Ignorer les mises à jour du champ individu
   > * Ignorer la journalisation d&#39;activité

1. Mappez vos [!UICONTROL Colonne de liste] dans le champ Marketo correspondant, puis cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >Les en-têtes de colonne doivent toujours correspondre exactement au champ (sensible à la casse) afin d’obtenir les meilleurs résultats de mappage automatique. Si vous utilisez des champs personnalisés et que vous ne les voyez pas dans la liste déroulante, revenez en arrière et [créer les](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"} ils peuvent devenir des options.

   >[!NOTE]
   >
   >Si vous ne souhaitez pas importer des champs, sélectionnez **Ignorer** dans le menu déroulant Champ Marketo .

1. Sélectionner **Mon programme de commerce** pour le **[!UICONTROL Programme d’acquisition]**, puis cliquez sur **[!UICONTROL Importer]**.

   ![](assets/import-a-list-of-people-13.png)

1. Attendez que vos employés importent, puis fermez la fenêtre contextuelle de progression de l&#39;import.

   ![](assets/import-a-list-of-people-14.png)

1. Retour à **Mon programme de commerce**, cliquez sur le bouton **[!UICONTROL Membres]** . Vous verrez toutes les personnes que vous venez d&#39;importer.

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>Vous pouvez analyser le succès de votre programme en suivant l’adhésion au programme. En savoir plus sur [**Programmes**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}.

## Mission accomplie {#mission-complete}

Les participants au salon sont désormais membres de votre programme Marketo !

<br> 

[◄ Mission 4 : Réponse automatique aux e-mails](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Mission 6 : Marketing goutte à goutte et fidélisation ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
