---
unique-page-id: 2359422
description: Personnalisation d’un courrier électronique - Documents Marketo - Documentation du produit
title: Personnaliser un e-mail
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
source-git-commit: 80512816eaf0a70a3f10a50c34aeea14edd9046b
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 10%

---

# Personnaliser un e-mail {#personalize-an-email}

## Mission : Personnaliser vos emails en ajoutant des jetons de données {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configuration et ajout d’une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Envoyer un E-mail de masse](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [Marketing goutte à goutte et fidélisation](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}


## Étape 1 : Sélectionner un email à personnaliser {#step-select-an-email-to-personalize}

1. Sélectionnez l’un des messages électroniques d’accueil créés dans la [aperçu rapide précédent](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} et cliquez sur **[!UICONTROL Créer un brouillon]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Une copie de cet e-mail sera créée en tant que brouillon. N’oubliez pas d’approuver le brouillon pour que les modifications soient mises en ligne.

Si vous n’avez pas activé de bloqueur de fenêtres contextuelles, l’éditeur de courrier électronique s’ouvre dans un nouvel onglet/nouvelle fenêtre. Sinon, cliquez sur **[!UICONTROL Créer un brouillon]** deux fois.

## Étape 2 : Faire du vendeur l’expéditeur {#step-make-the-salesperson-the-sender}

1. Sélectionnez la **[!UICONTROL De]** champ, mise en surbrillance et **delete** nom actuel.

   ![](assets/personalize-an-email-2.png)

1. Cliquez sur le bouton **Jeton** à droite de l’icône **[!UICONTROL De]** champ .

   ![](assets/personalize-an-email-3.png)

1. Recherchez et sélectionnez la variable **`{{lead.Lead Owner First Name}}`** jeton.

   ![](assets/personalize-an-email-4.png)

1. Saisissez le nom de votre société et un tiret pour le champ **Valeur par défaut** pour s’assurer qu’un élément s’affiche au cas où le prénom du représentant de la vente n’est pas disponible. Cliquez sur **Insérer**.

   ![](assets/personalize-an-email-5.png)

1. Accédez à la barre d’espace dans le **[!UICONTROL De]** , assurez-vous que le curseur clignote un espace après le jeton que vous venez d’insérer. Cliquez ensuite sur le bouton **Jeton** à nouveau.

   ![](assets/personalize-an-email-6.png)

1. Recherchez et sélectionnez la variable **`{{lead.Lead Owner Last Name}}`** jeton.

   ![](assets/personalize-an-email-7.png)

1. Saisissez &quot;Sales&quot; pour la variable **Valeur par défaut** et cliquez sur **Insérer**.

   ![](assets/personalize-an-email-8.png)

## Étape 3 : Ajout du nom du prospect au courrier électronique {#step-add-the-leads-name-to-the-email}

1. Sélectionnez la section modifiable supérieure, cliquez sur l’icône d’engrenage et sélectionnez **[!UICONTROL Modifier]**.

   ![](assets/personalize-an-email-9.png)

1. Ajoutez un espace après &quot;Hello&quot; et placez votre curseur devant la virgule, puis cliquez sur le bouton **Insérer un jeton** icône .

   ![](assets/personalize-an-email-10.png)

1. Recherchez et sélectionnez la variable **`{{lead.First Name}}`** jeton.

   ![](assets/personalize-an-email-11.png)

1. Saisissez &quot;Ami&quot; (ou toute étiquette de votre choix) dans le champ **[!UICONTROL Valeur par défaut]** champ et clic **[!UICONTROL Insérer]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Incluez toujours une valeur par défaut pour les jetons ; ainsi, la valeur par défaut sera affichée dans l’email si une partie des informations personnelles est manquante.

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/personalize-an-email-13.png)

1. Sous **[!UICONTROL Actions de courrier électronique]** et sélectionnez **[!UICONTROL Approuver et fermer]**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>Vous avez besoin d’une actualisation rapide sur la manière de vous envoyer l’email ? Voir [Envoyer un message électronique](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Mission accomplie {#mission-complete}

Félicitations, vous avez personnalisé votre email !

<br> 

[◄ Mission 6 : Marketing goutte à goutte et fidélisation](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Mission 8 : Prévenir un représentant commercial ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
