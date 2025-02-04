---
unique-page-id: 2359418
description: Importer une liste de personnes - Documents Marketo - Documentation du produit
title: Importer une liste de personnes
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 1676c9049c61a637faede4751ea49bbcfa018be5
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 4%

---

# Importer une liste de personnes {#import-a-list-of-people}

## Mission : Importer dans votre base de données une liste de tableurs des participants à des salons professionnels {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configuration et ajout d’une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

Dans ce tutoriel, vous apprendrez à importer dans Marketo des personnes à partir d&#39;un fichier de feuille de calcul.

## Étape 1 : Télécharger et modifier une feuille de calcul {#step-download-and-edit-a-spreadsheet}

1. Pour commencer, téléchargez notre fichier de feuille de calcul d&#39;exercices pratiques ([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}) sur votre ordinateur.

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >Lors de l&#39;importation d&#39;une date, utilisez le format suivant : **9/21/20** (Mois/Jour/Année).

   >[!NOTE]
   >
   >Tous les champs de date et d’heure importés sont traités comme des champs d’heure centrale. Si vous avez des champs date/heure dans un fuseau horaire différent, vous pouvez utiliser une formule Excel pour les transformer en Heure du Centre (Amérique/Chicago).

1. Ajoutez votre prénom, votre nom, votre adresse e-mail actuelle (afin de recevoir les e-mails de soutien que vous enverrez lors de la prochaine mission) et votre intitulé de poste. Enregistrez le fichier sur votre ordinateur.

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >* Assurez-vous que les adresses e-mail contiennent uniquement des caractères ASCII.
   >
   >* Marketo ne prend **pas** en charge les adresses e-mail contenant des émoticônes.
   >
   >* L’importation de valeurs `NULL` au moyen d’un fichier CSV peut générer une « valeur Modifier les données » pour les champs numériques du [journal d’activité](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"} d’une personne, _même si les champs sont déjà vides_. Si vous disposez de [Campagnes intelligentes](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"} utilisant le filtre « Valeur des données modifiée » ou le déclencheur « Modifications de la valeur des données », veillez à utiliser [contraintes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"} pour vous assurer qu’elles ne sont pas déclenchées inutilement lors des importations.

## Étape 2 : Créer un programme {#step-create-a-program}

1. Accédez à la zone **[!UICONTROL Activités marketing]**.

   ![](assets/import-a-list-of-people-3.png)

1. Sélectionnez votre dossier **Apprentissage**, puis sous **[!UICONTROL Nouveau]** cliquez sur **[!UICONTROL Nouveau programme]**.

   ![](assets/import-a-list-of-people-4.png)

1. **Nom** sélectionnez le programme « Mon programme de salon professionnel », puis sélectionnez « Événement » pour le **[!UICONTROL Type de programme]**.

   ![](assets/import-a-list-of-people-5.png)

1. Sélectionnez **[!UICONTROL Salon professionnel]** pour le **[!UICONTROL Canal]** et cliquez sur **[!UICONTROL Créer]**.

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>Les programmes d’événement se produisent à des dates spécifiques. En savoir plus sur les [**événements**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}.

## Étape 3 : Importer votre feuille de calcul dans Marketo {#step-import-your-spreadsheet-into-marketo}

1. Dans **Mon programme de salon professionnel**, cliquez sur **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Nouvel actif local]**.

   ![](assets/import-a-list-of-people-7.png)

1. Sélectionnez **[!UICONTROL Liste]**.

   ![](assets/import-a-list-of-people-8.png)

1. **Nommez** répertoriez les participants au salon et cliquez sur **[!UICONTROL Créer]**.

   ![](assets/import-a-list-of-people-9.png)

1. Dans la liste **[!UICONTROL Participants au salon professionnel]**, cliquez sur **[!UICONTROL Liste des actions]** et sélectionnez **[!UICONTROL Importer la liste]**.

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >Si vous utilisez votre propre fichier CSV, assurez-vous qu’il est codé au format UTF-8, UTF-16, Shift-JIS ou EUC-JP.

   >[!NOTE]
   >
   >La limite de taille des fichiers CSV est 100MB.

1. **[!UICONTROL Parcourez]** accédez au fichier de feuille de calcul **tradeshow-attendees.csv** sur votre ordinateur et cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >En mode d&#39;importation de liste, choisir **[!UICONTROL Ignorer les nouvelles personnes et les mises à jour]** signifie que vous n&#39;affecterez pas les enregistrements de personne existants et que vous ne consignerez aucune activité. Utilisez ce mode si vous souhaitez obtenir une liste statique rapide et préfiltrée des personnes existantes à utiliser dans vos activités marketing. La sélection de ce mode va :
   >
   > * Ignorer la création de nouvelles personnes
   > * Ignorer les mises à jour du champ individu
   > * Ignorer la journalisation d&#39;activité

1. Mappez vos champs [!UICONTROL Colonne de liste] à leur champ Marketo respectif et cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >Les en-têtes de colonne doivent toujours correspondre exactement au champ (sensibilité à la casse) afin d’obtenir les meilleurs résultats de mappage automatique. Si vous utilisez des champs personnalisés et que vous ne les voyez pas dans la liste déroulante, revenez en arrière et [créez-les](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"} afin qu’ils puissent devenir des options.

   >[!NOTE]
   >
   >Si vous ne souhaitez pas importer certains champs, sélectionnez **Ignorer** dans le menu déroulant Champ Marketo .

1. Sélectionnez **Mon programme de salon professionnel** pour le **[!UICONTROL Programme d&#39;acquisition]**, puis cliquez sur **[!UICONTROL Importer]**.

   ![](assets/import-a-list-of-people-13.png)

1. Attendez que votre équipe effectue l’importation, puis fermez le pop-up de progression de l’importation.

   ![](assets/import-a-list-of-people-14.png)

1. De retour dans **Mon programme de salon professionnel**, cliquez sur l&#39;onglet **[!UICONTROL Membres]**. Vous verrez toutes les personnes que vous venez d&#39;importer.

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>Vous pouvez analyser le succès de votre programme en effectuant le suivi de l’adhésion au programme. En savoir plus sur les [**programmes**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}.

## Mission accomplie {#mission-complete}

Les participants au salon sont désormais membres de votre programme Marketo !

<br> 

[◄ Mission 4 : Réponse automatique aux courriers électroniques](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Mission 6 : Drip, Drip, Nurture ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
