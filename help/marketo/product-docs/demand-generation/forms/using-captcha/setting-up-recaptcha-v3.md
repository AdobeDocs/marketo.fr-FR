---
description: Configuration de reCAPTCHA v3 - Documents Marketo - Documentation du produit
title: Configuration de reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# Configuration de reCAPTCHA v3 {#setting-up-recaptcha-v3}

ReCAPTCHA v3 est une expérience sans frictions qui évalue les envois de formulaire en fonction de leur degré de méfiance sans utiliser de défis de texte, d’image ou de bouton. [En savoir plus](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}.

## Récupération de votre Data Center et de votre Munchkin ID {#retrieve-your-data-center-and-munchkin-id}

Pour l’étape 6 de la section Configuration initiale de reCAPTCHA v3 ci-dessous, vous aurez besoin du centre de données et de l’identifiant Munchkin de votre abonnement Marketo Engage. Voici comment les trouver.

1. Dans Marketo, cliquez sur **Admin**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Cliquez sur **Mon compte**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Faites défiler l’écran jusqu’à Informations sur l’assistance.

   ![](assets/setting-up-recaptcha-v3-3.png)

## Configuration initiale de reCAPTCHA v3 {#initial-recaptcha-v3-setup}

Les étapes suivantes sont effectuées en dehors de Marketo.

1. Accédez à [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"} et cliquez sur Admin Console v3.

1. Connectez-vous/inscrivez-vous à un compte Google.

1. Cliquez sur le bouton Créer (+) pour créer une nouvelle clé.

1. Créez un libellé pour identifier la clé à utiliser pour Marketo Engage.

1. Choisissez le type **reCAPTCHA v3**. Marketo Engage ne prend actuellement pas en charge reCAPTCHA v2.

1. Ajoutez chaque domaine utilisé par l’abonnement au Marketo Engage. Les domaines non définis ici renverront des erreurs sur les formulaires où reCAPTCHA est activé. N’oubliez pas de remplacer les mots &quot;datacenter&quot; et &quot;munchkinID&quot; par les [données de votre abonnement](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * tout domaine de landing page et alias paramétré dans l&#39;abonnement

   >[!NOTE]
   >
   >Par exemple, si le centre de données de votre compte est &quot;jst&quot;, le domaine que vous placez sur la liste autorisée serait `app-sjst.marketo.com`. Si votre Munchkin ID est 123-ABC-789, le domaine que vous placeriez sur la liste autorisée sera `123-ABC-789.mktoweb.com`.

1. Définissez un propriétaire et une adresse électronique supplémentaire qui doit recevoir des alertes sur ce service.

1. Acceptez les conditions d’utilisation de reCAPTCHA.

1. Cliquez sur **Submit**.

   >[!NOTE]
   >
   >Conservez la clé du site et la clé secrète à portée de main pour la configuration du Marketo Engage.

## Configuration de CAPTCHA en Marketo Engage {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>Après avoir suivi ces étapes et [activé CAPTCHA dans votre premier formulaire Marketo](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}, veillez à tester le formulaire immédiatement, car toute erreur de configuration dans la configuration reCAPTCHA peut endommager le formulaire.

1. Dans Marketo, cliquez sur **Admin**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Sélectionnez **CAPTCHA** dans l’arborescence.

   ![](assets/setting-up-recaptcha-v3-5.png)

1. Cliquez sur **Modifier** dans les paramètres CAPTCHA.

   ![](assets/setting-up-recaptcha-v3-6.png)

1. Cliquez sur la liste déroulante CAPTCHA et sélectionnez reCAPTCHA v3.

   ![](assets/setting-up-recaptcha-v3-7.png)

1. Insérez la clé secrète et la clé du site. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[Activer CAPTCHA dans Marketo Forms](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
