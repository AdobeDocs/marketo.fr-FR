---
unique-page-id: 14352600
description: Comment configurer votre serveur SMTP Outlook365 avec Sales Connect - Marketo Docs - Documentation sur le produit
title: Comment configurer votre serveur SMTP Outlook365 avec Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Comment configurer votre serveur SMTP Outlook365 avec Sales Connect {#how-to-set-up-your-outlook-smtp-server-with-sales-connect}

>[!NOTE]
>
>Si votre organisation utilise Outlook et que vous essayez de configurer un canal de diffusion de courriel avec Marketing Cloud Sales Connect, nous vous recommandons de vous connecter à votre serveur Exchange [à l&#39;aide de notre fonction](http://docs.marketo.com/x/Z4AOAQ)de connexion par courriel.

Pour configurer un serveur [SMTP](http://docs.marketo.com/x/zYTS) personnalisé comme autre canal de diffusion, ToutApp exige que vous utilisiez une forme d&#39;authentification à des fins de sécurité. Vous pouvez configurer n’importe quel serveur SMTP sur votre page [de configuration](http://toutapp.com/next#settings/email-servers/smtp/configure)SMTP. Pour configurer un serveur SMTP Office365, Microsoft recommande la configuration suivante :\
**Serveur** SMTP : smtp.office365.com\
**Port** du serveur : Port 587 - Sécurisé\
**Méthode** d&#39;authentification : Connexion (SSL/TLS)\
**Nom d&#39;utilisateur ou Connexion**: votre adresse électronique Office365\
**Mot de passe**: votre mot de passe de messagerie Office365\
**Votre domaine**: votre domaine de société

Si vous rencontrez toujours des problèmes lors de la configuration de votre serveur SMTP, faites appel à votre administrateur Exchange pour vous assurer que les informations d&#39;identification appropriées sont utilisées.

>[!NOTE]
>
>Lors de l&#39;envoi via votre SMTP Office365, Microsoft impose une limite de 10 000 destinataires `limit of 30 messages sent per minute`par jour et une limite de 10 000 par jour. De plus, `each member` de votre équipe qui souhaite envoyer des e-mails par l&#39;intermédiaire de son serveur SMTP Office365 devra configurer cette opération avec leur propre adresse électronique et mot de passe dans leurs paramètres de connexion commerciale. Cochez la case correspondant au paramètre &quot; `Make this deliverability channel to all my team members``" will not work` pour cette configuration, conformément aux stratégies de compte Microsoft Office365.

