---
unique-page-id: 14352405
description: Configuration de l’authentification unique via SAML 2.0 dans Sales Connect - Marketo Docs - Documentation du produit
title: Configuration de l’authentification unique via SAML 2.0 dans Sales Connect
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Configuration de l’authentification unique via SAML 2.0 dans Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Nous prenons en charge l’authentification unique par le biais de la spécification SAML 2.0. Cependant, nous n&#39;avons actuellement aucune intégration directe avec aucun fournisseur. Nous devrons collecter des informations auprès de votre fournisseur d’authentification unique pour obtenir cette configuration.

>[!NOTE]
>
>Cela s’applique uniquement aux utilisateurs de **Marketo Sales Connect**. Si vous ne disposez pas de Sales Connect mais que vous souhaitez en savoir plus, contactez l’équipe Compte d’Adobe (votre gestionnaire de compte).

## Exigences {#requirements}

* compte SSO
* abonnement à la connexion Marketo Sales
* Metadata.xml du compte SSO (URL du problème, point de terminaison pour la validation et clé publique)

## Configuration {#setup}

Le fichier metadata.xml de l’instance SSO de votre équipe doit contenir l’URL de l’émetteur, le point de terminaison pour la validation et une clé publique.

L’emplacement d’authentification unique est également nécessaire pour que le compte d’authentification unique de votre entreprise soit un domaine unique. Par exemple, nous avons besoin d’un sous-domaine unique tel que `toutapp.pingidentity.com` ou similaire. Sans ce type d’identifiant unique, nous ne pourrons pas configurer SAML à partir du tableau de bord.

Les identifiants de connexion unique et Okta ne fournissent pas toujours des identifiants uniques lors de l’attribution d’une URL. Si vous utilisez Okta ou One Login, cela signifie que nous ne pourrons pas configurer une connexion à partir du bouton du tableau de bord. Nous pourrons toujours le configurer à partir du bouton Connexion unique sur l’ [application web](https://toutapp.com/login).

Une fois que nous aurons ces informations, nous travaillerons avec notre équipe d’ingénieurs pour les configurer pour votre abonnement.
