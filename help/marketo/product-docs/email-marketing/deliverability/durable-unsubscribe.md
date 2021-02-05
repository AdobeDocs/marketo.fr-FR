---
unique-page-id: 10094576
description: Désabonnement durable - Documents marketing - Documentation du produit
title: Désabonnement durable
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---


# Désabonnement durable {#durable-unsubscribe}

Marketo a amélioré le comportement de la fonctionnalité de désabonnement pour la rendre &quot;durable&quot;. Nous avons ajouté un état de courriel principal, qui est distinct de l&#39;indicateur de désabonnement visible sur l&#39;enregistrement des détails de la personne.

Si l’indicateur de désabonnement est défini sur false pour true, l’état du courrier électronique principal est mis à jour et la modification est propagée à d’autres personnes ayant la même adresse électronique. Si une personne est supprimée et recréée, ou si un nouvel enregistrement est créé avec la même adresse électronique, l’indicateur de désabonnement sera **non** remplacé.

>[!NOTE]
>
>La désinscription durable fonctionne sur toutes les partitions de votre base de données Marketo.

## Mettre à jour l&#39;indicateur Désabonner de True vers False (par exemple, Réabonner une personne) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Il existe plusieurs façons de s&#39;abonner à nouveau à une personne.

Dans Salesforce, **effacez** le champ Opt-out de courriel de l&#39;enregistrement du prospect/contact. Cette opération sera synchronisée avec Marketo.

![](assets/one.png)

Dans Marketo, **effacez** la zone désabonnée dans l&#39;onglet Infos de l&#39;enregistrement de la personne.

![](assets/two.png)

Exécutez une étape de flux **Modifier la valeur des données** comme illustré ci-dessous pour une ou plusieurs personnes.

![](assets/three.png)

Mettez à jour une personne existante via l’API SOAP.

## Création d&#39;une personne {#creating-a-new-person}

Lorsqu’une nouvelle personne est créée, Marketo la vérifie par rapport à la table d’état du courrier électronique principal. Si la personne a déjà été désabonnée, nous mettrons à jour l&#39;enregistrement à désabonner.

## Modification de l&#39;adresse électronique {#changing-an-email-address}

Si vous changez l’adresse électronique d’une personne en adresse électronique désabonnée, cette personne sera désabonnée. Cette modification peut se produire dans Marketing ou dans Salesforce.

Si vous changez une adresse de messagerie désabonnée en adresse de messagerie abonnée, cette personne devient abonnée.

## Réabonnement {#re-subscribing}

Tout comme un désabonnement provoquait le désabonnement de toutes les personnes ayant la même adresse électronique, un réabonnement reprenait en fait chaque personne ayant la même adresse électronique.

## Journal des Activités {#activity-log}

Les définitions des modifications de valeur de données pour _updateLeadEmailStatus_ et _resetLeadEmailStatus_ se trouvent dans [cet article de la communauté](http://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[Comprendre la désinscription](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
