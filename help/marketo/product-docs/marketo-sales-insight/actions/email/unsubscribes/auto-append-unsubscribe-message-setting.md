---
description: Paramètre De Message De Désabonnement D’Ajout Automatique - Documents Marketo - Documentation Du Produit
title: Paramètre de message de désabonnement d’ajout automatique
feature: Sales Insight Actions
exl-id: 17734f62-74e6-4168-a9c8-7835e3daf5ff
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Paramètre de message de désabonnement d’ajout automatique {#auto-append-unsubscribe-message-setting}

Assurez-vous que chaque e-mail d’actions Sales Insight envoyé inclut un message de désabonnement afin que les destinataires aient une option facile pour se désabonner de la communication. Lorsque l’option Ajouter un message de désabonnement est activée, toutes les communications envoyées par votre équipe depuis les ventes Marketo incluent un message de désabonnement, y compris les e-mails envoyés depuis l’application web et Salesforce.

>[!NOTE]
>
>Si vous utilisez le champ dynamique `{{team_unsubscribe}}` dans un modèle d’e-mail et que le paramètre d’ajout de message de désabonnement est activé, le champ dynamique de désabonnement de l’équipe renseigne votre message de désabonnement _au lieu_ d’ajouter votre message de désabonnement.

## Activer/Désactiver l’ajout du désabonnement {#enable-disable-unsubscribe-append}

1. Cliquez sur l’icône d’engrenage et sélectionnez **Paramètres**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. Sous Paramètres D’Administration, Cliquez Sur **Désabonnements**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Dans l’onglet Messagerie , sous Ajouter un message de désabonnement , déplacez le curseur sur l’état souhaité.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Si vous désactivez le paramètre Ajouter un message de désabonnement , nous vous recommandons d’ajouter un pied de page de désabonnement à vos modèles pour vous assurer que votre communication dispose d’une option d’opt-out. Pour ce faire, ajoutez votre propre message personnalisé à chaque modèle ou utilisez le `{{team_unsubscribe}}` [champ dynamique](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}.
