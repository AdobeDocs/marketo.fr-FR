---
unique-page-id: 10094576
description: Désabonnement durable - Documents Marketo - Documentation du produit
title: Désabonnement durable
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Désabonnement durable {#durable-unsubscribe}

Marketo a amélioré le comportement de la fonctionnalité de désabonnement pour la rendre « durable ». Nous avons ajouté un statut d’e-mail principal, qui est distinct de l’indicateur de désabonnement visible sur l’enregistrement des détails de la personne.

Si l’indicateur de désabonnement est défini de false à true, le statut de l’e-mail principal est mis à jour et la modification est propagée à d’autres personnes ayant la même adresse e-mail. Si une personne est supprimée et recréée, ou si un nouvel enregistrement est créé avec la même adresse e-mail, l’indicateur de désabonnement n’est **pas** remplacé.

>[!NOTE]
>
>Le désabonnement durable fonctionne sur toutes les partitions de l’ensemble de votre base de données Marketo.

## Remplacez l’indicateur de désabonnement de True par False (par exemple, Réabonner une personne). {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Il existe plusieurs façons de se réabonner.

Dans Salesforce, effacez le champ Désinscription par e-mail de l’enregistrement du prospect/contact. Cette opération va être synchronisée avec Marketo.

![Écran Salesforce](assets/durable-unsubscribe-1.png)

Dans Marketo, désélectionnez la zone Désabonné dans l’onglet Infos de l’enregistrement de la personne.

![Effacement de la zone de désabonnement dans un enregistrement de personne](assets/durable-unsubscribe-2.png)

Exécutez une étape de flux _Modifier la valeur des données_ comme illustré ci-dessous pour une ou plusieurs personnes.

![Étape de flux Modifier la valeur de données](assets/durable-unsubscribe-3.png)

## Création d’une personne {#creating-a-new-person}

Lorsqu’une nouvelle personne est créée, Marketo la compare au tableau principal de statut des e-mails. Si la personne a déjà été désabonnée, nous mettrons à jour l’enregistrement pour qu’elle soit désabonnée.

## Modification d’une adresse e-mail {#changing-an-email-address}

Si vous remplacez l’adresse e-mail d’une personne par une adresse e-mail de désabonnement, cette personne sera désabonnée. Cette modification peut se produire dans Marketo ou [!DNL Salesforce].

## Réabonnement {#re-subscribing}

De même qu’un désabonnement entraînerait le désabonnement de toutes les personnes ayant la même adresse e-mail, un réabonnement réabonnerait en fait chaque personne ayant la même adresse e-mail.

>[!MORELIKETHIS]
>
>[Comprendre le désabonnement](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
