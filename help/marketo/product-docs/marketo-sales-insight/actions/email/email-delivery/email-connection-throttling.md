---
description: Limitation de la connexion par e-mail - Documents Marketo - Documentation du produit
title: Limitation de la connexion aux e-mails
exl-id: 02450a1e-5b30-4057-b204-19fab1a7d6c9
feature: Sales Insight Actions
source-git-commit: 19f60f58ae4de26536b304eb8ae9677ecc221993
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Limitation de la connexion aux e-mails {#email-connection-throttling}

L’intégration de votre compte Sales Connect pour l’envoi par les fournisseurs de messagerie Exchange ou Gmail offre une configuration simplifiée et optimise la délivrabilité des emails pour la communication des ventes 1:1. Cependant, pour préserver la santé des systèmes et la sécurité des comptes, Gmail et Exchange appliquent les limites d’envoi des emails. Ces limites peuvent être augmentées ou diminuées à la discrétion des fournisseurs.

## Limitation de la connexion aux e-mails (Beta) {#email-connection-throttling-beta}

Le contrôle de connexion par e-mail permet aux administrateurs de Sales Connect de configurer le taux d’envoi des e-mails lors de l’utilisation de Gmail ou Exchange comme canal de diffusion, de sorte que le taux auquel les e-mails sont remis au fournisseur de canal de diffusion ne dépasse pas les limites appliquées.

Lorsque les limites sont régulièrement dépassées, cela peut parfois être considéré comme un comportement suspect de la part du fournisseur de canal de diffusion, ce qui entraîne l’échec des emails et parfois même la désactivation d’un compte.

**Remarques/points forts**

* Activé automatiquement lorsqu’un utilisateur se connecte à Gmail ou à Exchange
* Peut être personnalisé si vous souhaitez augmenter ou diminuer les paramètres des recommandations en fonction de vos besoins.
* Ralentit uniquement les emails envoyés par Gmail ou par Exchange, ne ralentit pas pour le canal de diffusion personnalisé
* Le ralentissement de la connexion par e-mail place chaque utilisateur dans des files d’attente distinctes, car chaque utilisateur a sa propre connexion avec son fournisseur de messagerie.

**Configuration des paramètres de limitation de la connexion par e-mail**

1. Cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/email-connection-throttling-1.png)

1. Sous Paramètres d’administration, cliquez sur **Général**.

   ![](assets/email-connection-throttling-2.png)

1. Dans la carte de limitation de la connexion par e-mail à droite, cliquez sur le bouton **Activer le ralentissement des emails** curseur.

   ![](assets/email-connection-throttling-3.png)

1. Dans la carte Limitation de la connexion par e-mail à droite, saisissez la taille de lot souhaitée des e-mails qui seront envoyés au fournisseur de canal de messagerie.

   ![](assets/email-connection-throttling-4.png)

1. Définissez la durée d’attente avant l’envoi de chaque lot. Dans cet exemple, nous choisissons 25 emails toutes les 45 secondes.

   ![](assets/email-connection-throttling-5.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/email-connection-throttling-6.png)

Une fois les modifications enregistrées, tous les utilisateurs verront leurs emails envoyés par lots à leur compte Gmail ou Exchange connecté pour diffusion.

## Limites des fournisseurs de messagerie {#email-provider-limits}

**Outlook 365**

Entreprise/entreprise

* 10 000 par jour
* 30 par minute
* 500 destinataires par email

Informations supplémentaires [peut être consulté ici](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 2 000 par jour (500 pour les comptes d’essai et marqués)
* 2 emails par seconde (limite API)
* 2 000 destinataires par message (maximum 500 pour les destinataires externes)

Informations supplémentaires [peut être consulté ici](https://support.google.com/a/answer/166852?hl=en).

**Serveur Microsoft Exchange (2010, 2013)**

Les limites sont définies par le service informatique de l’organisation, car le serveur est hébergé par l’organisation. Pour plus d’informations, contactez l’administrateur réseau ou système.

>[!MORELIKETHIS]
>
>* [Présentation du canal de diffusion](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Connexion par e-mail pour les utilisateurs de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connexion par e-mail pour les utilisateurs Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
