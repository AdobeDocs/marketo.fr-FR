---
description: Ajouter ou supprimer des personnes de vos documents Dynamics Campaign - Marketo - Documentation sur les produits
title: Ajouter ou supprimer des personnes de votre Dynamics Campaign
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Ajouter ou supprimer des personnes de votre Campaign {#add-or-remove-people-from-your-dynamics-campaign}

## Ajoute à Dynamics Campaign {#add-to-dynamics-campaign}

Cette étape de flux peut être utilisée dans les campagnes Marketo Smart pour ajouter des personnes en tant que pistes ou contacts dans une campagne Microsoft. Si la piste n&#39;existe pas encore dans Dynamics, elle sera automatiquement synchronisée et ajoutée à la campagne.

>[!NOTE]
>
>Cette action de flux est disponible uniquement pour les campagnes de déclenchement.

Dans votre campagne dynamique, recherchez et sélectionnez la campagne dynamique à laquelle vous souhaitez ajouter des personnes.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Si vous ne voyez pas de campagne Dynamics dans la liste de campagne :
>
>* Assurez-vous que Campaign Sync est fonctionnel
>* La campagne n&#39;est pas principale dans Microsoft Dynamics


Le système crée automatiquement une Liste de marketing statique spécifique à une campagne, chacune pour les pistes et les contacts, à laquelle ajouter la personne. Il s’agit d’une action ponctuelle et une fois que les synchronisations suivantes de la campagne ont lieu, la même Liste Marketing est utilisée. La norme de dénomination adoptée pour le nom statique de la Liste marketing est `Mkto-leads-<uniqueID>` pour les pistes et `Mkto-contacts-<uniqueID>` pour les contacts.

L’association de ces Listes marketing générées par Marketo à d’autres campagnes peut conduire à un comportement déroutant. Par exemple : l’ajout à une campagne entraîne également l’ajout à la deuxième campagne. De même, il n&#39;est pas recommandé de dissocier la Liste marketing générée par Marketo de Campaign dans Dynamics.

## Supprimer de Dynamics Campaign {#remove-from-dynamics-campaign}

Cette étape de flux peut être utilisée dans les campagnes Marketo Smart pour supprimer des personnes d&#39;une campagne Microsoft. Ceci supprime uniquement les pistes d&#39;un Campaign qui ont été précédemment ajoutées au Campaign par le biais de l&#39;action de flux &quot;Ajouté à Microsoft Campaign&quot;.

>[!NOTE]
>
>Cette action de flux est disponible uniquement pour les campagnes de déclenchement.

Dans votre campagne intelligente, recherchez et sélectionnez la campagne Dynamics dont vous souhaitez supprimer les utilisateurs.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Si une campagne Dynamics n&#39;apparaît pas dans la liste de campagne :
>
>* Assurez-vous que Campaign Sync est fonctionnel
>* La campagne n&#39;est pas principale dans Microsoft Dynamics

