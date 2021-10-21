---
description: Création d’un flux - Documentation Marketo Docs - Documentation du produit
title: Création d’un flux
hide: true
hidefromtoc: true
source-git-commit: 1022d3eaf4ee4a1686c5d8ae3168ee0197776289
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# Création d’un flux {#create-a-stream}

Il y a _nombreux_ des combinaisons de flux que vous pouvez créer. Voici un exemple où le spécialiste du marketing demande au visiteur du site s’il lui pose des questions sur le produit. Si oui, le visiteur peut planifier un rendez-vous. Si tel n&#39;est pas le cas, le visiteur a la possibilité de s&#39;inscrire à une liste d&#39;envoi pour une correspondance ultérieure. L’objectif est soit de planifier un rendez-vous, soit de recueillir l’e-mail du visiteur.

1. Après [créer votre dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#create-a-new-dialogue), cliquez sur le bouton **Stream Designer** .

   ![](assets/create-a-stream-1.png)

1. Faites glisser et déposez la carte de questions.

   ![](assets/create-a-stream-2.png)

1. Sous Chatbot Response, dites votre question comme vous voulez.

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >Poke est activé par défaut, ce qui affiche la question d’ouverture en regard de l’icône de chat sans que le visiteur n’ait à cliquer dessus pour la voir.

1. Saisissez vos réponses utilisateur et cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-4.png)

1. Pour &quot;Oui&quot;, nous voulons planifier un rendez-vous. En dessous de cette option, faites glisser le pointeur sur la carte du Planificateur de rendez-vous.

   ![](assets/create-a-stream-5.png)

1. Dans la colonne de droite, cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-6.png)

1. Comme il s&#39;agit d&#39;un objectif, faites glisser la carte Objectif sous le Planificateur de rendez-vous.

   ![](assets/create-a-stream-7.png)

1. Nommez votre objectif (ou choisissez un objectif existant) et cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-8.png)

1. Pour &quot;Non&quot;, nous voulons voir s&#39;ils vont s&#39;inscrire à la liste de diffusion. En dessous de cette option, faites glisser le pointeur sur une autre carte de questions.

   ![](assets/create-a-stream-9.png)

1. Saisissez votre réponse et ajoutez des choix de réponse pour le visiteur. Cliquez sur **Enregistrer** une fois terminé.

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >Vous pouvez ajouter d’autres réponses en cliquant sur **Ajouter une réponse**.

1. Sous la réponse &quot;Oui&quot;, faites glisser le pointeur sur la carte de capture d’informations pour collecter l’e-mail du visiteur.

   ![](assets/create-a-stream-11.png)

1. Cliquez sur le bouton **Type** et sélectionnez **E-mail**.

   ![](assets/create-a-stream-12.png)

1. Entrez un message de chatbot et un espace réservé. Assurez-vous que l’attribut est mappé sur le champ approprié dans Marketo et cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>Type</strong></td>
     <td>Type d’informations à capturer : Téléphone, Texte, E-mail.</td>
    </tr>
    <tr>
     <td><strong>Message Chatbot</strong></td>
     <td>Le message que le visiteur voit l’invitant à fournir les informations.</td>
    </tr>
    <tr>
     <td><strong>Paramètre fictif</strong></td>
     <td>Exemple de texte pour aider le visiteur à voir ce qu’il doit saisir.</td>
    </tr>
    <tr>
     <td><strong>Mapper la réponse à l'attribut</strong></td>
     <td>Permet de synchroniser la réponse du visiteur avec le champ correspondant dans son enregistrement de personne dans votre abonnement Marketo.</td>
    </tr>
   </table>

1. Comme la collecte de leur courrier électronique est un objectif, faites glisser la carte Objectif sous Capture d’informations.

   ![](assets/create-a-stream-14.png)

1. Nommez votre objectif (ou choisissez un objectif existant) et cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-15.png)

1. N&#39;oubliez pas d&#39;ajouter une réponse s&#39;ils disent &quot;Non&quot;. Faites glisser une carte de message sous cette option.

   ![](assets/create-a-stream-16.png)

1. Saisissez votre message, puis cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-17.png)

1. Lorsque vous souhaitez activer votre dialogue, cliquez sur **Publier**.

   ![](assets/create-a-stream-18.png)

>[!NOTE]
>
>Avant de cliquer sur Publier, n&#39;oubliez pas de vous assurer que vous avez [a saisi votre ou vos URL cibles.](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#target).

>[!MORELIKETHIS]
>
>[Dialogues](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)
