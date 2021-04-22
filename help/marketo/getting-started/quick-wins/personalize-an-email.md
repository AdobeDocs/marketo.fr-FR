---
unique-page-id: 2359422
description: Personnalisation d’un courrier électronique - Documents Marketo - Documentation du produit
title: Personnaliser un e-mail
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 10%

---

# Personnaliser un e-mail {#personalize-an-email}

## Mission : Rendez vos courriers électroniques personnels en ajoutant des jetons de données {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Configurer et Ajouter une personne](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [Envoyer un E-mail de masse](/help/marketo/getting-started/quick-wins/send-an-email.md)
>* [Marketing goutte à goutte et fidélisation](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)


## Étape 1 : Sélectionner un courriel à personnaliser {#step-select-an-email-to-personalize}

1. Sélectionnez l&#39;un des messages électroniques d&#39;accueil créés dans le fichier [précédent quick win](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md) et cliquez sur **Modifier le brouillon**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Une copie de cet e-mail sera créée en tant que brouillon. Vous devez approuver le brouillon pour que les modifications soient mises en oeuvre.

Si vous n&#39;avez pas activé de blocage des fenêtres contextuelles, l&#39;éditeur de messages électroniques s&#39;ouvre dans un nouvel onglet/une nouvelle fenêtre. Sinon, cliquez deux fois sur **Modifier le brouillon**.

## Étape 2 : Faire du vendeur l&#39;expéditeur {#step-make-the-salesperson-the-sender}

1. Sélectionnez le champ **De**, mettez en surbrillance et **supprimez** le nom actuel.

   ![](assets/two-5.png)

1. Cliquez sur l&#39;icône **Jeton** située à droite du champ **De**.

   ![](assets/three-4.png)

1. Recherchez et sélectionnez le jeton **`{{lead.Lead Owner First Name}}`**.

   ![](assets/four-3.png)

1. Tapez le nom de votre société et un tiret pour la valeur **Valeur par défaut** afin de vous assurer que quelque chose s&#39;affiche au cas où le prénom du représentant de la vente ne serait pas disponible. Cliquez sur **Insérer**.

   ![](assets/five-4.png)

1. Cliquez sur la barre d’espace dans le champ **From**, en veillant à ce que le curseur clignote un espace après le jeton que vous venez d’insérer. Cliquez de nouveau sur l’icône **Jeton**.

   ![](assets/six-4.png)

1. Recherchez et sélectionnez le jeton **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/seven-5.png)

1. Saisissez &quot;Sales&quot; pour la **Valeur par défaut** et cliquez sur **Insérer**.

   ![](assets/eight-3.png)

## Étape 3 : Ajouter le nom du prospect au courrier électronique {#step-add-the-leads-name-to-the-email}

1. Sélectionnez la section modifiable supérieure, cliquez sur l’icône d’engrenage et sélectionnez **Modifier**.

   ![](assets/nine-2.png)

1. Ajoutez un espace après &quot;Hello&quot; et placez votre curseur devant la virgule, puis cliquez sur l&#39;icône **Insérer un jeton**.

   ![](assets/ten-4.png)

1. Recherchez et sélectionnez le jeton **`{{lead.First Name}}`**.

   ![](assets/eleven-4.png)

1. Saisissez &quot;Friend&quot; (ou toute étiquette que vous souhaitez) dans le champ **Valeur par défaut** et cliquez sur **Insérer**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >toujours inclure une valeur par défaut pour les jetons ; ainsi, la valeur par défaut sera affichée dans le courrier électronique si une partie des informations personnelles est manquante.

1. Cliquez sur **Enregistrer**.

   ![](assets/thirteen-3.png)

1. Fermez l’onglet/la fenêtre de l’éditeur de courrier électronique.

   ![](assets/fourteen-3.png)

1. Sous **Actions de courriel**, sélectionnez **Approuver le brouillon**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>Vous avez besoin d&#39;une actualisation rapide de la façon de vous envoyer le courriel ? Voir [Envoyer un message électronique ](/help/marketo/getting-started/quick-wins/send-an-email.md).

### Mission accomplie {#mission-complete}

Félicitations, vous avez personnalisé votre e-mail !

<br> 

[◄ Mission 6 : Marketing goutte à goutte et fidélisation](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Mission 8 : Prévenir un représentant commercial ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
