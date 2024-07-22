---
unique-page-id: 2359422
description: Personnalisation d’un courrier électronique - Documents Marketo - Documentation du produit
title: Personnaliser un e-mail
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 3%

---

# Personnaliser un e-mail {#personalize-an-email}

## Mission : rendez vos emails personnels en ajoutant des jetons de données {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurer et ajouter une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Envoyer un courrier électronique en masse](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [Déroulement, goutte, formation](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## Étape 1 : Sélection d’un email à personnaliser {#step-select-an-email-to-personalize}

1. Sélectionnez l’un des messages électroniques de confiance créés dans la [précédente version rapide](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} et cliquez sur **[!UICONTROL Créer un brouillon]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Cette opération crée une copie de l’email en tant que brouillon. N’oubliez pas d’approuver le brouillon pour que les modifications soient mises en ligne.

Si vous n’avez pas activé de bloqueur de fenêtres contextuelles, l’éditeur de courrier électronique s’ouvre dans un nouvel onglet/nouvelle fenêtre. Sinon, cliquez deux fois sur **[!UICONTROL Créer un brouillon]** .

## Etape 2 : Faire du vendeur l&#39;expéditeur {#step-make-the-salesperson-the-sender}

1. Sélectionnez le champ **[!UICONTROL De]**, mettez en surbrillance et **supprimez** le nom actuel.

   ![](assets/personalize-an-email-2.png)

1. Cliquez sur l’icône **Jeton** à droite du champ **[!UICONTROL De]** .

   ![](assets/personalize-an-email-3.png)

1. Recherchez et sélectionnez le jeton **`{{lead.Lead Owner First Name}}`**.

   ![](assets/personalize-an-email-4.png)

1. Saisissez le nom de votre société et un tiret pour la **valeur par défaut** afin de vous assurer qu’un élément s’affiche si le prénom du représentant de la vente n’est pas disponible. Cliquez sur **Insérer**.

   ![](assets/personalize-an-email-5.png)

1. Appuyez sur la barre d’espace dans le champ **[!UICONTROL De]**, en vous assurant que le curseur clignote un espace après le jeton que vous venez d’insérer. Cliquez de nouveau sur l&#39;icône **Jeton** .

   ![](assets/personalize-an-email-6.png)

1. Recherchez et sélectionnez le jeton **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/personalize-an-email-7.png)

1. Saisissez &quot;Sales&quot; pour la **Valeur par défaut** et cliquez sur **Insérer**.

   ![](assets/personalize-an-email-8.png)

## Étape 3 : Ajout du nom du prospect au courrier électronique {#step-add-the-leads-name-to-the-email}

1. Sélectionnez la section modifiable supérieure, cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Modifier]**.

   ![](assets/personalize-an-email-9.png)

1. Ajoutez un espace après &quot;Hello&quot; et placez votre curseur devant la virgule, puis cliquez sur l’icône **Insérer un jeton** .

   ![](assets/personalize-an-email-10.png)

1. Recherchez et sélectionnez le jeton **`{{lead.First Name}}`**.

   ![](assets/personalize-an-email-11.png)

1. Entrez &quot;Friend&quot; (ou toute étiquette de votre choix) dans le champ **[!UICONTROL Default Value]** et cliquez sur **[!UICONTROL Insert]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Incluez toujours une valeur par défaut pour les jetons. Ainsi, la valeur par défaut sera affichée dans l’email si certaines informations personnelles sont manquantes.

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/personalize-an-email-13.png)

1. Sous **[!UICONTROL Actions par e-mail]**, sélectionnez **[!UICONTROL Approuver et fermer]**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>Vous avez besoin d’une actualisation rapide sur la manière de vous envoyer l’email ? Voir [Envoyer un message électronique](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Mission accomplie {#mission-complete}

Félicitations, vous avez personnalisé votre email !

<br> 

[◄ Mission 6 : Déchirer, Consommer, Infirmier](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Mission 8 : Alerter le représentant commercial ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
