---
unique-page-id: 1147356
description: Présentation de la journalisation des événements de courrier électronique - Documents Marketo - Documentation du produit
title: Présentation de la journalisation des événements de courrier électronique
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 3%

---

# Présentation de la journalisation des événements de courrier électronique {#understanding-email-event-logging}

Lors de l’envoi d’emails, Marketo consigne différents points de données dans les journaux d’activité de la personne. Voici les plus basiques.

| Événement | Description |
|---|---|
| Envoyé | Est consigné chaque fois qu’un courrier électronique est envoyé à partir des serveurs Marketo, qu’il soit réellement diffusé. Les messages rejetés sont toujours consignés comme &quot;Envoyé&quot;. |
| Diffusé | Est consigné chaque fois qu’un email est accepté par le serveur de messagerie du destinataire. Cela ne signifie pas qu’il évite les filtres anti-spam. Il ne peut y avoir qu&#39;une seule diffusion pour chaque email envoyé. |
| Renvoi définitif | Certains hard bounces sont le résultat de blocs de spam, donc nous n&#39;essaierons pas de lui envoyer un email pendant 24 heures dans aucune campagne. D&#39;autres hard bounces comme les boîtes de réception inexistantes sont permanents, et nous ne remettrons plus jamais la personne par courrier électronique de toute campagne. |
| Renvoi temporaire | Est consigné lorsqu’une réponse du serveur n’est pas claire, que la boîte de messagerie est pleine ou que des problèmes généraux du serveur surviennent. Nous mettons ces personnes dans une logique de reprise pendant 24 à 36 heures pour une diffusion future potentielle. Cela n’exclut pas la personne des autres envois. |
| Ouvert | Est consigné lorsqu’un destinataire consulte un email avec des images NON bloquées. Un seul événement d’ouverture par email, par personne et par campagne dynamique est consigné. S’ils ouvrent deux fois le même email à partir de leur boîte de réception, il ne sera pas consigné plus d’une fois. |
| Cliqué | Est consigné chaque fois qu’une URL décorée de l’email est chargée dans le navigateur (le résultat d’un clic sur le lien). En règle générale, il s&#39;agit du clic du destinataire, mais il peut également s&#39;agir d&#39;un couper/coller. |
| Désabonné | Est consigné lorsqu’une personne clique sur le lien de désabonnement d’un courrier électronique et envoie le formulaire de désabonnement. |

>[!CAUTION]
>
>Si le même email est envoyé à la même personne deux fois à partir de la même campagne, l&#39;événement **Ouvert** sera consigné un maximum d&#39;une fois.
