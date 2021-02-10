---
unique-page-id: 14352405
description: Configuration de l'authentification unique via SAML 2.0 dans Sales Connect - Marketo Docs - Documentation sur les produits
title: Configuration de l'authentification unique via SAML 2.0 dans Sales Connect
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Configuration de l&#39;authentification unique via SAML 2.0 dans Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Nous prenons en charge l’authentification unique par le biais de la spécification SAML 2.0. Cependant, nous n&#39;avons actuellement aucune intégration directe avec aucun fournisseur. Pour obtenir cette configuration, nous devrons recueillir des informations auprès de votre fournisseur d’authentification unique.

>[!NOTE]
>
>Ceci s&#39;applique uniquement aux clients **Marketing Sales Connect**. Si vous ne disposez pas de Sales Connect mais souhaitez en savoir plus, contactez votre responsable de succès client.

## Exigences {#requirements}

* compte SSO
* Abonnement de connexion commerciale
* Metadata.xml du compte SSO (URL de publication, point de terminaison pour la validation et clé publique)

## Configuration {#setup}

Le fichier metadata.xml de l’instance SSO de votre équipe doit contenir l’URL de l’émetteur, le point de terminaison de la validation et une clé publique.

Nous aurons également besoin de l’emplacement d’authentification unique pour que votre compte d’authentification unique de société soit un domaine unique. Par exemple, nous avons besoin d’un sous-domaine unique tel que `toutapp.pingidentity.com` ou similaire. Sans ce type d&#39;identifiant unique, nous ne pourrons pas configurer SAML à partir du tableau de bord.

One Login et Okta ne fournissent pas toujours des identifiants uniques lors de l’attribution d’une URL. Si vous utilisez Okta ou One Login, cela signifie que nous ne pourrons pas configurer une connexion à partir du bouton tableau de bord. Nous serons toujours en mesure de le configurer à partir du bouton Connexion unique sur l&#39;application [Web ](http://toutapp.com/login).

Une fois que nous aurons ces informations, nous travaillerons avec notre équipe d&#39;ingénieurs pour les mettre en place pour votre abonnement.
