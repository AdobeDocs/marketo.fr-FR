---
description: Présentation du canal de diffusion - Documents Marketo - Documentation du produit
title: Présentation du canal de diffusion
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Présentation du canal de diffusion {#delivery-channel-overview}

Marketo Sales vous offre plusieurs options pour diffuser des emails. Cet article passe en revue les canaux de diffusion que vous pouvez utiliser, comment les sélectionner et quand les choisir.

## Recommandé : Gmail ou Exchange via connexion par courriel {#recommended-gmail-or-exchange-via-email-connection}

Marketo Sales permet une configuration simplifiée et une délivrabilité améliorée grâce à notre service Email Connection. La connexion par e-mail permet à chaque utilisateur de se connecter à son compte [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) ou [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) sur les ventes Marketo afin d’être utilisé comme canal de diffusion de votre choix pour tous les e-mails de vente Marketo.

L&#39;utilisation de Gmail ou Exchange présente des avantages distincts par rapport aux autres options de canal de diffusion :

* Il s’agit d’un canal de diffusion éprouvé avec une réputation établie qui contribue à maintenir une délivrabilité élevée.
* Les méthodes d’authentification telles que SPF et DKIM sont déjà configurées et gérées par votre équipe informatique. Il n’y a donc pas de configuration supplémentaire.
* L’envoi d’emails au sein d’un réseau de messagerie donné (c’est-à-dire l’envoi d’un email en tant qu’utilisateur Exchange à une société qui reçoit des emails par Exchange) peut contribuer à améliorer la délivrabilité.

Il est important de noter que ces canaux de diffusion possèdent leurs propres limites d’envoi qui sont appliquées par Microsoft et Google. Pour combattre cela, nous utilisons un mécanisme de ralentissement pour aider les utilisateurs à rester dans ces limites. Pour en savoir plus sur le [ralentissement des emails ici](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Par défaut, le module externe O365 utilisera toujours votre canal de diffusion exchange et le module externe Gmail utilisera toujours votre canal de diffusion Gmail pour diffuser des emails à partir des modules externes.

**Suivi des rebonds** : les ventes Marketo peuvent détecter les rebonds pour les utilisateurs Exchange Online ou Gmail en détectant le message de rebonds envoyé dans la boîte de réception de l’expéditeur. Ces notifications de rebond seront cumulées aux notifications de modèle, d’analyse de campagne et de flux en direct pour les utilisateurs. Le suivi des rebonds n’est pas pris en charge pour les clients Exchange On-Prem.

## Canal de diffusion personnalisé via SMTP {#custom-delivery-channel-via-smtp}

Marketo Sales offre la possibilité supplémentaire de connecter un serveur SMTP tiers à utiliser comme canal de diffusion préféré de votre équipe commerciale.

L’utilisation d’un fournisseur SMTP tiers est une excellente option pour les équipes de vente dont le volume d’email est la priorité numéro un. Les fournisseurs SMTP tels que Sendgrid et Sparkpost sont optimisés pour répondre aux besoins de la diffusion d’emails en masse et peuvent être mis à l’échelle pour répondre aux besoins de ceux qui souhaitent déployer de gros volumes d’emails.

En outre, les fournisseurs SMTP tiers offrent une pléthore de fonctionnalités pour aider à répondre aux besoins de délivrabilité de votre équipe (tels que les rapports de diffusion email et les adresses IP dédiées), ce qui en fait une excellente option pour ceux qui recherchent des contrôles plus précis et une visibilité sur leur canal de diffusion email de vente.

## Serveurs de vente Marketo (hérités) {#marketo-sales-servers-legacy}

Les serveurs de vente Marketo ne sont disponibles que pour certains clients hérités de ToutApp. Ces clients verront les serveurs de vente Marketo disponibles dans leurs paramètres de messagerie. Tous les clients qui ne sont pas des clients hérités ne verront pas les ventes Marketo comme une option et doivent connecter leur compte Gmail ou Outlook aux ventes Marketo pour déverrouiller un canal de diffusion.

Les serveurs de vente Marketo ne prennent pas en charge les méthodes d’authentification DKIM et SPF, ce qui peut réduire le taux de délivrabilité. C’est pourquoi nous recommandons à tous les clients de se connecter à Gmail ou Outlook pour une meilleure délivrabilité.

## Serveurs MSC (hérités) {#msc-servers-legacy}

Les serveurs du SMC ne sont disponibles que pour certains clients hérités de ToutApp. Ces clients verront les serveurs MSC disponibles dans leurs paramètres de messagerie. Tous les clients non hérités ne verront pas le MSC comme une option et doivent connecter leur compte Gmail ou Outlook à Sales Connect pour déverrouiller un canal de diffusion.

Les serveurs du MSC ne prennent pas en charge les méthodes d&#39;authentification DKIM et SPF, ce qui peut réduire le taux de délivrabilité. C’est pourquoi nous recommandons à tous les clients de se connecter à Gmail ou Outlook pour une meilleure délivrabilité.

## Serveurs Marketo {#marketo-servers}

Les serveurs de messagerie Marketo ne s’intègrent pas aux ventes Marketo. Les serveurs Marketo sont optimisés pour la diffusion en masse afin de leur permettre de s’adapter aux besoins des marketeurs. Cependant, Gmail et Exchange ont un taux de succès plus élevé pour les communications de ventes 1:1, c’est pourquoi nous vous recommandons d’utiliser ces serveurs pour vos communications de vente.

>[!MORELIKETHIS]
>
>* [Connexion par e-mail pour les utilisateurs de Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connexion par e-mail pour les utilisateurs d’Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configuration d’un canal de diffusion personnalisé](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Limitation de la connexion par e-mail](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
