---
unique-page-id: 1147082
description: Supprimer une personne - Documents Marketo - Documentation du produit
title: Supprimer une personne
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Supprimer une personne {#delete-person}

Des personnes erronées entrent parfois dans votre base de données. L’étape de flux Supprimer une personne peut les supprimer.

![](assets/delete-person-1.png)

>[!CAUTION]
>
>Lorsque vous supprimez une personne, toutes ses données RCE historiques sont également supprimées. Elle ne peut pas être annulée.

1. Lorsque vous faites glisser l’étape de flux, elle est automatiquement définie pour être également supprimée de votre CRM.

   ![](assets/delete-person-2.png)

1. Vous pouvez effectuer une suppression depuis Marketo Engage et non depuis votre CRM, comme suit :

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>La suppression de la personne de votre CRM _fonctionne uniquement avec[!DNL Salesforce]_. Si vous supprimez une personne de Marketo et choisissez de la conserver dans [!DNL Salesforce], elle sera recréée dans Marketo si son enregistrement [!DNL Salesforce] est mis à jour.
