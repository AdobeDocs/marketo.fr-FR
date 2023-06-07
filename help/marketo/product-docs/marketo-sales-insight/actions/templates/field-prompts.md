---
description: Instructions de champ - Documents Marketo - Documentation du produit
title: Invite de champ
source-git-commit: 466df1fbd561860152f9fea02edb6eab5670c90a
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Invite de champ {#field-prompts}

Les invites de champ vous permettent d’ajouter une chaîne de texte aux emails qui doivent être supprimés ou remplacés avant l’envoi de l’email. C’est un excellent moyen de rappeler aux utilisateurs d’ajouter une personnalisation supplémentaire.

Pour ajouter une invite de champ, saisissez le texte de votre choix. Préfacez-la avec un point d’exclamation et entourez-la de accolades (voir ci-dessous).

**Exemples:**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

Les utilisateurs devront remplacer ce texte par leur propre personnalisation avant que l&#39;email puisse être envoyé.

>[!NOTE]
>
>Lors de l’utilisation d’invites avec des campagnes de ventes, il est préférable de les utiliser avec des étapes d’email manuelles. Ces étapes assignent à un utilisateur une tâche de rappel pour envoyer l’email, ce qui lui donne la possibilité de remplacer les invites par du texte personnalisé. Les étapes automatiques de courrier électronique dans les campagnes de vente tenteront d’envoyer automatiquement, sans permettre à l’utilisateur de remplacer les invites. Les messages électroniques non remplacés échouent à leur envoi.
