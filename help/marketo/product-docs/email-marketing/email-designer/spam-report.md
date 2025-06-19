---
solution: Marketo Engage
product: marketo
title: Spam Assassin
description: TEXTE ENVOYÉ ICI
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: bfa1bc900c2adc263e634a81440b77bef2976d3b
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 7%

---

# Spam Assassin {#spam-assassin}

En utilisant SpamAssassin dans Marketo Engage, vous pouvez tester le contenu de votre email et voir la probabilité que les FAI/fournisseurs de messagerie le marquent comme spam.

SpamAssassin analyse votre contenu et attribue un score en fonction de différents critères. Plus la valeur est faible, mieux c’est. Il est important de maintenir un score faible, car l&#39;envoi d&#39;e-mails avec un score élevé peut avoir un impact négatif sur votre délivrabilité globale.

## Accès au rapport sur les spams {#access-the-spam-report}

1. Dans l’écran Simuler , cliquez sur le bouton **Rapport sur les spams**.

CAPTURE D’ÉCRAN

1. Un rapport de spam est généré.

CAPTURE D’ÉCRAN

1. Vérifiez les scores et les descriptions de chaque élément.

>[!IMPORTANT]
>
>Si le score global est supérieur à 5, votre e-mail peut être bloqué ou marqué comme indésirable à la diffusion.

1. Si vous estimez que le score est trop élevé, modifiez votre contenu dans le Designer d&#39;e-mail, puis réexécutez le rapport sur les spams jusqu&#39;à ce que le score soit celui que vous souhaitez.

CAPTURE D’ÉCRAN

>[!NOTE]
>
>Le score de spam est dérivé via SpamAssassin et les règles ne sont pas la propriété d&#39;Adobe. Vous trouverez plus d’informations sur ces règles dans la [documentation de SpamAssassin](https://spamassassin.apache.org/#_blank). Liste complète des erreurs [voir ici](https://spamassassin.apache.org/old/tests_3_0_x.html?utm_source=chatgpt.com).
