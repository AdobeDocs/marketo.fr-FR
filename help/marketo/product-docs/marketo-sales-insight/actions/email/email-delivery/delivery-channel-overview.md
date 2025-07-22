---
description: Présentation Du Canal De Diffusion - Documents Marketo - Documentation Du Produit
title: Présentation Du Canal De Diffusion
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Présentation Du Canal De Diffusion {#delivery-channel-overview}

Le service commercial de Marketo vous offre plusieurs options pour diffuser des e-mails. Cet article passe en revue les canaux de diffusion que vous pouvez utiliser, comment les sélectionner et quand les sélectionner les uns par rapport aux autres.

## Recommandé : Gmail ou Exchange via une connexion par e-mail {#recommended-gmail-or-exchange-via-email-connection}

Le service de vente par e-mail de Marketo permet une configuration rationalisée et une délivrabilité améliorée. La connexion par e-mail permet à chaque utilisateur de se connecter à son compte [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) ou [[!DNL Exchange]](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) à Marketo Sales pour être utilisé comme canal de diffusion de choix pour tous les e-mails de vente Marketo.

L’utilisation de Gmail ou [!DNL Exchange] s’accompagne d’avantages distincts par rapport aux autres options de canal de diffusion :

* Il s’agit d’un canal de diffusion éprouvé, avec une réputation bien établie, qui contribue à maintenir une délivrabilité élevée.
* Les méthodes d’authentification telles que SPF et DKIM sont déjà configurées et gérées par votre équipe informatique. Il n’y a donc pas de configuration supplémentaire.
* L’envoi d’e-mails sur un réseau de messagerie donné (c’est-à-dire l’envoi d’un e-mail en tant qu’utilisateur [!DNL Exchange] à une société qui reçoit des e-mails par l’intermédiaire de [!DNL Exchange]) peut contribuer à améliorer la délivrabilité.

Il est important de noter que ces canaux de diffusion ont leurs propres limites d’envoi qui sont appliquées par Microsoft et Google. Pour lutter contre ce problème, nous utilisons un mécanisme de limitation pour aider les utilisateurs à respecter ces limites. Pour en savoir plus sur le [limitation des e-mails](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md), cliquez ici.

>[!NOTE]
>
>Par défaut, le plug-in O365 utilisera toujours votre canal de diffusion Exchange et le plug-in Gmail utilisera toujours votre canal de diffusion Gmail pour diffuser des e-mails à partir des plug-ins.

**Suivi des rebonds** : le service des ventes Marketo peut détecter les rebonds pour les utilisateurs d’Exchange Online ou de Gmail en détectant le message de rebond envoyé à la boîte de réception de l’expéditeur. Ces notifications de rebond seront cumulées dans les notifications de modèles d’analyse, de campagnes d’analyse et de flux en direct pour les utilisateurs. Le suivi des rebonds n’est pas pris en charge pour les clients Exchange On-Prem.

## Canal de diffusion personnalisé via SMTP {#custom-delivery-channel-via-smtp}

Le service commercial Marketo offre la possibilité supplémentaire de connecter un serveur SMTP tiers à utiliser comme canal de diffusion préféré de votre équipe commerciale.

L’utilisation d’un fournisseur SMTP tiers est une excellente option pour les équipes de vente pour lesquelles le volume d’e-mails est la priorité numéro un. Les fournisseurs SMTP tels que Sendgrid et Sparkpost sont optimisés pour répondre aux besoins de la diffusion d&#39;emails en masse et peuvent s&#39;adapter pour répondre aux besoins de ceux qui cherchent à déployer de grands volumes d&#39;emails.

En outre, les fournisseurs SMTP tiers offrent une pléthore de fonctionnalités pour aider à répondre aux besoins de délivrabilité de votre équipe (tels que les rapports de diffusion par e-mail et les adresses IP dédiées), ce qui en fait une option idéale pour ceux qui recherchent des contrôles plus granulaires et une meilleure visibilité autour de leur canal de diffusion par e-mail de vente.

## Serveurs de ventes Marketo (hérités) {#marketo-sales-servers-legacy}

Les serveurs de vente Marketo ne sont disponibles que pour certains clients ToutApp hérités. Ces clients verront les serveurs de vente Marketo disponibles dans leurs paramètres d’e-mail. Tous les clients non hérités ne verront pas l’option Ventes Marketo comme une option et doivent connecter leur compte Gmail ou [!DNL Outlook] au service Ventes Marketo pour déverrouiller un canal de diffusion.

Les serveurs de vente Marketo ne prennent pas en charge les méthodes d’authentification DKIM et SPF, ce qui peut réduire le taux de délivrabilité. C’est pourquoi nous recommandons à tous les clients de se connecter à Gmail ou [!DNL Outlook] pour une délivrabilité optimale.

## Serveurs MSC (hérités) {#msc-servers-legacy}

Les serveurs MSC ne sont disponibles que pour certains clients ToutApp hérités. Ces clients verront les serveurs MSC disponibles dans leurs paramètres de messagerie. Tous les clients non hérités ne verront pas MSC comme une option et doivent connecter leur compte Gmail ou Outlook à Sales Connect pour déverrouiller un canal de diffusion.

Les serveurs MSC ne prennent pas en charge les méthodes d’authentification DKIM et SPF, ce qui peut réduire le taux de délivrabilité. C’est pourquoi nous recommandons à tous les clients de se connecter à Gmail ou [!DNL Outlook] pour une délivrabilité optimale.

## Serveurs Marketo {#marketo-servers}

Les serveurs de messagerie Marketo ne s’intègrent pas au service commercial Marketo. Les serveurs Marketo sont optimisés pour la diffusion en masse afin de pouvoir s’adapter aux besoins des marketeurs. Cependant, Gmail et [!DNL Exchange] ont un taux de réussite plus élevé pour la communication commerciale 1:1, c’est pourquoi nous vous recommandons d’utiliser ces serveurs pour votre communication commerciale.

>[!MORELIKETHIS]
>
>* [Connexion par e-mail pour les utilisateurs Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connexion e-mail pour [!DNL Outlook] utilisateurs](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configuration d’un canal de diffusion personnalisé](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Limitation de la connexion aux e-mails](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
