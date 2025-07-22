---
unique-page-id: 14352405
description: Configuration de la connexion unique via SAML 2.0 in [!DNL Sales Connect] - Documents Marketo - Documentation du produit
title: Configuration de la connexion unique via SAML 2.0 dans  [!DNL Sales Connect]
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Configuration de la connexion unique via SAML 2.0 dans [!DNL Sales Connect] {#setting-up-sso-through-saml-in-sales-connect}

Nous prenons en charge la connexion unique via la spécification SAML 2.0. Cependant, nous n’avons pas d’intégrations directes avec un fournisseur pour le moment. Nous devrons collecter des informations auprès de votre fournisseur SSO pour obtenir cette configuration.

>[!NOTE]
>
>Ceci s’applique uniquement aux utilisateurs de **Marketo Sales Connect**. Si vous ne possédez pas Sales Connect mais souhaitez en savoir plus, veuillez contacter l’équipe chargée du compte Adobe (votre gestionnaire de compte).

## Exigences {#requirements}

* Compte SSO
* Abonnement à Marketo Sales Connect
* Metadata.xml à partir du compte SSO (URL de problème, point d’entrée pour la validation et clé publique)

## Configuration {#setup}

Le fichier metadata.xml de l’instance SSO de votre équipe doit contenir l’URL de l’émetteur, le point d’entrée pour la validation et une clé publique.

Nous aurons également besoin de l&#39;emplacement SSO pour que le compte SSO de votre entreprise soit un domaine unique. Par exemple, nous avons besoin d’un sous-domaine unique tel que `toutapp.pingidentity.com` ou similaire. Sans ce type d’identifiant unique, nous ne pourrons pas configurer SAML à partir du tableau de bord.

Un identifiant de connexion et Okta ne fournissent pas toujours des identifiants uniques lors de l’attribution d’une URL. Si vous utilisez Okta ou One Login, cela signifie que nous ne pourrons pas configurer une connexion à partir du bouton du tableau de bord. Nous pourrons toujours le configurer à partir du bouton d’authentification unique de l’[application web](https://toutapp.com/login).

Une fois que nous disposerons de ces informations, nous travaillerons avec notre équipe d’ingénieurs pour configurer cet abonnement.
