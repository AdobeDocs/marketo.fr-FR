---
unique-page-id: 14352407
description: Présentation du Canal de diffusion - Documentation du marketing - Documentation du produit
title: Présentation du Canal de diffusion
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---


# Présentation du Canal de diffusion {#delivery-channel-overview}

Marketing to Sales Connect vous offre plusieurs options pour diffuser des courriers électroniques. Cet article examine les canaux de diffusion que vous pouvez exploiter, comment les sélectionner et quand choisir l&#39;un par rapport à l&#39;autre.

## Recommandé : Gmail ou Exchange via la connexion par courriel {#recommended-gmail-or-exchange-via-email-connection}

Sales Connect permet une configuration simplifiée et une délivrabilité améliorée grâce à notre service Email Connection. La connexion par courriel permet à chaque utilisateur de se connecter à son [compte Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) ou [compte Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) à Sales Connect pour être utilisé comme canal de diffusion de choix pour tous les courriels de la connexion par courriel.

L&#39;utilisation de Gmail ou d&#39;Exchange présente certains avantages par rapport aux autres options de canal de diffusion :

* Il s&#39;agit d&#39;un canal de diffusion éprouvé et doté d&#39;une réputation établie qui contribue à maintenir la délivrabilité élevée.
* Les méthodes d&#39;authentification telles que SPF et DKIM sont déjà configurées et gérées par votre équipe informatique, il n&#39;y a donc pas de configuration supplémentaire.
* L&#39;envoi d&#39;e-mails au sein d&#39;un réseau de messagerie donné (c&#39;est-à-dire l&#39;envoi d&#39;un e-mail en tant qu&#39;utilisateur Exchange à une société qui reçoit des e-mails par le biais d&#39;Exchange) peut contribuer à accroître la délivrabilité.

Il est important de noter que ces canaux de diffusion ont leurs propres limites d&#39;envoi qui sont appliquées par Microsoft et Google. Pour lutter contre ce phénomène, nous utilisons un mécanisme de ralentissement pour aider les utilisateurs à rester dans ces limites. Pour en savoir plus sur la limitation des [adresses électroniques, cliquez ici](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Par défaut, le plug-in O365 utilisera toujours votre canal de diffusion d&#39;échange et le plug-in Gmail utilisera toujours votre canal de diffusion Gmail pour envoyer des courriers électroniques à partir des plug-ins.

**Suivi** des rebonds : Le MSC peut détecter les rebonds pour les utilisateurs d&#39;Exchange Online ou de Gmail en détectant le message de rebonds envoyé à la boîte de réception de l&#39;expéditeur. Ces notifications de rebonds seront cumulées dans les analyses des modèles, les analyses Campaign et les notifications de flux dynamiques pour les utilisateurs. Le suivi des rebonds n&#39;est pas pris en charge pour les clients Exchange On-Prem.

## Canal de Diffusion personnalisé via SMTP {#custom-delivery-channel-via-smtp}

Sales Connect offre l&#39;option supplémentaire de connexion d&#39;un serveur SMTP tiers à utiliser comme canal de diffusion préféré de votre équipe commerciale.

L&#39;utilisation d&#39;un fournisseur SMTP tiers est une option idéale pour les équipes de vente dont le volume de courrier électronique est la priorité numéro un. Les fournisseurs SMTP tels que Sendgrid et Sparkpost sont optimisés pour répondre aux besoins de la diffusion des e-mails en masse et peuvent être mis à l’échelle pour répondre aux besoins de ceux qui souhaitent déployer des volumes élevés de e-mails.

De plus, les fournisseurs SMTP tiers offre une multitude de fonctionnalités pour aider votre équipe à répondre à ses besoins en termes de délivrabilité (rapports de diffusion de messagerie électronique et adresses IP dédiées, par exemple), ce qui en fait une option idéale pour ceux qui recherchent des contrôles plus granulaires et une visibilité accrue sur leur canal de diffusion de courriel de vente.

## Serveurs MSC (hérités) {#msc-servers-legacy}

Les serveurs MSC ne sont disponibles que pour certains clients hérités de ToutApp. Ces clients verront les serveurs MSC disponibles dans leurs paramètres de messagerie. Tous les clients non hérités ne verront pas MSC comme une option et devraient connecter leur compte Gmail ou Outlook à Sales Connect pour déverrouiller un canal de diffusion.

Les serveurs MSC ne prennent pas en charge les méthodes d&#39;authentification DKIM et SPF, ce qui peut réduire le taux de délivrabilité. C&#39;est pourquoi nous recommandons que tous les clients se connectent à Gmail ou Outlook pour une meilleure délivrabilité.

## Serveurs de marketing {#marketo-servers}

Les serveurs de messagerie de marketing à marketing ne s&#39;intègrent pas à Sales Connect. Les serveurs marketing sont optimisés pour la diffusion en bloc afin de leur permettre de s’adapter aux besoins des spécialistes du marketing. Cependant, Gmail et Exchange ont un taux de réussite plus élevé pour la communication des ventes 1:1, c&#39;est pourquoi nous vous recommandons d&#39;utiliser ces serveurs pour votre communication des ventes.

>[!MORELIKETHIS]
>
>* [Connexion par courriel pour les utilisateurs de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connexion par courriel pour les utilisateurs d&#39;Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configuration d’un Canal de Diffusion personnalisé](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Limitation de la connexion au courriel](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

