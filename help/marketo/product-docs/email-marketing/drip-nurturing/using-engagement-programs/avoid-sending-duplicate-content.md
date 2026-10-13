---
unique-page-id: 10096409
description: Découvrez les scénarios qui empêchent ou autorisent les e-mails en double dans les programmes d’engagement. Utilisez les règles d'appartenance au programme et CEE pour éviter les répétitions.
title: Éviter d’envoyer du contenu en double
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
feature: Engagement Programs
TQID: 'https://experienceleague.adobe.com/vJ0HguG6ad182v-Jkf-0DF6zAosaJG5B-me3ghxnYIM'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: fc5011cf-5b46-40b1-a5de-d7f042f85633
    internal-label: Engagement programs
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 7%
---
# Éviter d’envoyer du contenu en double {#avoid-sending-duplicate-content}

Voici sept scénarios et résultats possibles à connaître pour éviter d’envoyer deux fois le même message à une personne à l’aide de programmes d’engagement.

## Scénarios {#scenarios}

| L’e-mail est envoyé depuis | La personne est | La personne reçoit un e-mail. |
|---|---|---|
| Une campagne dans un programme par défaut distinct et autonome | Pas membre du programme par défaut | Oui |
| Une campagne dans un programme par défaut distinct et autonome | Membre du programme par défaut | Non |
| Une campagne dans un programme par défaut qui est déclenchée à partir d’un cast dans le **même** programme CEE | Membre du programme par défaut | Non |
| Une campagne dans un programme par défaut qui est déclenchée à partir d’un cast dans le **même** programme CEE | Pas membre du programme par défaut | Oui |
| Une campagne dans un programme par défaut qui est déclenchée à partir d’un cast dans un **autre** programme CEE | Membre du programme par défaut | Non |
| Une campagne dans un programme par défaut qui est déclenchée à partir d’un cast dans un **autre** programme CEE | Pas membre du programme par défaut | Oui |
| Un programme CEE **différent** utilisant un flux intelligent | Un membre des deux programmes du CEE | Non |
