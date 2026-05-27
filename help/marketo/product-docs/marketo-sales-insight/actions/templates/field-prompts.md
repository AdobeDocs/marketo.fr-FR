---
description: Découvrez les invites de champ dans les modèles d’e-mail. Ajoutez des espaces réservés qui invitent l’expéditeur à renseigner du contenu personnalisé lors de l’envoi.
title: Prompts de champs
exl-id: c138b627-f853-4d35-b022-cc517d6b86d4
TQID: https://experienceleague.adobe.com/ahVbX8SGxaVUjSPsU-1uVc36ecIW60lwYXxDZSxC0kU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 2%

---

# Prompts de champs {#field-prompts}

Les invites de champ vous permettent d&#39;ajouter une chaîne de texte aux e-mails qui doivent être supprimés ou remplacés avant l&#39;envoi de l&#39;e-mail. Il s’agit d’un excellent moyen de rappeler aux utilisateurs d’ajouter une personnalisation supplémentaire.

Pour ajouter une invite de champ, saisissez le texte souhaité. Faites-la précéder d&#39;un point d&#39;exclamation et entourez-la de crochets (voir ci-dessous).

**Exemples :**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

<p>Les utilisateurs devront remplacer ce texte par leur propre personnalisation avant que l’e-mail ne puisse être envoyé.

![](assets/field-prompts-1.png)

>[!NOTE]
>
>Lors de l’utilisation d’invites avec des campagnes de vente, il est préférable de les utiliser avec des étapes d’email manuelles. Ces étapes attribuent à l’utilisateur une tâche de rappel pour envoyer l’e-mail, ce qui lui permet de remplacer les invites par du texte personnalisé. Les étapes d’envoi automatique par e-mail dans les campagnes de ventes tenteront d’envoyer automatiquement , sans permettre à l’utilisateur de remplacer les invites. Les invites qui ne sont pas remplacées entraînent l&#39;échec de l&#39;envoi des emails.
