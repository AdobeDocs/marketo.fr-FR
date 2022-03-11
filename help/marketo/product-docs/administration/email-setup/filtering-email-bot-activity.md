---
description: Filtrage de l’activité des robots de messagerie électronique - Documents Marketo - Documentation du produit
title: Filtrage de l’activité des robots de messagerie
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: a64c499f6972e94adfecbe164d86f7db1b1447aa
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Filtrage de l’activité des robots de messagerie {#filtering-email-bot-activity}

Parfois, l’activité de robots de messagerie peut gonfler par erreur les ouvertures de votre email et les données de clics. Voici comment réparer ça.

>[!NOTE]
>
>En utilisant la variable [Liste internationale des robots et araignées IAB/ABC](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/), toutes les activités d’ouverture/de clic avec une adresse IP ou un agent utilisateur correspondant à n’importe quel élément de cette liste seront identifiées comme une activité de robot et ne seront pas connectées à Marketo.

1. Cliquez sur **Administration**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Cliquez sur **Email**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Cliquez sur le bouton **Activité des robots** .

   ![](assets/filtering-email-bot-activity-3.png)

1. Cliquez sur le curseur pour activer **Filtrage de l’activité des robots**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Vous pouvez choisir séparément si l’activité des robots doit être enregistrée ou non. Si vous choisissez de ne pas le faire, il se peut qu’une baisse des ouvertures et des clics d’email soit observée lorsque les faux nombres sont filtrés.

**ÉTAPE FACULTATIVE**: Pour désactiver la fonction, désélectionnez simplement le curseur. Si vous désactivez cette option, les données &quot;Activité des robots dans les 90 derniers jours&quot; s’affichent comme suit : **not** réinitialiser.

>[!TIP]
>
>Tirez parti des données d’activité de robots dans les listes dynamiques par l’intermédiaire de la valeur booléenne &quot;Is Bot Activity&quot; (oui/non) ou dans les contraintes de filtre/déclenchement applicables.
