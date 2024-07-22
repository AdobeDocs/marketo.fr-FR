---
unique-page-id: 1147328
description: Erreurs hard et soft dans les courriers électroniques - Documents Marketo - Documentation du produit
title: Erreurs hard et soft dans les courriers électroniques
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Erreurs hard et soft dans les courriers électroniques {#hard-and-soft-bounces-in-email}

Un hard bounce peut rendre l’adresse électronique d’une personne invalide lorsqu’un serveur de messagerie indique à Marketo que son adresse électronique ne peut pas être diffusée. Un soft bounce signifie qu’une erreur s’est produite lors de l’envoi de l’email à la personne. Ce problème est automatiquement résolu et peut parfois prendre des jours. Les erreurs hard et soft se composent de [plusieurs catégories](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classification rebond {#bounce-classification}

Il existe 5 chaînes de personnes dans Marketo liées à la diffusion d’emails en difficulté.

1. **Email Suspended** - Défini sur True lorsqu’un certain type de hard bounce se produit.
1. **Email Suspended Cause** - Il peut y avoir de nombreuses raisons. Ce champ tente d&#39;expliquer la cause.
1. **Email suspendu à** - Lorsque le rebond offensant se produit, Marketo suspendra l’envoi à la personne pendant 24 heures à compter de cet horodatage.
1. **Email Invalid** - Défini sur True lorsqu’un certain type de hard bounce se produit.
1. **Email Invalid Cause** - La raison du hard bounce.

>[!NOTE]
>
>Une fois qu’une personne a atteint l’état **email suspendu**, il n’est pas possible d’effacer la case à cocher Email suspendu. Cependant, la personne sera toujours en mesure de poster 24 heures après la suspension initiale.
>
>Lorsqu’une personne est marquée comme **email non valide**, elle ne peut être réinitialisée que manuellement (ce que nous vous recommandons de ne faire que si vous savez que son email est valide) en décochant la case &quot;Email non valide&quot; dans l’onglet Informations sur la personne de son enregistrement.

>[!PREREQUISITES]
>
>Suivez [ ces étapes](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) pour créer un rapport Performance des emails qui générera des données de rebond.

Après avoir créé votre rapport Performance de messagerie, votre écran doit ressembler à celui-ci :

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Les filtres anti-spam créent parfois des hard bounces. Ces &quot;faux positifs&quot; ne sont pas une indication de la vraie validité de l&#39;adresse email de la personne.
