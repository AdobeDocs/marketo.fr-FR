---
description: Dialogues - Documents Marketo - Documentation du produit
title: Dialogues
hide: true
hidefromtoc: true
source-git-commit: c46902686f1d5af63a51f5eaae2dc0e6afe99629
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Dialogues {#dialogues}

Les boîtes de dialogue sont les conversations spécifiques que vous configurez. Ils peuvent être personnalisés par aspect, ainsi que par ce qui est dit et qui le voit.

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

Tout comme les listes dynamiques Marketo, les attributs Critères d’audience vous permettent de définir votre audience cible.

Il existe plusieurs attributs parmi lesquels choisir. Dans cet exemple, nous choisissons l’état de piste _est_ Californie et la taille de la société _est supérieure à_ 50.

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
>L’utilisation d’un astérisque agit comme un caractère générique fourre-tout. `https://*.website.com` placerait donc la boîte de dialogue sur chaque page du site, y compris les sous-domaines (par exemple : support.website.com). Et `https://website.com/folder/*` placerait la boîte de dialogue sur chaque page HTML dans le dossier suivant (par exemple : dans ce cas, disons que le dossier est &quot;sports&quot;, donc : website.com/sports/baseball.html, website.com/sports/football.html, etc.).
