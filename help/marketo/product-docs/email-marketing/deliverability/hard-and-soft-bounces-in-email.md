---
unique-page-id: 1147328
description: Retours nets et doux dans le courrier électronique - Documents marketing - Documentation du produit
title: Retours nets et doux dans le courrier électronique
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Retours nets et doux dans le courrier électronique {#hard-and-soft-bounces-in-email}

Un retour forcé peut rendre l&#39;adresse électronique d&#39;une personne invalide lorsqu&#39;un serveur de messagerie indique à Marketo que le courrier électronique de la personne ne peut pas être livré. Un rebond en douceur signifie qu&#39;un problème s&#39;est produit lors de la remise du courriel à la personne ; cela se résout automatiquement et peut parfois prendre des jours. Les rebonds durs et doux se composent de [plusieurs catégories](http://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classification de rebond {#bounce-classification}

Il y a 5 chaînes de personnes dans Marketo qui sont liées à une diffusion de messagerie en problème.

1. **Courrier électronique suspendu** - Défini sur True lorsqu’un certain type de rebond dur se produit.
1. **Cause** suspendue du courriel - Il peut y avoir de nombreuses raisons. Ce champ tente d&#39;expliquer la cause.
1. **Courriel suspendu à **- Lorsque le rebond offensant se produit, Marketo suspendra l&#39;envoi à la personne pendant 24 heures à partir de cet horodatage.
1. **Adresse électronique non valide** - Défini sur True lorsqu&#39;un certain type de rebond dur se produit.
1. **Cause** non valide du courrier électronique - Raison du rebond brutal.

>[!NOTE]
>
>Une fois qu&#39;une personne atteint l&#39;état suspendu **du** courrier électronique, il n&#39;y a aucun moyen d&#39;effacer la case à cocher du courrier électronique suspendu. Toutefois, la personne sera toujours prête à être expédiée 24 heures après la suspension initiale.
>
>Lorsqu&#39;une personne est marquée comme non valide **de son** courrier électronique, elle ne peut être réinitialisée que manuellement (ce que nous vous recommandons de ne faire que si vous savez que son courrier électronique est valide) en décochant la case &quot;Adresse électronique non valide&quot; dans l&#39;onglet Informations sur la personne de son enregistrement.

>[!PREREQUISITES]
>
>Suivez [ces étapes](../../../product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) pour créer un rapport sur les performances des courriels, qui générera des données de rebond.

Après avoir créé votre rapport sur les performances des courriels, votre écran devrait ressembler à celui-ci : ![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Les filtres indésirables génèrent parfois des rebonds durs. Ces &quot;faux positifs&quot; ne sont pas une indication de la validité réelle de l&#39;adresse électronique de la personne.

