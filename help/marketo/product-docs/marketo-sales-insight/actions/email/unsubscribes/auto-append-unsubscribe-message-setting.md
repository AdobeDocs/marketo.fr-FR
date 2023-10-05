---
description: Ajout automatique du paramètre de message de désabonnement - Documents Marketo - Documentation du produit
title: Ajout automatique du paramètre de message de désabonnement
feature: Sales Insight Actions
exl-id: 17734f62-74e6-4168-a9c8-7835e3daf5ff
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Ajout automatique du paramètre de message de désabonnement {#auto-append-unsubscribe-message-setting}

Assurez-vous que chaque e-mail d’actions Sales Insight envoyé comprend un message de désabonnement afin que les destinataires puissent facilement se désabonner de la communication. Lorsque l’ajout du message de désabonnement est activé, toutes les communications que votre équipe envoie à partir des ventes Marketo comprennent un message de désabonnement, y compris les courriers électroniques envoyés à partir de l’application web et de Salesforce.

>[!NOTE]
>
>Si vous utilisez la variable `{{team_unsubscribe}}` champ dynamique dans un modèle d’email et que le paramètre d’ajout de message de désabonnement est activé, le champ dynamique de désabonnement de l’équipe renseignera votre message de désabonnement. _au lieu de_ ajout de votre message de désabonnement.

## Activer/Désactiver Désabonner Ajouter {#enable-disable-unsubscribe-append}

1. Cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. Sous Paramètres d’administration, cliquez sur **Désabonne**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Dans l’onglet Messagerie, sous Ajouter un message de désabonnement, déplacez le curseur à l’état souhaité.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Si vous désactivez le paramètre d’ajout de message de désabonnement, il est recommandé d’ajouter un pied de page de désabonnement à vos modèles afin de vous assurer que votre communication dispose d’une option d’exclusion. Vous pouvez le faire en ajoutant votre propre message personnalisé à chaque modèle ou en utilisant la variable `{{team_unsubscribe}}` [champ dynamique](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}.
