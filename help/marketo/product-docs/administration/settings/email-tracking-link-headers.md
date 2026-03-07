---
description: Comment personnaliser les en-têtes des liens de suivi des e-mails dans Admin sous E-mail, y compris Strict-Transport-Security pour HTTPS, avec les conseils de révision informatique.
title: En-têtes de lien de suivi des e-mails
exl-id: 2db1f1b3-3afe-4710-a8b1-b06fbf09ec8c
feature: Administration
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 9%

---

# En-têtes de lien de suivi des e-mails {#email-tracking-link-headers}

Suivez les étapes ci-dessous pour personnaliser les en-têtes de lien de suivi des e-mails.

1. Dans Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/email-tracking-link-headers-1.png)

1. Cliquez sur **[!UICONTROL E-mail]**.

   ![](assets/email-tracking-link-headers-2.png)

1. Faites défiler jusqu’aux options d’en-tête personnalisé. Choisissez les paramètres souhaités et cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   ![](assets/email-tracking-link-headers-3.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>Utilisez cette option pour garantir que les liens de tracking seront toujours diffusés via HTTPS (ne doit être défini que pour les abonnements disposant de liens de tracking sécurisés par SSL).</td>
 </tr>
</table>

>[!CAUTION]
>
>Il est important de passer en revue ces paramètres avec votre équipe informatique afin de déterminer la politique de votre entreprise à définir. Des paramètres incorrects peuvent empêcher certains visiteurs d’accéder à vos liens d’e-mail.
