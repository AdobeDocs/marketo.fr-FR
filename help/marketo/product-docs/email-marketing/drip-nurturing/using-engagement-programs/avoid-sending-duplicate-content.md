---
unique-page-id: 10096409
description: Évitez d’envoyer du contenu en double - Documents Marketo - Documentation du produit
title: Éviter d’envoyer du contenu en double
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 3%

---

# Éviter d’envoyer du contenu en double {#avoid-sending-duplicate-content}

Avez-vous déjà reçu deux fois le même email ? C&#39;est embêtant, n&#39;est-ce pas ?

Vous trouverez ci-dessous sept scénarios et résultats possibles à connaître pour éviter d’envoyer à une personne le même message deux fois avec des programmes d’engagement.

## Scénarios {#scenarios}

| L’email est envoyé à partir de | La personne est | Personne reçoit un email |
|---|---|---|
| Une campagne dans un programme distinct, autonome et par défaut | Pas membre du programme par défaut | Oui |
| Une campagne dans un programme distinct, autonome et par défaut | Un membre du programme par défaut | Non |
| Une campagne dans un programme par défaut qui est déclenché à partir d’un cast dans le programme **same** CEE | Un membre du programme par défaut | Non |
| Une campagne dans un programme par défaut qui est déclenché à partir d’un cast dans le programme **same** CEE | Pas membre du programme par défaut | Oui |
| Une campagne dans un programme par défaut qui est déclenché à partir d’un diffusion dans un programme **différent** CEE | Un membre du programme par défaut | Non |
| Une campagne dans un programme par défaut qui est déclenché à partir d’un diffusion dans un programme **différent** CEE | Pas membre du programme par défaut | Oui |
| Un programme CEE **différent** utilisant un flux dynamique | Un membre des deux programmes du CEE | Non |
