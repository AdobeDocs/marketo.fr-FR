---
unique-page-id: 2359422
description: Personnalisation d’un courrier électronique - Documents Marketo - Documentation du produit
title: Personnaliser un e-mail
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 8%

---

# Personnaliser un e-mail {#personalize-an-email}

## Mission : Personnaliser vos emails en ajoutant des jetons de données {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configuration et ajout d’une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Envoyer un message électronique](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}
>* [Déchets, goutte, Infirmière](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;}


## Étape 1 : Sélectionner un email à personnaliser {#step-select-an-email-to-personalize}

1. Sélectionnez l’un des messages électroniques d’accueil créés dans la [aperçu rapide précédent](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;} et cliquez sur **Modifier le brouillon**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Une copie de cet e-mail sera créée en tant que brouillon. Vous devez approuver le brouillon pour que les modifications soient mises en ligne.

Si vous n’avez pas activé de bloqueur de fenêtres contextuelles, l’éditeur de courrier électronique s’ouvre dans un nouvel onglet/nouvelle fenêtre. Sinon, cliquez sur **Modifier le brouillon** deux fois.

## Étape 2 : Faire du vendeur l’expéditeur {#step-make-the-salesperson-the-sender}

1. Sélectionnez la **De** champ, mise en surbrillance et **delete** nom actuel.

   ![](assets/two-5.png)

1. Cliquez sur le bouton **Jeton** à droite de l’icône **De** champ .

   ![](assets/three-4.png)

1. Recherchez et sélectionnez la variable **`{{lead.Lead Owner First Name}}`** jeton.

   ![](assets/four-3.png)

1. Saisissez le nom de votre société et un tiret pour le champ **Valeur par défaut** pour s’assurer qu’un élément s’affiche au cas où le prénom du représentant de la vente n’est pas disponible. Cliquez sur **Insérer**.

   ![](assets/five-4.png)

1. Accédez à la barre d’espace dans le **De** , assurez-vous que le curseur clignote un espace après le jeton que vous venez d’insérer. Cliquez ensuite sur le bouton **Jeton** à nouveau.

   ![](assets/six-4.png)

1. Recherchez et sélectionnez la variable **`{{lead.Lead Owner Last Name}}`** jeton.

   ![](assets/seven-5.png)

1. Saisissez &quot;Sales&quot; pour la variable **Valeur par défaut** et cliquez sur **Insérer**.

   ![](assets/eight-3.png)

## Étape 3 : Ajout du nom du prospect au courrier électronique {#step-add-the-leads-name-to-the-email}

1. Sélectionnez la section modifiable supérieure, cliquez sur l’icône d’engrenage et sélectionnez **Modifier**.

   ![](assets/nine-2.png)

1. Ajoutez un espace après &quot;Hello&quot; et placez votre curseur devant la virgule, puis cliquez sur le bouton **Insérer un jeton** icône .

   ![](assets/ten-4.png)

1. Recherchez et sélectionnez la variable **`{{lead.First Name}}`** jeton.

   ![](assets/eleven-4.png)

1. Saisissez &quot;Ami&quot; (ou toute étiquette de votre choix) dans le champ **Valeur par défaut** champ et clic **Insérer**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Incluez toujours une valeur par défaut pour les jetons ; ainsi, la valeur par défaut sera affichée dans l’email si une partie des informations personnelles est manquante.

1. Cliquez sur **Enregistrer**.

   ![](assets/thirteen-3.png)

1. Fermez l&#39;onglet/la fenêtre de l&#39;éditeur d&#39;email.

   ![](assets/fourteen-3.png)

1. Sous **Actions de courrier électronique**, sélectionnez **Approuver le brouillon**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>Vous avez besoin d’une actualisation rapide sur la manière de vous envoyer l’email ? Voir [Envoyer un message électronique](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}.

### Mission accomplie {#mission-complete}

Félicitations, vous avez personnalisé votre email !

<br> 

[◄ Mission 6 : Marketing goutte à goutte et fidélisation](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Mission 8 : Prévenir un représentant commercial ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
