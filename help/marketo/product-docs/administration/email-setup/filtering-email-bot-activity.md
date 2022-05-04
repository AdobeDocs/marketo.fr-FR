---
description: Filtrage de l’activité des robots de messagerie électronique - Documents Marketo - Documentation du produit
title: Filtrage de l’activité des robots de messagerie
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: 2ef4b0b2a541c8b6a67bd654fda45956601661bd
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Filtrage de l’activité des robots de messagerie {#filtering-email-bot-activity}

Parfois, l’activité de robots de messagerie peut gonfler par erreur les ouvertures de votre email et les données de clics. Suivez les étapes ci-dessous pour résoudre ce problème.

Nous utilisons trois méthodes distinctes pour confirmer l’activité des robots :

* Correspondance avec [Liste de robots Interactive Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target=&quot;_blank&quot;} : Les activités qui correspondent à tout élément de la liste UA/IP de l’IAB (Agent utilisateur/Adresse IP) seront marquées comme des robots.
* Correspondance avec les URL/adresses IP des liens masqués : Nous ajoutons un lien masqué à tous les emails et capturons les clics UA/IP qui en proviennent. Les activités qui correspondent à ces UA/IP seront marquées comme des robots.
* Correspondance avec le modèle de proximité : Lorsque plus de deux activités se produisent en même temps (en moins de deux secondes), elles sont identifiées comme des robots.

Par rapport aux clics sur les liens de courrier électronique et à l’activité d’ouverture de courrier électronique, les nouvelles attributs sont renseignés avec les valeurs ci-dessous :

* Les activités identifiées comme des robots auront &quot;Activité de robot&quot; comme &quot;True&quot; et &quot;Modèle d’activité de robot&quot; comme modèle/méthode identifié.
* Les activités identifiées comme n’étant pas des robots auront &quot;Activité des robots&quot; comme &quot;False&quot; et &quot;Modèle d’activité des robots&quot; comme &quot;N/A&quot;.
* Les activités qui se sont produites avant l’introduction de ces attributs auront &quot;Activité de robot&quot; comme &quot;&quot; (vide) et &quot;Modèle d’activité de robot&quot; comme &quot;&quot; (vide).

1. Cliquez sur **Administration**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Cliquez sur **Email**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Cliquez sur le bouton **Activité des robots** .

   ![](assets/filtering-email-bot-activity-3.png)

1. Cliquez sur le bouton **Activation de l’identification des activités de robots** curseur à activer.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Vous pouvez choisir séparément si l’activité des robots doit être enregistrée ou non. Si vous choisissez de ne pas le faire, il se peut qu’une baisse des ouvertures et des clics d’email soit observée lorsque les faux nombres sont filtrés.

**ÉTAPE FACULTATIVE**: Pour désactiver la fonction, désélectionnez simplement le curseur. Si vous la désactivez, les données **not** réinitialiser.

>[!TIP]
>
>Tirez parti des données d’activité de robots dans les listes dynamiques par l’intermédiaire de la valeur booléenne &quot;Is Bot Activity&quot; (yes/no) et &quot;Bot Activity Pattern&quot; des filtres &quot;Lien cliqué dans le courrier électronique&quot; et &quot;Open Email&quot;, ainsi que des déclencheurs &quot;Clicks Link in Email&quot; et &quot;Opens Email&quot;.
