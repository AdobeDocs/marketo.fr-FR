---
description: Filtrage de l’Activité des robots de messagerie électronique - Docs Marketo - Documentation du produit
title: Filtrage de l’Activité des robots de messagerie
source-git-commit: b491f476c4facc6343559a0acf5d5527e9afc618
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# Filtrage de l’Activité des robots de messagerie {#filtering-email-bot-activity}

Parfois, l’activité des robots de messagerie peut gonfler par erreur les ouvertures de vos courriels et les clics sur les données. Voici comment réparer ça.

>[!NOTE]
>
>En utilisant la [Liste internationale des moteurs de balayage et robots d&#39;ABC/IAB](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/), toutes les activités d&#39;ouverture/clic avec une adresse IP ou un agent utilisateur qui correspond à quelque chose de cette liste seront identifiées comme activité de robots et ne seront pas connectées dans Marketo.

1. Cliquez sur **Admin**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Cliquez sur **Courriel**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Cliquez sur l&#39;onglet **Activité du robot**.

   ![](assets/filtering-email-bot-activity-3.png)

1. Cochez la case **Activer le filtrage de l&#39;Activité des robots de messagerie**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Après avoir activé cette fonctionnalité, vous pouvez voir une baisse des ouvertures des courriels et des clics lorsque de faux nombres sont filtrés.

**ÉTAPE** FACULTATIVE : Pour désactiver la fonction, désélectionnez simplement la case à cocher. Si vous désactivez cette option, les données &quot;Activité de robots au cours des 90 derniers jours&quot; ne se réinitialisent **pas**.
