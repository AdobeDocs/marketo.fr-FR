---
description: Ajouter ou supprimer des personnes de votre campagne Dynamics - Documents Marketo - Documentation du produit
title: Ajouter ou supprimer des personnes de votre campagne Dynamics
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Ajouter ou supprimer des personnes de votre campagne Dynamics {#add-or-remove-people-from-your-dynamics-campaign}

## Ajouter à Dynamics Campaign {#add-to-dynamics-campaign}

Cette étape de flux peut être utilisée dans les campagnes dynamiques Marketo Engage pour ajouter des personnes comme pistes ou contacts dans une campagne Microsoft. Si la piste n’existe pas encore dans Dynamics, elle sera automatiquement synchronisée et ajoutée à la campagne.

>[!NOTE]
>
>Cette action de flux est disponible uniquement pour les campagnes de déclenchement .

Dans votre campagne dynamique, recherchez et sélectionnez la campagne Dynamics à laquelle vous souhaitez ajouter vos personnes.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Si vous ne voyez pas de campagne Dynamics dans la liste des campagnes :
>
>* Vérifiez que la synchronisation de campagne est fonctionnelle.
>* La campagne n’est pas active dans [!DNL Microsoft Dynamics]

Le système crée automatiquement une liste de marketing statique propre aux campagnes, qui regroupe les pistes et les contacts, afin d’ajouter la personne. Il s’agit d’une action ponctuelle. Une fois pour les synchronisations suivantes de la campagne, la même liste marketing est utilisée. La norme de dénomination adoptée pour le nom statique de la liste marketing est la suivante : `Mkto-leads-<uniqueID>` pour les pistes et `Mkto-contacts-<uniqueID>` pour les contacts.

L’association de ces listes marketing générées par Marketo à d’autres campagnes peut entraîner un comportement déroutant. Par exemple : l’ajout à une campagne entraîne également l’ajout à la seconde campagne. De même, il n’est pas recommandé de dissocier la liste marketing générée par Marketo de la campagne dans Dynamics.

## Supprimer de Dynamics Campaign {#remove-from-dynamics-campaign}

Cette étape de flux peut être utilisée dans les campagnes dynamiques Marketo pour supprimer des personnes d’une campagne Microsoft. Cela supprime uniquement les pistes d’une campagne qui ont été ajoutées précédemment à la campagne par le biais de l’action de flux &quot;Ajout à la campagne Microsoft&quot;.

>[!NOTE]
>
>Cette action de flux est disponible uniquement pour les campagnes de déclenchement .

Dans votre campagne dynamique, recherchez et sélectionnez la campagne Dynamics dont vous souhaitez supprimer vos personnes.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Si vous ne voyez pas de campagne Dynamics dans la liste des campagnes :
>
>* Vérifiez que la synchronisation de campagne est fonctionnelle.
>* La campagne n’est pas active dans [!DNL Microsoft Dynamics]
