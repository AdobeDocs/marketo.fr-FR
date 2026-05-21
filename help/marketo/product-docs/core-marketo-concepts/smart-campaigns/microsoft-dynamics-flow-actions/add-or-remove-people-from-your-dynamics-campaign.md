---
description: Découvrez comment ajouter ou supprimer des personnes d’une campagne Microsoft Dynamics avec une étape de flux. Synchronisez Marketo avec les campagnes Dynamics.
title: Ajouter ou supprimer des personnes de votre  [!DNL Dynamics]  Campaign
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
TQID: https://experienceleague.adobe.com/b6tUqixPGr7ZWTUKVg4L6EKryziHA2IwzpuTepWWEwU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 324
ht-degree: 0%

---

# Ajouter ou supprimer des personnes de votre campagne [!DNL Dynamics] {#add-or-remove-people-from-your-dynamics-campaign}

## Ajouter à Dynamics Campaign {#add-to-dynamics-campaign}

Cette étape de flux peut être utilisée dans les campagnes intelligentes Marketo Engage pour ajouter des personnes en tant que prospects ou contacts dans une campagne Microsoft. Si le prospect n’existe pas encore dans Dynamics, il sera automatiquement synchronisé et ajouté à la campagne.

>[!NOTE]
>
>Cette action de flux est disponible uniquement pour les campagnes de déclenchement.

Dans votre campagne intelligente, recherchez et sélectionnez la campagne Dynamics à laquelle vous souhaitez ajouter vos personnes.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Si une campagne Dynamics n’apparaît pas dans la liste des campagnes :
>
>* Vérifier que la synchronisation de la campagne est fonctionnelle
>* La campagne n’est pas active dans [!DNL Microsoft Dynamics]

Le système crée automatiquement une liste marketing statique spécifique à une campagne, pour chaque prospect et contact, à laquelle ajouter la personne. Il s’agit d’une action unique, qui n’est utilisée qu’une seule fois pour les synchronisations suivantes de la campagne. La norme de dénomination adoptée pour le nom statique de la liste marketing est `Mkto-leads-<uniqueID>` pour les prospects et `Mkto-contacts-<uniqueID>` pour les contacts.

L’association de ces listes marketing générées par Marketo à d’autres campagnes peut entraîner un comportement déroutant. Par exemple : l’ajout de à une campagne entraîne également l’ajout de à la deuxième campagne. De même, il n’est pas recommandé de dissocier la liste marketing générée par Marketo de la campagne dans [!DNL Dynamics].

## Supprimer de Dynamics Campaign {#remove-from-dynamics-campaign}

Cette étape de flux peut être utilisée dans les campagnes intelligentes Marketo pour supprimer des personnes d’une campagne Microsoft. Cette opération supprime uniquement les prospects d’une campagne qui ont été précédemment ajoutés à la campagne par le biais de l’action de flux « Ajouté à Microsoft Campaign ».

>[!NOTE]
>
>Cette action de flux est disponible uniquement pour les campagnes de déclenchement.

Dans votre campagne intelligente, recherchez et sélectionnez la campagne Dynamics dont vous souhaitez supprimer vos membres.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Si aucune campagne [!DNL Dynamics] n’apparaît dans la liste des campagnes :
>
>* Vérifier que la synchronisation de la campagne est fonctionnelle
>* La campagne n’est pas active dans [!DNL Microsoft Dynamics]
