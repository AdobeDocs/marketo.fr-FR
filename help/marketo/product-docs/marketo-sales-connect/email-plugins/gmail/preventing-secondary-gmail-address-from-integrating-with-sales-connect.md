---
unique-page-id: 14352546
description: Prévention de l’intégration des adresses Gmail Secondaire à Sales Connect - Documents Marketo - Documentation du produit
title: Empêcher l’intégration de l’adresse Gmail Secondaire à Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Empêcher l’intégration de l’adresse Gmail Secondaire à Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Intégration de Gmail endommagée (pourquoi mon Gmail personnel envoie-t-il des emails ?) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

La raison la plus courante d’une connexion Gmail rompue est une intégration accidentelle avec le compte personnel d’un utilisateur. Cela peut se produire lorsqu’un utilisateur clique sur &quot;Se connecter&quot; ou lorsqu’il tente d’envoyer un courrier électronique à partir de son compte personnel. Cela peut être très tentant, car l’option existe lors de l’accès à votre compte Gmail dans la même instance de Chrome que votre courrier électronique de travail.

## Pourquoi Sales Connect tente-t-il même de s’intégrer à mon Gmail personnel ? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect s’intègre à Gmail par le biais d’une extension installée dans le navigateur Chrome. Chaque fois que l’extension détecte une instance de Gmail ouverte, elle offre une option d’intégration avec celle-ci. Pour empêcher une intégration avec votre compte Gmail personnel, nous vous recommandons l’une des trois choses suivantes...

Se connecter en tant qu’autre utilisateur Chrome (recommandé)

Cliquez sur [ce lien](https://support.google.com/chrome/answer/2364824?hl=en) pour découvrir comment créer un autre profil Chrome.

**Avantages** : la connexion en tant qu’autre utilisateur ouvre une nouvelle instance de Chrome. Cette instance est une toute nouvelle fenêtre de Chrome et aucune de vos anciennes extensions n’existera dans celle-ci. Il conserve également les cookies afin que vous n’ayez pas à vous connecter à votre Gmail à chaque fois.

**Inconvénients** : deux fenêtres de Chrome doivent être ouvertes.

Utiliser un autre navigateur

**Avantages :** L’utilisation d’un autre navigateur Internet (IE ou Firefox) sur lequel l’extension n’est pas installée empêchera cela.

**Inconvénients** : L’utilisation de plusieurs navigateurs peut être embêtante.

Utiliser Une Fenêtre Incognito

**Avantages :** Une fenêtre incognito est comme ouvrir une version nue de Chrome. En d’autres termes, aucune de vos extensions n’est installée et Sales Connect ne sera pas là pour se connecter.

**Inconvénients** : vous devrez vous connecter à Gmail chaque fois que vous commencerez votre journée, et à nouveau si vous fermez accidentellement la fenêtre.
