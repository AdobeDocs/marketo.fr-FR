---
unique-page-id: 10099077
description: Découvrez comment importer une liste de contrôle dans votre instance Marketo Engage.
title: Power Pack sur la délivrabilité des e-mails - Comment importer une liste de contrôle
exl-id: a4782611-2556-43bf-802b-afeb332eafcd
feature: Deliverability
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Power Pack sur la délivrabilité des e-mails : Importer une liste de contrôle {#email-deliverability-power-pack-how-to-import-a-seed-list}

Une liste de contrôle est une liste de comptes de messagerie de plusieurs fournisseurs de messagerie, dont Google Apps, Hotmail, Yahoo !, etc., qui est utilisée pour estimer le taux de délivrabilité des boîtes de réception par rapport à celui des dossiers de spam. Vous trouverez ci-dessous les étapes à suivre pour intégrer cette liste à votre instance Marketo Engage.

>[!IMPORTANT]
>
>Cet article est destiné aux personnes disposant actuellement d&#39;un abonnement Everest actif. Si vous utilisez Inbox Tracker by Bird (anciennement MessageBird), vos tutoriels [sont disponibles ici](/help/marketo/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.md){target="_blank"}.

## Importer une liste de contrôle {#import-a-seed-list}

1. Dans Mon Marketo, sélectionnez **[!UICONTROL Outils de délivrabilité]**.

   ![](assets/email-deliverability-power-pack-1.png)

1. L’application [!DNL Everest] s’ouvre. Dans le volet de navigation de gauche, cliquez sur **[!UICONTROL En cours]** et sélectionnez **[!UICONTROL Emplacement de la boîte de réception]**.

   ![](assets/email-deliverability-power-pack-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Gérer la liste de contrôle]**.

   ![](assets/email-deliverability-power-pack-3.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Actions]** et sélectionnez **[!UICONTROL Télécharger : un par ligne]**.

   ![](assets/email-deliverability-power-pack-4.png)

   >[!NOTE]
   >
   >Utilisez l’optimisateur de liste de contrôle (en haut de la page) si vous [!DNL Everest] optimiser votre liste à votre place.

1. Après l’exportation, la liste s’affiche sous la forme d’un fichier .txt dans le dossier des téléchargements de votre navigateur. Récupérez-la et [importez-la](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) dans votre instance Marketo sous forme de liste statique.

   ![](assets/email-deliverability-power-pack-5.png)

   >[!TIP]
   >
   >Veillez à donner à votre liste un nom qui la rendra plus facile à trouver.

   >[!CAUTION]
   >
   >Vous obtenez un nombre limité de ces campagnes d’emplacement de boîte de réception par mois. Pour savoir combien vous en obtenez, consultez la section [!UICONTROL Abonnement] sous [!UICONTROL Paramètres du compte] > [!UICONTROL Abonnement] dans [!DNL Everest]. Pour en savoir plus, contactez votre représentant commercial Marketo.

## Acquisition de nouvelles listes de contrôle {#acquiring-new-seedlists}

Votre liste de contrôle peut changer aussi souvent que tous les mois. Il est important de vous connecter régulièrement au pack d’alimentation délivrabilité des e-mails et de vérifier le statut de votre liste de contrôle. Lorsque de nouvelles adresses sont ajoutées ou qu’une mise à jour est requise de votre côté, vous êtes averti(e) via l’icône de notification située dans le coin inférieur gauche de l’application.

Une fois votre liste statique dans Marketo créée, vous pouvez commencer à l’envoyer pour tester l’emplacement de votre boîte de réception d’e-mail.
