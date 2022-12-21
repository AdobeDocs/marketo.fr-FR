---
unique-page-id: 10092969
description: Filtre de synchronisation Microsoft Dynamics - Fusion - Documents Marketo - Documentation du produit
title: Filtre de synchronisation Microsoft Dynamics - Fusion
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Filtre de synchronisation Microsoft Dynamics : Fusion {#microsoft-dynamics-sync-filter-merge}

La fusion de pistes dans Microsoft Dynamics utilise le type Deux options - Filtre de synchronisation = Oui (TRUE) et Filtre de synchronisation = Non (FALSE). Lorsque vous fusionnez deux enregistrements, le résultat varie en fonction de l’enregistrement True et de l’enregistrement False.

Les enregistrements de piste deviennent vrais ou faux en fonction des règles de workflow définies par l’administrateur pour déterminer le gagnant. Le filtre de synchronisation pour l’enregistrement gagnant détermine finalement si l’enregistrement MS Dynamics est synchronisé avec Marketo.

C&#39;est quand un enregistrement est vrai et qu&#39;un enregistrement est faux qu&#39;il devient délicat.

| Si le filtre de synchronisation pour l’enregistrement perdu est : | et le filtre de synchronisation pour l’enregistrement gagnant est : | Résultat dans Marketo |
|---|---|---|
| True | True | L’enregistrement gagnant se synchronise toujours avec Marketo. |
| False | False | Le record de la victoire continue **not** synchronisation avec Marketo |
| False | True | L’enregistrement gagnant sera synchronisé avec Marketo. |
| True | False | L’enregistrement gagnant ne sera pas synchronisé avec Marketo |
