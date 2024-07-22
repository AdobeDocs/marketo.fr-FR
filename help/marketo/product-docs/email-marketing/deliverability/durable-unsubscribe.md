---
unique-page-id: 10094576
description: Désabonnement durable - Documents Marketo - Documentation du produit
title: Désabonnement durable
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 35f5b33b01462b1cd00e29360daee465c7f18cf0
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Désabonnement durable {#durable-unsubscribe}

Marketo a amélioré le comportement de la fonctionnalité de désabonnement pour la rendre &quot;durable&quot;. Nous avons ajouté un état d’email principal, qui est distinct de l’indicateur de désabonnement visible dans l’enregistrement des détails de la personne.

Si l’indicateur unsubscribe est défini sur false sur true, l’état de l’email principal est mis à jour et la modification est propagée à d’autres personnes ayant la même adresse email. Si une personne est supprimée et recréée, ou si un nouvel enregistrement est créé avec la même adresse électronique, l’indicateur de désabonnement sera **not** remplacé.

>[!NOTE]
>
>Le désabonnement durable fonctionne sur toutes les partitions de votre base de données Marketo entière.

## Mettre à jour l’indicateur Se désabonner de True à False (par exemple, Se réabonner à une personne) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Il existe plusieurs façons de réinscrire une personne.

Dans Salesforce, **effacez** le champ Email Opt Out sur l&#39;enregistrement de l&#39;prospect/du contact. Cette opération se synchronise avec Marketo.

![](assets/one.png)

Dans Marketo, **effacez** la case désabonnée dans l’onglet Informations de l’enregistrement de la personne.

![](assets/two.png)

Exécutez une étape de flux **Modifier la valeur de données** comme illustré ci-dessous sur une ou plusieurs personnes.

![](assets/three.png)

Mettre à jour une personne existante via SOAP API.

## Création d’une personne {#creating-a-new-person}

Lorsqu’une nouvelle personne est créée, Marketo la vérifie par rapport au tableau d’état de l’email maître. Si la personne a déjà été désinscrite, nous mettrons à jour l&#39;enregistrement à désinscrire.

## Modification d’une adresse électronique {#changing-an-email-address}

Si vous remplacez l’adresse électronique d’une personne par une adresse électronique de désabonnement, cette personne sera désinscrite. Cette modification peut se produire dans Marketo ou dans Salesforce.

Si vous remplacez une adresse email désabonnée par une adresse qui est abonnée, cette personne deviendra abonnée.

## Réabonnement {#re-subscribing}

Tout comme un désabonnement provoquait la désinscription de toutes les personnes ayant la même adresse email, un réabonnement réabonnait en fait chaque personne ayant la même adresse email.

>[!MORELIKETHIS]
>
>[Comprendre le désabonnement](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
