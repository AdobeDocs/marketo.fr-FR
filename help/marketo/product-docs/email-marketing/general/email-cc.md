---
unique-page-id: 17727995
description: Email CC - Documents Marketo - Documentation du produit
title: Envoyer CC par courrier électronique
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Envoyer CC par courrier électronique {#email-cc}

La fonctionnalité E-mail CC permet l’envoi d’e-mails spécifiés via Marketo pour inclure les destinataires en copie.

Cette fonctionnalité est disponible sur toutes les ressources de messagerie Marketo, quelle que soit la manière dont l’e-mail est envoyé (campagne par lots ou déclenchée). Le destinataire CC recevra une copie exacte de l’e-mail envoyé à la personne Marketo choisie. Ainsi, toute activité d’engagement (ouvertures, clics, etc.) sera consignée dans le journal d’activité de la personne Marketo dans la ligne « À » de l’e-mail. Cependant, l’activité de diffusion (envoyée, diffusée, hard bounce, etc.) _autre que le « soft bounce »_ ne s’enregistrera **pas**, car Marketo n’est pas en mesure de distinguer les événements de diffusion pour la personne Marketo des destinataires en copie (CC). Marketo ne peut mettre en cache que 100 000 personnes à la fois. Si votre liste dynamique dépasse les 100 000 et qu&#39;il est impératif que chaque personne y soit mise en copie conforme, nous vous recommandons de diviser votre liste.

>[!NOTE]
>
>La fonctionnalité E-mail CC n’a pas été conçue pour être utilisée avec les tests A/B. Vous pouvez l’utiliser quand même si vous le souhaitez. Toutefois, étant donné qu’il n’est pas pris en charge techniquement, l’assistance Marketo ne pourra pas vous aider à résoudre les problèmes.

## Configurer le CC d’e-mail {#set-up-email-cc}

1. Dans Mon Marketo, cliquez sur **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Dans l’arborescence, sélectionnez **[!UICONTROL E-mail]**.

   ![](assets/two.png)

1. Cliquez sur **[!UICONTROL Modifier les paramètres CC de l’e-mail]**.

   ![](assets/three.png)

1. Sélectionnez jusqu’à 25 champs Lead ou Entreprise Marketo (de type « E-mail ») à rendre disponibles pour une utilisation comme adresses CC dans les e-mails. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/four.png)

## Utilisation de la fonctionnalité E-mail Cc {#using-email-cc}

1. Sélectionnez votre e-mail et cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/five.png)

1. Cliquez sur **[!UICONTROL Paramètres de messagerie]**.

   ![](assets/six.png)

1. Sélectionnez les champs à utiliser pour mettre en copie les personnes. _Il existe une limite de cinq par e-mail_. Dans cet exemple, nous ne voulons que le CC de Propriétaire du lead. Cliquez sur **Enregistrer** lorsque vous avez terminé.

   ![](assets/seven.png)

   C&#39;est aussi simple que ça ! Dans l’exemple ci-dessus, lorsque vous envoyez l’e-mail, le prospect propriétaire des destinataires que vous avez choisis est CC&#39;d.

   >[!NOTE]
   >
   >Si une adresse e-mail non valide se trouve dans un champ CC, elle sera ignorée.

   Pour une identification rapide, la vue Résumé des e-mails vous indique si/quels champs de copie d’e-mail ont été sélectionnés.

   ![](assets/eight.png)

   Si l’e-mail est approuvé, mais que l’administrateur Marketo désactive un ou plusieurs champs CC avant l’envoi de l’e-mail, **ces personnes ne recevront pas d’e-mail**. Dans ce scénario, la vue Résumé de l’e-mail grisera tous les champs qui ont été désactivés après approbation, mais qui ont été pré-envoyés :

   ![](assets/removal.png)

   >[!NOTE]
   >
   >L’erreur ci-dessus s’affiche également dans la section Paramètres de messagerie du brouillon d’e-mail.

## Après l’envoi {#after-the-send}

* Si un destinataire CC clique sur un lien suivi dans l’e-mail, l’activité de clic (comme toutes les autres activités d’engagement) sera associée au destinataire principal de l’e-mail. De plus, ils peuvent cliquer sur une page contenant le code de suivi web Marketo (munchkin.js), ce qui entraîne leur cookie en tant que destinataire principal.

>[!TIP]
>
>Vous avez la possibilité de [désactiver tout ou partie des liens de tracking](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) dans un email.

* Une fois la campagne par e-mail exécutée, l’activité Envoyer un e-mail inclut une liste de toutes les adresses CC qui ont été incluses pour chaque destinataire du publipostage. Si des adresses CC ont été ignorées en raison du désabonnement, cela sera également noté dans l’activité.
* Les liens de désabonnement et les pages fonctionnent normalement dans les e-mails en copie (CC). Cela permet aux destinataires en copie (CC) de se désabonner correctement s&#39;ils le souhaitent (en respectant les réglementations anti-spam), et un enregistrement de cette action sera stocké dans la base de données Marketo.
* Les personnes répertoriées comme désabonnées dans votre base de données Marketo ne recevront **pas** d’e-mails via CC.
