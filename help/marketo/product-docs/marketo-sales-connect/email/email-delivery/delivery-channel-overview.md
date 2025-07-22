---
unique-page-id: 14352407
description: Présentation Du Canal De Diffusion - Documents Marketo - Documentation Du Produit
title: Présentation Du Canal De Diffusion
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Présentation Du Canal De Diffusion {#delivery-channel-overview}

Marketo [!DNL Sales Connect] offre plusieurs options pour diffuser des e-mails. Cet article passe en revue les canaux de diffusion que vous pouvez utiliser, comment les sélectionner et quand les sélectionner les uns par rapport aux autres.

## Recommandé : Gmail ou [!DNL Exchange] via la connexion par e-mail {#recommended-gmail-or-exchange-via-email-connection}

[!DNL Sales Connect] permet une configuration rationalisée et une délivrabilité améliorée grâce à notre service de connexion par e-mail. La connexion [!UICONTROL E-mail] permet à chaque utilisateur de se connecter à son compte [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) ou [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) pour [!DNL Sales Connect] utiliser comme canal de diffusion de choix pour tous les e-mails [!DNL Sales Connect].

L’utilisation de Gmail ou [!DNL Exchange] s’accompagne d’avantages distincts par rapport aux autres options de canal de diffusion :

* Il s’agit d’un canal de diffusion éprouvé, avec une réputation bien établie, qui contribue à maintenir une délivrabilité élevée.
* Les méthodes d’authentification telles que SPF et DKIM sont déjà configurées et gérées par votre équipe informatique. Il n’y a donc pas de configuration supplémentaire.
* L’envoi d’e-mails sur un réseau de messagerie donné (c’est-à-dire l’envoi d’un e-mail en tant qu’utilisateur [!DNL Exchange] à une société qui reçoit des e-mails par l’intermédiaire de [!DNL Exchange]) peut contribuer à améliorer la délivrabilité.

Il est important de noter que ces canaux de diffusion ont leurs propres limites d’envoi qui sont appliquées par Microsoft et Google. Pour lutter contre ce problème, nous utilisons un mécanisme de limitation pour aider les utilisateurs à respecter ces limites. Pour en savoir plus sur le [limitation des e-mails](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md), cliquez ici.

>[!NOTE]
>
>Par défaut, le plug-in O365 utilisera toujours votre canal de diffusion Exchange et le plug-in Gmail utilisera toujours votre canal de diffusion Gmail pour diffuser des e-mails à partir des plug-ins.

**Suivi des bounces** : le MSC peut détecter les bounces pour les utilisateurs [!DNL Exchange Online] ou Gmail en détectant le message de bounce envoyé à la boîte de réception de l’expéditeur. Ces notifications de rebond seront cumulées dans les notifications de modèles d’analyse, de campagnes d’analyse et de flux en direct pour les utilisateurs. Le suivi des bounces n’est pas pris en charge pour les clients On-Prem [!DNL Exchange].

## Canal de diffusion personnalisé via SMTP {#custom-delivery-channel-via-smtp}

[!DNL Sales Connect] offre la possibilité supplémentaire de connecter un serveur SMTP tiers à utiliser comme canal de diffusion préféré de votre équipe commerciale.

L’utilisation d’un fournisseur SMTP tiers est une excellente option pour les équipes de vente pour lesquelles le volume d’e-mails est la priorité numéro un. Les fournisseurs SMTP tels que [!DNL Sendgrid] et [!DNL Sparkpost] sont optimisés pour répondre aux besoins de la diffusion d’e-mails en masse et peuvent s’adapter aux besoins de ceux qui cherchent à déployer de grands volumes d’e-mails.

En outre, les fournisseurs SMTP tiers offrent une pléthore de fonctionnalités pour aider à répondre aux besoins de délivrabilité de votre équipe (tels que les rapports de diffusion par e-mail et les adresses IP dédiées), ce qui en fait une option idéale pour ceux qui recherchent des contrôles plus granulaires et une meilleure visibilité autour de leur canal de diffusion par e-mail de vente.

## Serveurs MSC (hérités) {#msc-servers-legacy}

Les serveurs MSC ne sont disponibles que pour certains clients ToutApp hérités. Ces clients verront les serveurs MSC disponibles dans leurs paramètres de messagerie. Tous les clients non hérités ne verront pas MSC comme une option et doivent connecter leur compte Gmail ou [!DNL Outlook] à [!DNL Sales Connect] pour déverrouiller un canal de diffusion.

Les serveurs MSC ne prennent pas en charge les méthodes d’authentification DKIM et SPF, ce qui peut réduire le taux de délivrabilité. C’est pourquoi nous recommandons à tous les clients de se connecter à Gmail ou [!DNL Outlook] pour une délivrabilité optimale.

## Serveurs Marketo {#marketo-servers}

Les serveurs de messagerie Marketo ne s’intègrent pas à [!DNL Sales Connect]. Les serveurs Marketo sont optimisés pour la diffusion en masse afin de pouvoir s’adapter aux besoins des marketeurs. Cependant, Gmail et [!DNL Exchange] ont un taux de réussite plus élevé pour la communication commerciale 1:1, c’est pourquoi nous vous recommandons d’utiliser ces serveurs pour votre communication commerciale.

>[!MORELIKETHIS]
>
>* [Connexion par e-mail pour les utilisateurs Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connexion e-mail pour [!DNL Outlook] utilisateurs](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configuration d’un canal de diffusion personnalisé](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Limitation de la connexion aux e-mails](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
