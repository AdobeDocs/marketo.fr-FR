---
description: Découvrez comment configurer la sécurité de Dynamic Chat avec des domaines bloqués ou autorisés. Limitez les domaines de messagerie que les agents voient et les sites qui peuvent utiliser votre script de conversation.
title: Paramètres de sécurité
feature: Dynamic Chat
exl-id: 68a53986-6f42-4aa2-86f6-0b2097f94963
TQID: https://experienceleague.adobe.com/7ans6J5WCXbTalK7ubMCrWBLWaJm3prPCoxsrCWEKtg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 88949407423d12a95bf39470e3c29835d934e2f6
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 3%

---

# Paramètres de sécurité {#security-settings}

Dans les paramètres de sécurité, vous avez la possibilité d’ajouter des domaines à une liste autorisée bloquée ou .

![](assets/security-settings-1.png)

>[!IMPORTANT]
>
>Le filtrage Bloquer et Autoriser le domaine de messagerie s’applique uniquement lorsqu’un visiteur saisit son adresse e-mail directement dans Dynamic Chat, dans le chatbot ou dans un flux de conversation. Elle ne s’applique pas aux adresses e-mail que Dynamic Chat reçoit des produits intégrés, tels que Marketo Engage. Pour plus d’informations, consultez le tableau ci-dessous.

| Scénario | Le filtrage s’applique-t-il ? |
|---|---|
| Le visiteur saisit directement son adresse e-mail dans le chatbot Dynamic Chat | Oui |
| Le visiteur saisit directement son adresse e-mail dans un flux de conversation Dynamic Chat | Oui |
| L’e-mail est pré-rempli à partir d’un envoi de formulaire Marketo (le flux conversationnel apparaît après le remplissage du formulaire) | Non |
| L’e-mail est transmis à Dynamic Chat à partir de tout autre système intégré | Non |

## Domaines d’e-mail bloqués {#blocked-email-domains}

Si vous ne souhaitez pas que vos agents interagissent avec des visiteurs disposant de domaines de messagerie (par exemple, un concurrent), ajoutez leur domaine de messagerie au place sur la liste bloquée de la .

1. Sélectionnez le curseur **Activer la validation** pour activer la liste bloquée. Saisissez jusqu’à 50 domaines et cliquez sur **Enregistrer**.

   ![](assets/security-settings-2.png)

## Domaines autorisés {#allowed-domains}

L’ajout de domaines autorisés garantit que des tiers ne peuvent pas extraire le code JavaScript de votre site et l’ajouter au leur.

1. Sélectionnez le curseur **Activer la validation** pour activer la liste autorisée. Saisissez les domaines autorisés et cliquez sur **Enregistrer**.

   ![](assets/security-settings-3.png)
