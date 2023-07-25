---
description: Stream Designer - Documents Marketo - Documentation du produit
title: Designer de flux
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
feature: Dynamic Chat
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 2%

---

# Designer de flux {#stream-designer}

Il y a _many_ combinaisons de diffusion possibles. Cet article contient un exemple dans lequel le spécialiste du marketing demande au visiteur du site s’il lui pose des questions sur un produit. Si oui, le visiteur peut planifier un rendez-vous. Si ce n’est pas le cas, le visiteur a la possibilité de s’inscrire à une liste de distribution pour une correspondance ultérieure. On leur offre aussi un PDF gratuit. L’objectif final est de planifier un rendez-vous ou de collecter l’email du visiteur.

>[!PREREQUISITES]
>
>Avant de pouvoir utiliser la carte Document, vous devez d’abord [configurer](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"} dans votre compte d’Adobe.

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
  <td><strong>Document</strong></td>
  <td>Permet d’incorporer des documents PDF dans les boîtes de dialogue et de suivre l’activité d’engagement des visiteurs dans les documents (nombre de pages consultées, téléchargement du document et/ou tout terme de recherche utilisé).</td>
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

## Icônes du concepteur de diffusion en continu {#stream-designer-icons}

Dans le coin supérieur droit du concepteur de flux, vous verrez quelques icônes. Voici ce qu&#39;ils font.

<table>
 <tr>
  <td><img src="assets/stream-designer-1.png"></td>
  <td>Ajoute une grille à l’arrière-plan pour ceux qui préfèrent cette vue.</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-2.png"></td>
  <td>Zoom avant, création de cartes plus grandes</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-3.png"></td>
  <td>Zoom arrière, création de cartes plus petites</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-4.png"></td>
  <td>Ouvre une fenêtre pour que vous puissiez tester votre conversation (appuyez sur le même bouton pour fermer).</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-5.png"></td>
  <td>Organise toutes les cartes dans votre flux</td>
 </tr>
</table>

## Création d’un flux {#create-a-stream}

1. Après avoir [créer votre boîte de dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}, cliquez sur le bouton **Concepteur de diffusion** .

   ![](assets/stream-designer-6.png)

1. Faites glisser et déposez la carte Question .

   ![](assets/stream-designer-7.png)

1. Sous Réponse Chatbot, entrez votre question comme vous le souhaitez.

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >Vous pouvez personnaliser l’expérience des visiteurs connus du chat à l’aide de jetons (par exemple : Hello `{{lead.leadFirstName:""}}`). Il vous suffit de cliquer sur l’icône d’accolade à droite pour effectuer votre sélection. Ajoutez une valeur par défaut entre les guillemets si vous souhaitez que les visiteurs anonymes voient quelque chose de générique (par exemple : Hello `{{lead.leadFirstName:"there"}}`).

   >[!NOTE]
   >
   >Par défaut, le point est activé, ce qui affiche la question d’ouverture en regard de l’icône de conversation sans que le visiteur ait à cliquer dessus pour l’afficher. Poke n’est disponible que sur la première carte de la conversation.

1. Saisissez vos réponses utilisateur et cliquez sur **Enregistrer**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**Modifier les valeurs stockées** est une étape facultative pour ceux qui souhaitent stocker une valeur différente dans la base de données de celle affichée pour les visiteurs dans le chatbot pour les attributs mappés dans la carte de question (par exemple : le visiteur voit &quot;Optimisation du moteur de recherche&quot;, vous stockez cette valeur comme &quot;SEO&quot;.

1. Pour &quot;Oui&quot;, nous voulons planifier un rendez-vous. Par conséquent, en dessous de cette option, faites glisser sur la carte Planificateur de rendez-vous .

   ![](assets/stream-designer-10.png)

1. Dans la colonne de droite, cliquez sur **Enregistrer**.

   ![](assets/stream-designer-11.png)

1. Comme il s’agit d’un objectif, faites glisser la carte Objectif sous le Planificateur de rendez-vous.

   ![](assets/stream-designer-12.png)

1. Nommez votre objectif (ou choisissez un objectif existant) et cliquez sur **Enregistrer**.

   ![](assets/stream-designer-13.png)

1. Pour &quot;Non&quot;, nous voulons voir s’ils vont rejoindre la liste de distribution. Par conséquent, sous cette option, faites glisser sur une autre carte Question .

   ![](assets/stream-designer-14.png)

1. Saisissez votre réponse et ajoutez des choix de réponse pour le visiteur. Cliquez sur **Enregistrer** une fois terminé.

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >Vous pouvez ajouter d’autres réponses en cliquant sur **Ajouter une réponse**.

1. Sous la réponse &quot;Oui&quot;, faites glisser la souris sur la carte Capture d’informations afin de collecter l’email du visiteur.

   ![](assets/stream-designer-16.png)

1. Cliquez sur le bouton **Type** et sélectionnez **Email**.

   ![](assets/stream-designer-17.png)

1. Saisissez un message de chatterbot et un espace réservé. Assurez-vous que l’attribut est mappé sur le champ approprié dans Marketo et cliquez sur **Enregistrer**.

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td><strong>Type</strong></td>
     <td>Le type d’informations que vous souhaitez capturer : Téléphone, Texte, Email.</td>
    </tr>
    <tr>
     <td><strong>Message du chatbot</strong></td>
     <td>Le message que le visiteur voit l’invite à fournir les informations.</td>
    </tr>
    <tr>
     <td><strong>Espace réservé</strong></td>
     <td>Exemple de texte aidant le visiteur à voir ce qu’il doit entrer.</td>
    </tr>
    <tr>
     <td><strong>Mapper la réponse à l’attribut</strong></td>
     <td>Permet de synchroniser la réponse du visiteur avec le champ correspondant dans son enregistrement Personne de votre abonnement Marketo.</td>
    </tr>
   </table>

1. Puisque la collecte de leur email est un objectif, faites glisser la carte Objectif sous Capture d’informations.

   ![](assets/stream-designer-19.png)

1. Nommez votre objectif (ou choisissez un objectif existant) et cliquez sur **Enregistrer**.

   ![](assets/stream-designer-20.png)

1. N’oubliez pas d’ajouter une réponse s’ils disent &quot;Non&quot;. Une option consiste à faire glisser une carte Message ci-dessous et à dire &quot;merci quand même&quot;. Mais dans cet exemple, nous allons plutôt leur fournir un document de PDF gratuit.

   ![](assets/stream-designer-21.png)

1. Dans cet exemple, nous allons créer un nouveau document. Attribuez-lui un nom, saisissez l’URL du PDF que vous avez déjà hébergé, puis cliquez sur **Enregistrer**.

   ![](assets/stream-designer-22.png)

1. Sélectionnez la **Aperçu** bascule pour afficher l’aperçu de votre dialogue.

   ![](assets/stream-designer-23.png)

1. Lorsque vous êtes prêt à activer votre dialogue, cliquez sur **Publier**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>Avant de cliquer sur Publier, n’oubliez pas de vous assurer que vous avez [ont saisi votre ou vos URL cibles.](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Créer un dialogue](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}
>* [Critère d’audience](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target="_blank"}
>* Rapports [ ](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target="_blank"}
>* [Utilisation de la carte de document](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"}
