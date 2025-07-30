---
solution: Marketo Engage
product: marketo
title: Rapport de spam
description: Découvrez comment utiliser SpamAssassin pour tester le contenu de votre e-mail et évaluer la probabilité qu'il soit marqué comme indésirable.
level: Beginner, Intermediate
feature: Email Designer
exl-id: 6954850e-2b1a-4bf5-b918-1c54d6926b7e
source-git-commit: aba42b7480c6e042c462c423615ad35a5f66212f
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 8%

---

# Rapport de spam {#email-spam-report}

En utilisant SpamAssassin dans Marketo Engage, vous pouvez tester le contenu de votre email et voir la probabilité que les FAI/fournisseurs de messagerie le marquent comme spam.

SpamAssassin analyse votre contenu et attribue un score en fonction de différents critères. Plus la valeur est faible, mieux c’est. Il est important de maintenir un score faible, car l&#39;envoi d&#39;e-mails avec un score élevé peut avoir un impact négatif sur votre délivrabilité globale.

## Accès au rapport de spam {#access-the-spam-report}

1. Dans votre e-mail, cliquez sur **Simuler du contenu**.

   ![](assets/email-spam-report-1.png){width="600" zoomable="yes"}

   >[!NOTE]
   >
   >Si vous n’avez pas encore ajouté de profil de test, vous devrez le faire juste après l’étape 1.

1. Cliquez sur le bouton **Rapport sur les spams**.

   ![](assets/email-spam-report-2.png)

1. Un rapport de spam est généré.

   ![](assets/email-spam-report-3.png){width="600" zoomable="yes"}

1. Vérifiez les scores et les descriptions de chaque élément.

   >[!IMPORTANT]
   >
   >Si le score global est supérieur à 5, votre e-mail peut être bloqué par le destinataire ou marqué comme indésirable à la diffusion.

1. Si vous estimez que le score est trop élevé, modifiez le contenu du Designer d&#39;e-mail en fonction des résultats du rapport, puis réexécutez le rapport **Rapport sur les spams**.

   ![](assets/email-spam-report-4.png){width="800" zoomable="yes"}

Lorsque le score est à votre goût, il est prêt à être envoyé.

![](assets/email-spam-report-5.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Le score de spam est dérivé via SpamAssassin et **les règles ne sont pas la propriété d&#39;Adobe**. Vous trouverez plus d’informations sur ces règles dans la [documentation de SpamAssassin](https://spamassassin.apache.org/#_blank){target="_blank"}. Liste complète des erreurs [voir ici](https://spamassassin.apache.org/old/tests_3_0_x.html){target="_blank"}.
