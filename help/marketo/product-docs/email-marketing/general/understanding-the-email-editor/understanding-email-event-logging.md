---
unique-page-id: 1147356
description: Présentation de la journalisation des Événements électroniques - Documents marketing - Documentation du produit
title: Présentation de la journalisation des Événements électroniques
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# Présentation de la journalisation des Événements électroniques {#understanding-email-event-logging}

Lors de l’envoi de courriers électroniques, Marketo consigne différents points de données dans les journaux d’activité de la personne. Voici les fondamentaux.

| Événement | Description |
|---|---|
| Envoyé | Est consigné chaque fois qu’un courrier électronique est envoyé à partir des serveurs Marketo, qu’il soit effectivement diffusé ou non. Les courriels reportés sont toujours enregistrés comme &quot;Envoyé&quot;. |
| Livré | Est consigné chaque fois qu’un courrier électronique est accepté par le serveur de messagerie du destinataire. Cela ne signifie pas qu&#39;il évite les filtres de spam. Il ne peut y avoir qu&#39;une diffusion pour chaque courrier électronique envoyé. |
| Bruyant | Certains rebonds durs sont le résultat de blocs de spam, nous n&#39;essaierons donc pas de lui envoyer un courriel pendant 24 heures dans une campagne. D&#39;autres rebonds durs comme des inbox inexistantes sont permanents, et nous n&#39;enverrons plus jamais de courriels à la personne de toute campagne. |
| Rebond léger | Est consigné lorsqu&#39;une réponse du serveur n&#39;est pas claire, que la boîte aux lettres est pleine ou que le serveur présente des problèmes généraux. Nous faisons passer ces gens par une logique de nouvelle tentative pendant 24 à 36 heures pour une diffusion future potentielle. Cela n&#39;exclut pas la personne d&#39;autres envois. |
| Ouvert | Est consigné lorsqu’un destinataire vue un courrier électronique contenant des images NON bloquées. Un seul événement ouvert par courriel, par personne et par campagne dynamique est enregistré. S’ils ouvrent deux fois le même courrier électronique depuis leur boîte de réception, il ne sera pas enregistré plusieurs fois. |
| Clic | Est consigné chaque fois qu’une URL décorée du courrier électronique est chargée dans le navigateur (résultat d’un clic sur le lien). Il s’agit généralement du clic du destinataire, mais il peut également s’agir d’un copier-coller. |
| Non abonné | Est consigné lorsqu’une personne clique sur le lien de désabonnement d’un courrier électronique et envoie le formulaire de désabonnement. |

>[!CAUTION]
>
>Si le même courrier électronique est envoyé à la même personne deux fois à partir de la même campagne, le événement **ouvert** est enregistré une fois au maximum.

