---
description: Ajout automatique du paramètre de message de désabonnement - Documents Marketo - Documentation du produit
title: Ajout automatique du paramètre de message de désabonnement
feature: Marketo Sales Connect
exl-id: 8aa75123-f6b5-4dfe-8fa7-f764620c04e8
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Ajout automatique du paramètre de message de désabonnement {#auto-append-unsubscribe-message-setting}

Assurez-vous que chaque email envoyé comprend un message de désabonnement afin que les destinataires puissent facilement se désabonner de la communication. Lorsque l’ajout du message de désabonnement est activé, toutes les communications que votre équipe envoie à partir des ventes Marketo comprennent un message de désabonnement, y compris les emails envoyés à partir de l’application web, Salesforce, du module externe Gmail et du module externe Outlook.

## Informations à noter {#things-to-note}

* Pour les emails envoyés à partir des modules externes, le désabonnement n’est annexé qu’à l’utilisation d’un modèle.

* Si vous utilisez le champ dynamique `{{team_unsubscribe}}` dans un modèle de courrier électronique et que le paramètre d’ajout de message de désabonnement est activé, le champ dynamique de désabonnement de l’équipe renseignera votre message de désabonnement _au lieu d’ajouter_ à votre message de désabonnement.

## Activer/Désactiver Désabonner Ajouter {#enable-disable-unsubscribe-append}

1. Cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. Sous Paramètres Admin, Cliquez Sur **Se Désabonner**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Dans l’onglet Messagerie, sous Ajouter un message de désabonnement, déplacez le curseur à l’état souhaité.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Si vous désactivez le paramètre d’ajout de message de désabonnement, il est recommandé d’ajouter un pied de page de désabonnement à vos modèles afin de vous assurer que votre communication dispose d’une option d’exclusion. Pour ce faire, ajoutez votre propre message personnalisé à chaque modèle ou utilisez le `{{team_unsubscribe}}` [champ dynamique](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}.
