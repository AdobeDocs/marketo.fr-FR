---
unique-page-id: 1147328
description: Erreurs hard et soft dans les e-mails - Documents Marketo - Documentation du produit
title: Rebonds définitifs et temporaires dans les e-mails
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 15%

---

# Rebonds définitifs et temporaires dans les e-mails {#hard-and-soft-bounces-in-email}

Un rebond définitif peut rendre l’adresse e-mail d’une personne non valide lorsqu’un serveur de messagerie indique à Marketo que l’e-mail de la personne ne peut pas être remis. Un soft bounce signifie qu’un problème est survenu lors de la diffusion de l’e-mail à la personne. Ce problème est automatiquement résolu et peut parfois prendre des jours. Les rebonds définitifs et temporaires comprennent [plusieurs catégories](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classification des rebonds {#bounce-classification}

Dans Marketo, 5 chaînes de personne sont liées à la diffusion d’e-mails en difficulté.

1. **E-mail suspendu** - Définissez cette valeur sur True lorsqu&#39;un certain type de hard bounce se produit.
1. **Cause de suspension de l’e-mail** - Il peut y avoir plusieurs raisons. Ce champ tente d’expliquer la cause.
1. **E-mail suspendu à** - Lorsque le rebond fautif se produit, Marketo suspend l’envoi de courrier à la personne pendant 24 heures à partir de cet horodatage.
1. **E-mail non valide** - Définissez cette valeur sur True lorsqu’un certain type de hard bounce se produit.
1. **Cause non valide des e-mails** - Raison du hard bounce.

>[!NOTE]
>
>Une fois qu’une personne a atteint le statut **e-mail suspendu**, il n’est pas possible de décocher la case e-mail suspendu . Cependant, la personne deviendra toujours postable 24 heures après la suspension initiale.
>
>Lorsqu’une personne est marquée comme **e-mail non valide**, elle ne peut être réinitialisée que manuellement (ce que nous vous recommandons de ne faire que si vous savez avec certitude que son e-mail est valide) en décochant la case « E-mail non valide » dans l’onglet Informations sur la personne de son enregistrement.

>[!PREREQUISITES]
>
>Pour créer un rapport sur les performances des e-mails[&#x200B; qui générera des données de bounce](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) procédez comme suit.

Après avoir créé votre rapport sur les performances des e-mails, l’écran doit ressembler à ceci :

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Les filtres anti-spam génèrent parfois des hard bounces. Ces « faux positifs » ne sont pas une indication de la véritable validité de l’adresse e-mail de la personne.
