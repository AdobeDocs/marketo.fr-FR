---
description: Configuration de reCAPTCHA v3 - Documents Marketo - Documentation du produit
title: Configuration de reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 24942664d613fa2851bad7a0dd3862027deacf37
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Configuration de reCAPTCHA v3 {#setting-up-recaptcha-v3}

Texte d’introduction

## Configuration initiale de reCAPTCHA v3 {#initial-recaptcha-v3-setup}

Texte : Description v3 : les étapes suivantes sont effectuées en dehors de Marketo Engage.

1. Accédez à [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;} et cliquez sur le Admin Console v3.

1. Connectez-vous/inscrivez-vous à un compte Google.

1. Cliquez sur le bouton Créer (+) pour créer une nouvelle clé.

1. Créez un libellé pour identifier la clé à utiliser pour Marketo Engage.

1. Choisir le type **reCAPTCHA v3**. Marketo Engage ne prend actuellement pas en charge reCAPTCHA v2.

1. Ajoutez chaque domaine utilisé par l’abonnement au Marketo Engage. Les domaines non définis ici renverront des erreurs sur les formulaires où reCAPTCHA est activé.

   * 123-ABC-456.mktoweb.com
   * app-pod.marketo.com
   * tout domaine de landing page et alias paramétré dans l&#39;abonnement

1. Définissez un propriétaire et une adresse électronique supplémentaire qui doit recevoir des alertes sur ce service.

1. Acceptez les conditions d’utilisation de reCAPTCHA.

1. Cliquez sur **Envoyer**.

>[!NOTE]
>
>Conservez la clé du site et la clé secrète à portée de main pour la configuration du Marketo Engage.

## Configuration de CAPTCHA en Marketo Engage {#setting-up-captcha-in-marketo-engage}

1. Dans Marketo, cliquez sur **Administration**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Sélectionner **CAPTCHA** dans l&#39;arbre.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Cliquez sur **Modifier** sur les paramètres CAPTCHA.

   ![](assets/setting-up-recaptcha-v3-3.png)

1. Cliquez sur la liste déroulante CAPTCHA et sélectionnez reCAPTCHA v3.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Insérez la clé secrète et la clé du site. Cliquez sur **Enregistrer** une fois terminé.

   ![](assets/setting-up-recaptcha-v3-5.png)
