---
description: Stream Designer - Documents Marketo - Documentation du produit
title: Concepteur de diffusion
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: 38e65efc50f7f5e7a2a3dbe91035327007475721
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Concepteur de diffusion {#stream-designer}

Il y a _many_ combinaisons de flux que vous pouvez créer. Cet article contient un exemple dans lequel le spécialiste du marketing demande au visiteur du site s’il lui pose des questions sur un produit. Si oui, le visiteur peut planifier un rendez-vous. Si ce n’est pas le cas, le visiteur a la possibilité de s’inscrire à une liste de distribution pour une correspondance ultérieure. L’objectif est de planifier un rendez-vous ou de collecter l’adresse électronique du visiteur.

## Diffusion en continu de cartes Designer {#stream-designer-cards}

Le concepteur de flux contient plusieurs cartes que vous pouvez ajouter pour façonner la conversation de conversation.

<table>
 <tr>
  <td><strong>Message</strong></td>
  <td>Utilisez cette option lorsque vous souhaitez faire une déclaration sans réponse nécessaire (par exemple : "Salut ! Tous les articles ont une remise de 25 % aujourd’hui avec le code SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Question</strong></td>
  <td>Utilisez cette option lorsque vous souhaitez poser une question à choix multiples, à laquelle vous fournissez les réponses disponibles (par exemple : Quel type de véhicule vous intéresse ? Réponses = VUS, Compacte, Camion, etc.).</td>
 </tr>
 <tr>
  <td><strong>Capture d’informations</strong></td>
  <td>Utilisez lorsque vous souhaitez collecter des informations. Les trois champs à choisir sont Adresse électronique, Numéro de téléphone et Texte (ce qui permet au visiteur d’écrire son propre message).</td>
 </tr>
 <tr>
  <td><strong>Planificateur de rendez-vous</strong></td>
  <td>Fournit au visiteur un calendrier des dates disponibles pour planifier un suivi. La disponibilité du calendrier reflète <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">l’agent suivant en ligne</a>.</td>
 </tr>
 <tr>
  <td><strong>Objectif</strong></td>
  <td>Il s’agit de la seule carte que les visiteurs ne verront pas. Il vous appartient de déterminer à quel moment un objectif est atteint dans le chat spécifique (par exemple : Si la collecte de l’e-mail du visiteur est votre objectif, placez la carte Objectif immédiatement après la capture d’informations dans le flux).</td>
 </tr>
</table>

## Création d’un flux {#create-a-stream}

1. Après avoir [créer votre boîte de dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md), cliquez sur le bouton **Concepteur de diffusion** .

   ![](assets/create-a-stream-1.png)

1. Faites glisser et déposez la carte Question .

   ![](assets/create-a-stream-2.png)

1. Sous Réponse Chatbot, entrez votre question comme vous le souhaitez.

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >Par défaut, le point est activé, ce qui affiche la question d’ouverture en regard de l’icône de conversation sans que le visiteur ait à cliquer dessus pour l’afficher.

1. Saisissez vos réponses utilisateur et cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-4.png)

1. Pour &quot;Oui&quot;, nous voulons planifier un rendez-vous. Par conséquent, en dessous de cette option, faites glisser sur la carte Planificateur de rendez-vous .

   ![](assets/create-a-stream-5.png)

1. Dans la colonne de droite, cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-6.png)

1. Comme il s’agit d’un objectif, faites glisser la carte Objectif sous le Planificateur de rendez-vous.

   ![](assets/create-a-stream-7.png)

1. Nommez votre objectif (ou choisissez un objectif existant) et cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-8.png)

1. Pour &quot;Non&quot;, nous voulons voir s’ils vont rejoindre la liste de distribution. Par conséquent, sous cette option, faites glisser sur une autre carte Question .

   ![](assets/create-a-stream-9.png)

1. Saisissez votre réponse et ajoutez des choix de réponse pour le visiteur. Cliquez sur **Enregistrer** une fois terminé.

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >Vous pouvez ajouter d’autres réponses en cliquant sur **Ajouter une réponse**.

1. Sous la réponse &quot;Oui&quot;, faites glisser la souris sur la carte Capture d’informations afin de collecter l’email du visiteur.

   ![](assets/create-a-stream-11.png)

1. Cliquez sur le bouton **Type** et sélectionnez **Email**.

   ![](assets/create-a-stream-12.png)

1. Saisissez un message de chatterbot et un espace réservé. Assurez-vous que l’attribut est mappé sur le champ approprié dans Marketo et cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>Type</strong></td>
     <td>Le type d’informations que vous souhaitez capturer : Téléphone, Texte, Email.</td>
    </tr>
    <tr>
     <td><strong>Message de chatbot</strong></td>
     <td>Le message que le visiteur voit l’invite à fournir les informations.</td>
    </tr>
    <tr>
     <td><strong>Paramètre fictif</strong></td>
     <td>Exemple de texte aidant le visiteur à voir ce qu’il doit entrer.</td>
    </tr>
    <tr>
     <td><strong>Associer la réponse à l’attribut</strong></td>
     <td>Permet de synchroniser la réponse du visiteur avec le champ correspondant dans son enregistrement Personne de votre abonnement Marketo.</td>
    </tr>
   </table>

1. Puisque la collecte de leur email est un objectif, faites glisser la carte Objectif sous Capture d’informations.

   ![](assets/create-a-stream-14.png)

1. Nommez votre objectif (ou choisissez un objectif existant) et cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-15.png)

1. N’oubliez pas d’ajouter une réponse s’ils disent &quot;Non&quot;. Faites glisser une carte Message sous cette option.

   ![](assets/create-a-stream-16.png)

1. Saisissez votre message et cliquez sur **Enregistrer**.

   ![](assets/create-a-stream-17.png)

1. Sélectionnez la **Aperçu** bascule pour afficher l’aperçu de votre dialogue.

   ![](assets/create-a-stream-18.png)

1. Lorsque vous êtes prêt à activer votre dialogue, cliquez sur **Publier**.

   ![](assets/create-a-stream-19.png)

>[!NOTE]
>
>Avant de cliquer sur Publier, n’oubliez pas de vous assurer que vous avez [ont saisi votre ou vos URL cibles.](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#target).

>[!MORELIKETHIS]
>
>* [Créer un dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Critères d’audience](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target=&quot;_blank&quot;}
>* [Rapports](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}
