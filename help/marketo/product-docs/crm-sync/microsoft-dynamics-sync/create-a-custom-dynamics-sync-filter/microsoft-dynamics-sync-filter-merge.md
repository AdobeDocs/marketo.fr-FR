---
unique-page-id: 10092969
description: Filtre Microsoft Dynamics Sync -Fusion - Documents Marketo - Documentation du produit
title: Filtre Microsoft Dynamics Sync -Fusion
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Filtre Microsoft Dynamics Sync : Fusionner {#microsoft-dynamics-sync-filter-merge}

La fusion de pistes dans Microsoft Dynamics utilise le type Deux options - Filtre de synchronisation = Oui (TRUE) et Filtre de synchronisation = Non (FALSE). Lorsque vous fusionnez deux enregistrements, le résultat varie selon l’enregistrement True et False.

Les enregistrements de piste deviennent vrais ou faux en fonction des règles de flux de travail définies par l&#39;administrateur pour déterminer le gagnant. Le filtre de synchronisation pour l&#39;enregistrement gagnant détermine finalement si l&#39;enregistrement MS Dynamics se synchronise avec Marketo.

C&#39;est quand un enregistrement est vrai et qu&#39;un autre est faux que ça devient délicat.

| Si le filtre de synchronisation pour l&#39;enregistrement perdu est : | et le filtre de synchronisation pour l&#39;enregistrement gagnant est : | Résultat dans Marketo |
|---|---|---|
| Vrai | Vrai | L&#39;enregistrement gagnant continue la synchronisation avec Marketo |
| Faux | Faux | L’enregistrement gagnant continue à **ne pas** synchroniser avec Marketo. |
| Faux | Vrai | L&#39;enregistrement gagnant sera synchronisé avec Marketo |
| Vrai | Faux | L&#39;enregistrement gagnant ne sera pas synchronisé avec Marketo |
