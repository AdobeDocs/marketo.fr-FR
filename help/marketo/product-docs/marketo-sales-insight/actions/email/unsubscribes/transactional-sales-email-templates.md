---
description: Modèles de courrier électronique de vente transactionnelle - Documents Marketo - Documentation du produit
title: Modèles d’e-mail de vente transactionnelle
hide: true
hidefromtoc: true
feature: Sales Insight Actions
source-git-commit: f11e455196cdfb7a6c1054df40344cab5b06772b
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Modèles d’e-mail de vente transactionnelle {#transactional-sales-email-templates}

Si votre équipe envoie des emails transactionnels ou non commerciaux, vous pouvez marquer un modèle d’email comme non commercial afin qu’il puisse contourner les désabonnements.

## Informations à noter {#things-to-note}

* Les emails non commerciaux contourneront les désabonnements aux ventes et [Vérification du désabonnement du Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* Les messages de désabonnement ne sont pas automatiquement ajoutés aux emails non commerciaux, même si la variable [ajout du paramètre d’administration des messages de désabonnement](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}`[dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} renseignera toujours le message de désabonnement de votre équipe.

## Configuration d’un modèle de courrier électronique à des fins non commerciales {#configure-an-email-template-for-non-commercial-use}

Accédez à la section Modèle .

Recherchez le modèle que vous souhaitez mettre à jour.

Sélectionnez le modèle.

Activez le bouton d’activation/désactivation d’email non commercial sous Paramètres du modèle.

Envoyer un email non commercial

Lorsqu’une personne désabonnée est sélectionnée, elle est mise en surbrillance orange.

Dans la fenêtre de composition, sélectionnez le modèle non commercial que vous souhaitez afficher.

Une bannière indique aux utilisateurs qu’ils ont sélectionné un modèle d’email non commercial.

Cliquez sur Envoyer et l&#39;email sera toujours envoyé même si la personne est désinscrite.
