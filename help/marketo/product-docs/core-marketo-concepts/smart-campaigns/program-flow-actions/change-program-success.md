---
unique-page-id: 1147009
description: Changer la réussite du programme - Documents Marketo - Documentation du produit
title: Modifier les succès du programme
exl-id: 5b45b6d0-0c3d-4677-8b9a-8bbf03b1209e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 6%

---

# Modifier les succès du programme {#change-program-success}

## APERÇU {#overview}

Si un groupe de personnes a été accidentellement marqué avec succès du programme, vous pouvez utiliser cette étape de flux pour définir la réussite sur true ou false.

![](assets/image2014-9-22-14-3a45-3a8.png)

## Utilisation {#usage}

1. Lorsque vous faites glisser cette étape de flux, le programme est automatiquement défini sur le programme qui contient la campagne dynamique que vous modifiez.

   >[!NOTE]
   >
   >Seuls les membres du programme seront affectés.

   ![](assets/image2014-9-22-14-3a45-3a35.png)

1. Sélectionner **Succès** ou **Date de succès** comme attribut.

   ![](assets/image2014-9-22-14-3a45-3a39.png)

   >[!NOTE]
   >
   >La définition de la date de succès sur un élément définit automatiquement la réussite sur true. La définition de la variable Succès sur true définit automatiquement la Date de succès sur la date actuelle.

1. Définissez la variable **Nouvelle valeur** to **True** ou **False**.

   ![](assets/image2014-9-22-14-3a45-3a55.png)

   >[!TIP]
   >
   >Vous pouvez utiliser l’étape de flux deux fois pour définir à la fois l’indicateur de succès et la date.

Fantastique ! Maintenant, vous savez comment annuler et forcer le succès.
