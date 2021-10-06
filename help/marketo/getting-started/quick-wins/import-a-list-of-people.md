---
unique-page-id: 2359418
description: Importation d’une liste de personnes - Documents Marketo - Documentation du produit
title: Importation d’une liste de personnes
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: 1b37a750c5e609b9e43e942df752305d85153989
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 5%

---

# Importation d’une liste de personnes {#import-a-list-of-people}

## Mission : Importez dans votre base de données une feuille de calcul contenant les participants aux salons professionnels. {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configuration et ajout d’une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

Dans ce tutoriel, vous apprendrez à importer dans Marketo des personnes à partir d’un fichier de feuille de calcul.

## Étape 1 : Téléchargement et modification d’une feuille de calcul {#step-download-and-edit-a-spreadsheet}

1. Pour commencer, téléchargez notre fichier de feuille de calcul pratique ([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv)) sur votre ordinateur.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Lors de l&#39;import d&#39;une date, utilisez le format suivant : **9/21/20** (Mois/Jour/Année).

   >[!NOTE]
   >
   >Les champs Date/Heure importés sont traités comme heure centrale. Si des champs Date/Heure se trouvent dans un fuseau horaire différent, vous pouvez utiliser une formule Excel pour les transformer en heure normale du Centre (Amérique/Chicago).

1. Ajoutez vos propres prénom, nom, adresse électronique et titre de la tâche, puis enregistrez le fichier sur votre ordinateur.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>Entrez votre véritable adresse électronique dans le fichier CSV afin de recevoir les e-mails de préparation que vous enverrez lors de la prochaine mission.

## Étape 2 : Créer un programme {#step-create-a-program}

1. Accédez à la zone **Activités marketing** .

   ![](assets/ma-2.png)

1. Sélectionnez votre dossier **Apprentissage**, puis sous **Nouveau** cliquez sur **Nouveau programme**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **** Nommez le programme &quot;My Tradeshow Program&quot; et sélectionnez &quot;Event&quot; pour le type de  **programme**.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Sélectionnez **Tradeshow** pour le **canal** et cliquez sur **Créer**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>Les programmes d’événement se produisent à des dates spécifiques. En savoir plus sur [**les événements**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md).

## Étape 3 : Importation de votre feuille de calcul dans Marketo {#step-import-your-spreadsheet-into-marketo}

1. Dans **Mon programme de commerce**, cliquez sur **Nouveau** et sélectionnez **Nouvelle ressource locale**.

   ![](assets/seven-3.png)

1. Cliquez sur **Liste**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **** Nommez la liste &quot;Participant(e) de commerce&quot; et cliquez sur  **Créer**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. Dans votre liste **Participant(s) de commerce**, cliquez sur **Actions de liste** et sélectionnez **Importer la liste**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Si vous utilisez votre propre fichier CSV, assurez-vous qu’il est codé au format UTF-8, UTF-16, Shift-JIS ou EUC-JP.

   >[!NOTE]
   >
   >La taille des fichiers CSV est limitée à 100 Mo.

1. **** Accédez au fichier  **tradeshow-attendees.** csvtabreadsheet sur votre ordinateur et cliquez sur  **Suivant**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >En mode d’importation de liste, le fait de sélectionner **Ignorer les nouvelles personnes et les mises à jour** signifie que vous n’aurez aucune incidence sur les enregistrements de personne existants ni sur les activités enregistrées. Utilisez ce mode si vous souhaitez obtenir une liste statique rapide et préfiltrée des personnes existantes à utiliser dans vos activités marketing. La sélection de ce mode permet d’effectuer les opérations suivantes :
   >
   > * Ignorer la création d’une nouvelle personne
   > * Ignorer les mises à jour du champ individu
   > * Ignorer la journalisation d&#39;activité


1. Faites correspondre vos champs Colonne de liste avec leur champ Marketo respectif et cliquez sur **Suivant**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Les en-têtes de colonne doivent toujours correspondre exactement au champ (sensible à la casse) afin d’obtenir les meilleurs résultats de mappage automatique. Si vous utilisez des champs personnalisés et que vous ne les voyez pas dans la liste déroulante, revenez en arrière et [créez-les](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) afin qu’elles puissent devenir des options.

   >[!NOTE]
   >
   >Si vous ne souhaitez pas importer des champs, sélectionnez **Ignorer** dans le menu déroulant Champ Marketo .

1. Sélectionnez **Mon programme de commerce** pour le **programme d’acquisition**, puis cliquez sur **Importer**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Attendez que vos employés importent, puis fermez la fenêtre contextuelle de progression de l&#39;import.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. De retour dans **Mon programme Tradeshow**, cliquez sur l’onglet **Membres**. Vous verrez toutes les personnes que vous venez d&#39;importer.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>Vous pouvez analyser le succès de votre programme en suivant l’adhésion au programme. En savoir plus sur [**Programmes**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md).

## Mission accomplie {#mission-complete}

Les participants au salon sont désormais membres de votre programme Marketo !

<br> 

[◄ Mission 4 : Réponse automatique aux e-mails](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Mission 6 : Marketing goutte à goutte et fidélisation ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
