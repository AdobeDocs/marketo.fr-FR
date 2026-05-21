---
unique-page-id: 1147328
description: Découvrez les erreurs hard et soft, ainsi que la manière dont Marketo les classe. Utilisez les champs E-mail suspendu et E-mail non valide pour gérer les problèmes de diffusion.
title: Rebonds définitifs et temporaires dans les e-mails
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
TQID: https://experienceleague.adobe.com/qr4rAdOWWg5dazZVztnoTUv6WJQE8Xpm2WKttjQaOOg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 310
ht-degree: 14%

---

# Rebonds définitifs et temporaires dans les e-mails {#hard-and-soft-bounces-in-email}

Un rebond définitif peut rendre l’adresse e-mail d’une personne non valide lorsqu’un serveur de messagerie indique à Marketo que l’e-mail de la personne ne peut pas être remis. Un soft bounce signifie qu’un problème est survenu lors de la diffusion de l’e-mail à la personne. Ce problème est automatiquement résolu et peut parfois prendre des jours. Les rebonds définitifs et temporaires comprennent [plusieurs catégories](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classification des rebonds {#bounce-classification}

Marketo comporte 5 champs de personne liés à la diffusion d’e-mails avec des problèmes.

1. **E-mail suspendu** - Définissez cette valeur sur True lorsqu&#39;un certain type de hard bounce se produit.
1. **Cause de suspension de l’e-mail** - Il peut y avoir plusieurs raisons. Ce champ tente d’expliquer la cause.
1. **E-mail suspendu à** - Lorsque le rebond fautif se produit, Marketo suspend l’envoi de courrier à la personne pendant 24 heures à partir de cet horodatage.
1. **E-mail non valide** - Définissez cette valeur sur True lorsqu’un certain type de hard bounce se produit.
1. **Cause non valide des e-mails** - Raison du hard bounce.

>[!NOTE]
>
>Une fois qu’une personne a atteint le statut **e-mail suspendu**, il n’est pas possible de décocher la case e-mail suspendu . Cependant, la personne deviendra toujours postable 24 heures après la suspension initiale.
>
>Lorsqu’une personne est marquée comme **e-mail non valide**, elle ne peut être réinitialisée que manuellement (ce qui est recommandé uniquement si vous avez confirmé que l’adresse e-mail est valide) en décochant la case « E-mail non valide » dans l’onglet Informations sur la personne de son enregistrement.

>[!PREREQUISITES]
>
>Pour créer un rapport sur les performances des e-mails[&#128279;](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) qui générera des données de bounce procédez comme suit.

Après avoir créé votre rapport sur les performances des e-mails, l’écran doit ressembler à ceci :

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Les filtres anti-spam génèrent parfois des hard bounces. Ces « faux positifs » ne sont pas une indication de la véritable validité de l’adresse e-mail de la personne.
