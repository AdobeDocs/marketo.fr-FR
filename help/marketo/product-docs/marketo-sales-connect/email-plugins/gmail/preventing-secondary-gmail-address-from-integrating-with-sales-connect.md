---
unique-page-id: 14352546
description: Empêcher l'adresse Gmail Secondaire de s'intégrer à Sales Connect - Marketo Docs - Documentation du produit
title: Prévention de l'intégration de l'adresse Gmail Secondaire à Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# Empêcher l&#39;adresse Gmail Secondaire de s&#39;intégrer à Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Intégration de Gmail rompue (pourquoi mes e-mails personnels Gmail sont-ils envoyés) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

La raison la plus courante d&#39;une connexion Gmail interrompue est une intégration accidentelle avec le compte personnel d&#39;un utilisateur. Cela peut se produire lorsqu’un utilisateur clique sur &quot;Se connecter&quot; ou lorsqu’il tente d’envoyer un courriel à partir de son compte personnel. Cela peut être très tentant car l&#39;option existe lors de l&#39;accès à votre compte Gmail dans la même instance de Chrome que votre courrier électronique de travail.

## Pourquoi Sales Connect tente-t-il même de s&#39;intégrer à mon Gmail personnel ? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect s&#39;intègre à Gmail via une extension installée dans le navigateur Chrome. Chaque fois que l&#39;extension détecte une instance de Gmail open, elle offre une option d&#39;intégration avec elle. Pour éviter une intégration avec votre compte Gmail personnel, nous vous recommandons l&#39;une des trois choses...

Se connecter en tant qu’autre utilisateur Chrome (recommandé)

Cliquez sur [ce lien](http://support.google.com/chrome/answer/2364824?hl=en) pour savoir comment créer un autre Profil Chrome.

**Avantages** : La connexion en tant qu’autre utilisateur ouvre une nouvelle instance de Chrome. Cette instance est une toute nouvelle fenêtre de Chrome, et aucune de vos anciennes extensions n’existera dans celle-ci. Il conserve également les cookies afin que vous n&#39;ayez pas à vous connecter à votre Gmail à chaque fois.

**Contre** : Deux fenêtres de Chrome doivent être ouvertes.

Utiliser un autre navigateur

**Avantages :** L&#39;utilisation d&#39;un autre navigateur Internet (IE ou Firefox) qui ne dispose pas de l&#39;extension empêchera cela.

**Contre** : L’utilisation de plusieurs navigateurs peut être gênante.

Utiliser une fenêtre Incognito

**Avantages :** Une fenêtre incognito est semblable à l’ouverture d’une version nue de Chrome. En d&#39;autres termes, aucune de vos extensions n&#39;est installée et Sales Connect n&#39;est pas là pour se connecter.

**Contre** : Vous devrez vous connecter à Gmail chaque fois que vous début votre journée, et encore si vous fermez accidentellement la fenêtre.
