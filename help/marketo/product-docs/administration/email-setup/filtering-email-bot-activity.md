---
description: Filtrage de l’activité de robot d’e-mail - Documents Marketo - Documentation du produit
title: Filtrage de l’activité des robots d’e-mail
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
feature: Email Setup
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Filtrage de l’activité des robots d’e-mail {#filtering-email-bot-activity}

Parfois, l’activité des robots d’e-mail peut gonfler par erreur les données d’ouvertures d’e-mail et de clics. Suivez les étapes ci-dessous pour résoudre ce problème.

Nous utilisons deux méthodes distinctes pour confirmer l’activité des robots :

* Correspondance avec [liste de robots Interactive Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target="_blank"} : les activités qui correspondent à tout ce qui figure dans la liste IAB UA/IP (agent utilisateur/adresse IP) seront marquées comme des robots.
* Correspondance avec le modèle de proximité : lorsque plusieurs activités se produisent en même temps (en moins d’une seconde), elles sont identifiées comme des robots. Les attributs pris en compte lors de la comparaison sont les suivants :
   * ID de lead (doit être le même)
   * Ressource e-mail (doit être la même)
   * Clic sur un lien ou ouverture d’un e-mail
   * Décalage horaire (doit être inférieur à une seconde)

Par rapport aux activités clic sur les liens d’e-mail et ouverture de l’e-mail , les nouveaux attributs seront renseignés avec les valeurs ci-dessous :

* Les activités identifiées comme des robots auront « Activité de robot » comme « Vrai » et « Modèle d’activité de robot » comme modèle/méthode identifié
* Les activités identifiées comme n’étant pas des robots auront « Activité de robot » comme « Fausse » et « Modèle d’activité de robot » comme « S.O. »
* Les activités qui se sont produites avant l’introduction de ces attributs auront « Activité de robot » comme « » (vide) et « Modèle d’activité de robot » comme « » (vide)

## Sélectionner le type de filtre {#select-filter-type}

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Cliquez sur **[!UICONTROL Email]**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Cliquez sur l’onglet **[!UICONTROL Activité de robot]**.

   ![](assets/filtering-email-bot-activity-3.png)

1. Vous avez le choix entre deux curseurs. Vous pouvez en activer un seul ou les deux. Si vous activez **[!UICONTROL Correspondre avec la liste IAB]**, choisissez de [!UICONTROL consigner l’activité de robot] _ou_ [!UICONTROL filtrer l’activité de robot].

   ![](assets/filtering-email-bot-activity-4.png)

1. Si vous activez **[!UICONTROL Correspondance avec le modèle de proximité]**, choisissez de [!UICONTROL consigner l’activité de robot] _ou_ [!UICONTROL filtrer l’activité de robot]. Vous pouvez également définir le nombre de secondes pour **Durée entre les activités** (0 par défaut, 3 au maximum).

   ![](assets/filtering-email-bot-activity-5.png)

>[!NOTE]
>
>Lorsque la valeur **Durée entre les activités** est définie sur 0 seconde, nous identifions les activités d’e-mail qui se produisent exactement à la même seconde. Si plusieurs activités de courrier électronique se produisent dans le délai spécifié de secondes, elles seront identifiées comme des activités de robots.

>[!IMPORTANT]
>
>* Si vous choisissez [!UICONTROL Filtrer l’activité des robots], une baisse des ouvertures d’e-mails et des clics peut s’afficher, car les fausses activités sont éliminées.

**ÉTAPE FACULTATIVE** : pour désactiver l’une des fonctionnalités, désélectionnez simplement le curseur correspondant. Si vous le faites, les données ne sont pas réinitialisées.

>[!TIP]
>
>Tirez parti des données d’activité des robots dans les listes dynamiques via les valeurs booléennes « Est une activité de robot » (oui/non) et « Modèle d’activité de robot » dans les filtres « Lien cliqué dans l’e-mail » et « Ouvrir l’e-mail », ainsi que les déclencheurs « Clics sur le lien dans l’e-mail » et « Ouvre l’e-mail ».

## IP, Place sur la liste bloquée {#ip-blocklist}

Nous avons compilé une liste d’adresses IP responsables de la génération de millions de faux engagements, car ces engagements reçus de l’une des adresses IP suivantes sont automatiquement filtrés et ne sont pas ajoutés à votre instance Marketo Engage. Cela peut entraîner une réduction des ouvertures d’e-mail, des clics et d’autres activités associées. La liste ci-dessous peut être mise à jour périodiquement.

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
>Nous analysons et examinons minutieusement chaque adresse IP avant de l&#39;ajouter à cette liste, en nous assurant que seules les adresses IP les plus critiques et les plus dangereuses sont bloquées.
