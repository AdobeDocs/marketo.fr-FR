---
description: Filtrage de l’activité des robots de messagerie électronique - Documents Marketo - Documentation du produit
title: Filtrage de l’activité des robots de messagerie
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
feature: Email Setup
source-git-commit: f3d0b2be794ca4bb6c38c942cef1fa72fe091d7c
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# Filtrage de l’activité des robots de messagerie {#filtering-email-bot-activity}

Parfois, l’activité de robots de messagerie peut gonfler par erreur les ouvertures de votre email et les données de clics. Suivez les étapes ci-dessous pour résoudre ce problème.

Nous utilisons deux méthodes distinctes pour confirmer l’activité des robots :

* Correspondance avec la [liste de robots Interactive Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target="_blank"} : les activités qui correspondent à tout élément de la liste IAB UA/IP (User Agent/IP address) seront marquées comme des robots.
* Correspondance avec le modèle de proximité : lorsque plusieurs activités se produisent en même temps (en moins d’une seconde), elles sont identifiées comme des robots. Les attributs pris en compte lors de la comparaison sont les suivants :
   * Identifiant de piste (doit être le même)
   * Ressource de messagerie électronique (doit être identique)
   * Clic sur un lien ou ouverture d’un courrier électronique
   * Différence horaire (doit être inférieure à une seconde)

Par rapport aux clics sur les liens de courrier électronique et à l’activité d’ouverture de courrier électronique, de nouveaux attributs seront renseignés avec les valeurs ci-dessous :

* Les activités identifiées comme des robots auront &quot;Activité de robot&quot; comme &quot;True&quot; et &quot;Modèle d’activité de robot&quot; comme modèle/méthode identifié.
* Les activités identifiées comme n’étant pas des robots auront &quot;Activité des robots&quot; comme &quot;False&quot; et &quot;Modèle d’activité des robots&quot; comme &quot;N/A&quot;.
* Les activités qui se sont produites avant l’introduction de ces attributs auront &quot;Activité de robot&quot; comme &quot;&quot; (vide) et &quot;Modèle d’activité de robot&quot; comme &quot;&quot; (vide).

## Sélectionner le type de filtre {#select-filter-type}

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Activité de robot]** .

   ![](assets/filtering-email-bot-activity-3.png)

1. Vous avez le choix entre deux curseur. Vous ne pouvez activer qu’un seul ou les deux. Si vous activez l’option **[!UICONTROL Correspondance avec la liste IAB]**, choisissez d’activer l’activité  _ou_ [!UICONTROL filtrer l’activité de robot].

   ![](assets/filtering-email-bot-activity-4.png)

1. Si vous activez l’option **[!UICONTROL Correspondance avec le modèle de proximité]**, choisissez si vous souhaitez  _ou_ [!UICONTROL filtrer l’activité de robot]. Vous pouvez également définir la durée en secondes de **durée entre les activités** (la valeur par défaut est 0, la valeur maximale est 3).

   ![](assets/filtering-email-bot-activity-5.png)

>[!NOTE]
>
>**Durée entre les activités** définie sur 0 seconde, nous identifierons les activités de courrier électronique qui se produisent exactement à la même seconde. Si plusieurs activités de courrier électronique se produisent au cours de la durée indiquée, elles sont identifiées comme une activité de robot.

>[!IMPORTANT]
>
>* Si vous choisissez [!UICONTROL Filtrer l’activité des robots], il se peut qu’une baisse des ouvertures d’email et des clics s’affiche, car les fausses activités sont éliminées.

**ÉTAPE FACULTATIVE** : pour désactiver l’une des fonctionnalités, désélectionnez simplement le curseur approprié. Si vous le faites, les données ne sont pas réinitialisées.

>[!TIP]
>
>Tirez parti des données d’activité de robots dans les listes dynamiques par l’intermédiaire de la valeur booléenne &quot;Is Bot Activity&quot; (yes/no) et &quot;Bot Activity Pattern&quot; des filtres &quot;Lien cliqué dans le courrier électronique&quot; et &quot;Open Email&quot;, ainsi que des déclencheurs &quot;Clicks Link in Email&quot; et &quot;Opens Email&quot;.

## LISTE BLOQUÉE IP {#ip-blocklist}

Nous avons compilé une liste des adresses IP responsables de la génération de millions d’engagements factices, car l’engagement reçu de l’une des adresses IP suivantes est automatiquement filtré et n’est pas ajouté à votre instance de Marketo Engage. Cela peut se traduire par une réduction des ouvertures d’email, des clics et d’autres activités associées. La liste ci-dessous peut être mise à jour régulièrement.

* 40.94.34.52
* 40.94.34.86
* 52.34.76.65
* 54.70.53.60
* 54.71.187.124
* 60.28.2.248
* 64.235.150.252
* 64.235.153.10
* 64.235.153.2
* 64.235.154.105
* 64.235.154.109
* 64.235.154.140
* 64.74.215.1
* 64.74.215.100
* 64.74.215.138
* 64.74.215.139
* 64.74.215.142
* 64.74.215.146
* 64.74.215.150
* 64.74.215.154
* 64.74.215.158
* 64.74.215.162
* 64.74.215.164
* 64.74.215.166
* 64.74.215.170
* 64.74.215.174
* 64.74.215.176
* 64.74.215.178
* 64.74.215.51
* 64.74.215.56
* 64.74.215.58
* 64.74.215.59
* 64.74.215.86
* 64.74.215.98
* 65.154.226.101
* 66.249.91.149
* 70.42.131.106
* 74.125.217.116
* 74.217.90.250
* 104.129.41.4
* 104.47.55.126
* 104.47.58.126
* 104.47.70.126
* 104.47.73.126
* 104.47.73.254
* 104.47.74.126
* 128.220.160.1
* 155.70.39.101
* 162.129.251.14
* 162.129.251.42
* 208.52.157.204

>[!NOTE]
>
>Nous analysons et analysons méticuleusement chaque adresse IP avant de l’ajouter à cette liste, en veillant à ce que seules les adresses IP les plus critiques et les plus nocives soient bloquées.
