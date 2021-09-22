---
description: Dialogues - Documents Marketo - Documentation du produit
title: Dialogues
hide: true
hidefromtoc: true
source-git-commit: d5c1c1d0ce2a521898eaa4f6610bf1ce04b4f66b
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Dialogues {#dialogues}

Les boîtes de dialogue sont les conversations individuelles que vous allez configurer. Découvrez comment les personnaliser visuellement, déterminer les pages sur lesquelles elles apparaissent et déterminer ce qui est dit et qui les voit.

## Créer un dialogue {#create-a-new-dialogue}

1. Cliquez sur **Dialogues**.

PICC

1. Cliquez sur le bouton **Créer** .

PICC

1. Saisissez un nom (la description est facultative), définissez le niveau de priorité, puis cliquez sur **Enregistrer**.

PICC

>[!NOTE]
>
>EXPLIQUER LE NIVEAU DE PRIORITÉ

## Critères d’audience {#audience-criteria}

Tout comme les listes dynamiques Marketo, les attributs Critères d’audience vous permettent de définir votre audience cible. Vous pouvez cibler des pistes connues ou inconnues à l’aide d’attributs déduits, de pistes ou de sociétés (ou d’une combinaison de ces attributs).

Il existe _de nombreuses combinaisons d’attributs_ parmi lesquelles choisir. Dans cet exemple, nous ciblons tous les prospects connus en Californie qui travaillent pour une société de plus de 50 employés.

1. Saisissez l’attribut Etat de piste et faites-le glisser vers la droite.

PICC

1. __ Isis défini par défaut. Dans le champ Sélectionner des valeurs , saisissez CA (vous pouvez également cliquer sur la liste déroulante et sélectionner dans la liste).

PICC

1. Saisissez l’attribut Taille de la société et faites-le glisser vers la droite.

PICC

1. Cliquez sur la liste déroulante des opérateurs et sélectionnez Supérieur à.

PICC

1. Saisissez 50, puis cliquez ailleurs à l’écran pour enregistrer.

PICC

COMMENT CAPTURER LES PISTES D’ANON

REMARQUE : peut-être mentionné le fonctionnement/l’affichage inféré d’un cas d’utilisation, l’e-mail de piste est vide.

## Ajout de groupes {#add-groups}

Vous avez également la possibilité de regrouper des attributs, au cas où vous souhaitez tous avoir certains attributs avec &quot;n’importe lequel&quot; d’un autre.

FINISSEZ CECI

## Cible {#target}

C’est là que vous saisissez la ou les URL spécifiques sur lesquelles doit s’afficher un dialogue spécifique.

Formats acceptables :

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>L’utilisation d’un astérisque agit comme un caractère générique fourre-tout. `https://*.website.com` placerait donc la boîte de dialogue sur chaque page du site, y compris les sous-domaines (par exemple : `support.website.com`). Et `https://website.com/folder/*` placerait la boîte de dialogue sur chaque page HTML dans le dossier suivant (par exemple : dans ce cas, disons que le dossier est &quot;sports&quot;, donc : website.com/sports/baseball.html, website.com/sports/football.html, etc.).

## Concepteur de diffusion {#stream-designer}

Le concepteur de flux contient différentes cartes que vous pouvez ajouter pour façonner la conversation de conversation.

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
  <td>Fournit au visiteur un calendrier des dates disponibles pour planifier un suivi. La disponibilité du calendrier reflète [l’agent suivant en ligne](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing).</td>
 </tr>
 <tr>
  <td><strong>Objectif</strong></td>
  <td>Il s’agit de la seule carte que les visiteurs ne verront pas. Il vous appartient de déterminer à quel moment un objectif est atteint dans le chat spécifique (par exemple : Si la collecte de l’e-mail du visiteur est votre objectif, placez la carte Objectif après Capture d’informations dans le flux).</td>
 </tr>
</table>

PROPRE SECTION POSSIBLE

AFFICHER LES EXEMPLES CI-DESSOUS