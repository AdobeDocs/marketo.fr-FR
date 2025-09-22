---
unique-page-id: 10096409
description: Éviter D’Envoyer Du Contenu En Double - Documents Marketo - Documentation Du Produit
title: Éviter d’envoyer du contenu en double
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
feature: Engagement Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 7%

---

# Éviter d’envoyer du contenu en double {#avoid-sending-duplicate-content}

Avez-vous déjà reçu le même e-mail deux fois ? Ennuyeux, n&#39;est-ce pas ?

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
