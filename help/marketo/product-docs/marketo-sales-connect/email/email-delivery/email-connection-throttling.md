---
description: Limitation de la connexion par courriel - Documents marketing - Documentation du produit
title: Limitation de la connexion au courriel
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---


# Limitation de la connexion par courriel {#email-connection-throttling}

L&#39;intégration de votre compte Sales Connect pour envoyer par l&#39;intermédiaire des fournisseurs de messagerie Exchange ou Gmail simplifie la configuration et optimise la délivrabilité du courrier électronique pour la communication 1:1 sur les ventes. Cependant, pour préserver la santé des systèmes et la sécurité des comptes, Gmail et Exchange appliquent des limites d&#39;envoi de courriers électroniques. Ces limites peuvent être augmentées ou diminuées à la discrétion des fournisseurs.

## Limitation de la connexion par courriel (bêta) {#email-connection-throttling-beta}

>[!AVAILABILITY]
>
>Cette fonctionnalité est actuellement dans la version bêta. Pour rejoindre cette version bêta, contactez votre responsable de succès client.

Le contrôle de connexion par courriel permet aux administrateurs de Sales Connect de configurer le taux d&#39;envoi des courriers électroniques lors de l&#39;utilisation de Gmail ou d&#39;Exchange comme canal de diffusion, de sorte que le taux auquel les courriers électroniques sont transmis au fournisseur de canal de diffusion ne dépasse pas les limites imposées.

Lorsque les limites sont régulièrement dépassées, cela peut parfois être considéré comme un comportement suspect de la part du fournisseur de canaux de diffusion, ce qui provoque l&#39;échec des courriels et parfois même la désactivation d&#39;un compte.

**Remarques/Points saillants**

* Activé automatiquement une fois qu&#39;un utilisateur se connecte à Gmail ou Exchange
* Peut être personnalisé si vous souhaitez augmenter ou diminuer les paramètres de la recommandation en fonction de vos besoins
* Limite uniquement les e-mails envoyés par Gmail ou Exchange, ne ralentit pas pour le canal de diffusion personnalisé
* Le ralentissement de la connexion par courriel met en file d&#39;attente chaque utilisateur individuellement pour qu&#39;il envoie des courriers électroniques séparément, chaque utilisateur ayant sa propre connexion avec son fournisseur de messagerie.

**Configuration des paramètres de limitation de la connexion par courriel**

1. Cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/email-connection-throttling-1.png)

1. Cliquez sur **Général**.

   ![](assets/email-connection-throttling-2.png)

1. Dans la carte de limitation de la connexion par courriel, entrez la taille de lot souhaitée des courriers électroniques qui seront envoyés au fournisseur de canal de messagerie.

   ![](assets/email-connection-throttling-3.png)

1. Définissez la durée d’attente avant l’envoi de chaque lot. Dans cet exemple, nous choisissons 25 courriels toutes les 45 secondes.

   ![](assets/email-connection-throttling-4.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/email-connection-throttling-5.png)

Une fois les modifications enregistrées, tous les utilisateurs verront leurs courriels envoyés par lots à leur compte Gmail ou Exchange connecté pour diffusion.

## Limites du fournisseur de messagerie {#email-provider-limits}

**Outlook 365**

Entreprise/Entreprise

* 10 000 par jour
* 30 par minute
* 500 destinataires par courriel

Vous trouverez plus d&#39;informations [ici](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 2 000 par jour (500 pour les comptes d&#39;essai et les comptes marqués)
* 2 courriers électroniques par seconde (limite d’API)
* 2 000 destinataires par message (maximum 500 pour les destinataires externes)

Vous trouverez plus d&#39;informations [ici](https://support.google.com/a/answer/166852?hl=en).

**Microsoft Exchange Server (2010, 2013)**

Les limites sont définies par le service informatique de l’entreprise lorsque le serveur est hébergé par l’entreprise. Contactez l’administrateur réseau ou système, le cas échéant, pour obtenir des informations supplémentaires.

>[!MORELIKETHIS]
>
>* [Présentation du Canal de diffusion](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Connexion par courriel pour les utilisateurs de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connexion par courriel pour les utilisateurs d&#39;Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

