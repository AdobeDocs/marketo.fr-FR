---
description: Paramètre De Message De Désabonnement D’Ajout Automatique - Documents Marketo - Documentation Du Produit
title: Paramètre d’ajout automatique du message de désabonnement
feature: Marketo Sales Connect
exl-id: 8aa75123-f6b5-4dfe-8fa7-f764620c04e8
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 4%

---

# Paramètre d’ajout automatique du message de désabonnement {#auto-append-unsubscribe-message-setting}

Assurez-vous que chaque e-mail envoyé inclut un message de désabonnement afin que les destinataires aient une option facile pour se désabonner de la communication. Lorsque l’option Ajouter un message de désabonnement est activée, toutes les communications envoyées par votre équipe depuis les ventes Marketo incluent un message de désabonnement, y compris les e-mails envoyés depuis l’application web, Salesforce, le plug-in Gmail et le plug-in Outlook.

## Éléments à noter {#things-to-note}

* Pour les e-mails envoyés à partir des modules externes, le désabonnement n’est ajouté que lorsqu’un modèle est utilisé.

* Si vous utilisez le champ dynamique `{{team_unsubscribe}}` dans un modèle d’e-mail et que le paramètre d’ajout de message de désabonnement est activé, le champ dynamique de désabonnement de l’équipe renseigne votre message de désabonnement _au lieu_ d’ajouter votre message de désabonnement.

## Activer/Désactiver l’ajout du désabonnement {#enable-disable-unsubscribe-append}

1. Cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. Sous Paramètres D’Administration, Cliquez Sur **Désabonnements**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Dans l’onglet Messagerie , sous Ajouter un message de désabonnement , déplacez le curseur sur l’état souhaité.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Si vous désactivez le paramètre Ajouter un message de désabonnement , nous vous recommandons d’ajouter un pied de page de désabonnement à vos modèles pour vous assurer que votre communication dispose d’une option d’opt-out. Pour ce faire, ajoutez votre propre message personnalisé à chaque modèle ou utilisez le `{{team_unsubscribe}}` [champ dynamique](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}.
