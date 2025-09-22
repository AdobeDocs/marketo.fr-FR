---
unique-page-id: 1147356
description: Comprendre La Journalisation Des Événements Par E-Mail - Documents Marketo - Documentation Du Produit
title: Présentation de la journalisation des événements d’e-mail
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 3%

---

# Présentation de la journalisation des événements d’e-mail {#understanding-email-event-logging}

Lors de l’envoi d’e-mails, Marketo consigne différents points de données dans les journaux d’activité de la personne. Voici les éléments de base.

| Événement | Description |
|---|---|
| [!UICONTROL Envoyé] | est consignée chaque fois qu’un e-mail est envoyé à partir des serveurs Marketo, qu’il soit réellement diffusé ou non. Les e-mails rebonds sont toujours consignés comme « Envoyés ». |
| [!UICONTROL Délivrés] | Est consignée chaque fois qu’un e-mail est accepté par le serveur de messagerie du destinataire. Cela ne signifie pas qu&#39;il a évité les filtres de spam. Il ne peut y avoir qu’une seule diffusion pour chaque e-mail envoyé. |
| [!UICONTROL Hard bounce] | Certains hard bounces sont le résultat de blocs de spam. Nous n&#39;essaierons donc pas d&#39;envoyer un e-mail à cette personne pendant 24 heures dans n&#39;importe quelle campagne. D’autres erreurs hard, telles que des boîtes de réception inexistantes, sont permanentes et nous n’enverrons plus jamais d’e-mail à la personne depuis aucune campagne. |
| [!UICONTROL Soft Bounce] | Est consigné lorsqu&#39;une réponse du serveur n&#39;est pas claire, que la boîte de messagerie est pleine ou que des problèmes généraux surviennent sur le serveur. Nous soumettons ces personnes à une logique de reprise pendant 24 à 36 heures pour une éventuelle diffusion future. Cela ne disqualifie pas la personne pour d&#39;autres envois. |
| [!UICONTROL Ouvert] | Est consignée lorsqu’un destinataire consulte un e-mail dont les images NE SONT PAS bloquées. Un seul événement ouvert par e-mail, par personne et par campagne intelligente est consigné. S’ils ouvrent deux fois le même e-mail à partir de leur boîte de réception, il ne sera pas consigné plus d’une fois. |
| [!UICONTROL sur lequel l’utilisateur a cliqué] | est consignée chaque fois qu’une URL décorée de l’e-mail est chargée dans le navigateur (résultat d’un clic sur le lien) ; Généralement, il s’agit du clic du destinataire, mais il peut également s’agir d’un couper/coller. |
| [!UICONTROL Désabonné] | Est consignée lorsqu’une personne clique sur le lien de désabonnement d’un e-mail et envoie le formulaire de désabonnement. |

>[!CAUTION]
>
>Si le même e-mail est envoyé à la même personne deux fois à partir de la même campagne, l’événement **[!UICONTROL Ouvert]** est consigné une fois au maximum.
