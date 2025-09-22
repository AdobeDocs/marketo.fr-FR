---
unique-page-id: 14352546
description: Empêcher l’intégration d’une adresse Gmail Secondaire à Sales Connect - Documents Marketo - Documentation du produit
title: Empêchement de l’intégration d’une adresse Gmail secondaire à Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 2%

---

# Empêcher l’intégration d’une adresse Gmail Secondaire à [!DNL Sales Connect] {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Intégration de Gmail rompue (pourquoi mon profil Gmail envoie-t-il des emails) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

La raison la plus courante de l’interruption d’une connexion Gmail est une intégration accidentelle au compte personnel d’un utilisateur. Cela peut se produire lorsqu’un utilisateur clique sur « Se connecter » ou tente d’envoyer un e-mail à partir de son compte personnel. Cela peut être très tentant, car l’option existera lors de l’accès à votre compte Gmail dans la même instance de [!DNL Chrome]que votre e-mail professionnel.

## Pourquoi essaie-t-[!DNL Sales Connect] même de m’intégrer à mon Gmail personnel ? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

[!DNL Sales Connect] s’intègre à Gmail par le biais d’une extension installée dans le navigateur [!DNL Chrome]. Chaque fois que l’extension envoie une instance de Gmail ouverte, elle offre une option permettant de l’intégrer. Pour éviter toute intégration avec votre compte Gmail personnel, nous vous recommandons l’une des trois actions suivantes...

Se Connecter En Tant Qu&#39;Autre [!DNL Chrome]Utilisateur Recommandé)

Cliquez sur [ce lien](https://support.google.com/chrome/answer/2364824?hl=en) pour savoir comment créer un autre [!DNL Chrome]Profil.

**Avantages** : la connexion en tant qu’autre utilisateur ouvre une nouvelle instance de [!DNL Chrome]. Cette instance est une toute nouvelle fenêtre d’[!DNL Chrome], et aucune de vos anciennes extensions n’existera dans celle-ci. Il conserve également des cookies afin que vous n&#39;ayez pas à vous connecter à votre Gmail à chaque fois.

**Inconvénients** : Deux fenêtres de [!DNL Chrome] doivent être ouvertes.

Utiliser un autre navigateur

**Avantages :** l’utilisation d’un autre navigateur Internet (IE ou Firefox) sans extension installée empêchera cela.

**Inconvénients** : l’utilisation de plusieurs navigateurs peut être ennuyeuse.

Utiliser Une Fenêtre Incognito

**Avantages :** une fenêtre en mode privé revient à ouvrir une version nue d’[!DNL Chrome]. En d’autres termes, aucune de vos extensions n’y sera installée et [!DNL Sales Connect] ne sera pas là pour se connecter.

**Inconvénients** : Vous devrez vous connecter à Gmail chaque fois que vous commencerez votre journée, et de nouveau si vous fermez accidentellement la fenêtre.
