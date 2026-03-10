---
unique-page-id: 10092969
description: Comprendre comment fonctionne le filtre de synchronisation Dynamics lors de la fusion de prospects. Découvrez comment la valeur du filtre de synchronisation des enregistrements gagnants détermine si l’enregistrement se synchronise avec Marketo.
title: Filtre de synchronisation Microsoft Dynamics - Fusion
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Filtre de synchronisation [!DNL Microsoft] Dynamics : fusion {#microsoft-dynamics-sync-filter-merge}

La fusion des prospects dans [!DNL Microsoft Dynamics] utilise le type Deux options : Filtre de synchronisation = Oui (TRUE) et Filtre de synchronisation = Non (FALSE). Lorsque vous fusionnez deux enregistrements, le résultat varie en fonction de l&#39;enregistrement qui est Vrai et de celui qui est Faux.

Les enregistrements de leads deviennent true ou false en fonction des règles de workflow définies par l’administrateur pour déterminer le gagnant. Le filtre de synchronisation de l’enregistrement gagnant détermine en fin de compte si l’enregistrement [!DNL MS Dynamics] se synchronise avec Marketo.

C&#39;est lorsqu&#39;un enregistrement est vrai et qu&#39;un autre est faux que ça devient compliqué.

| Si le filtre de synchronisation de l’enregistrement perdu est : | et le filtre de synchronisation pour l’enregistrement gagnant est : | Ceci est le résultat dans Marketo |
|---|---|---|
| [!UICONTROL Vrai] | [!UICONTROL Vrai] | L’enregistrement gagnant continue de se synchroniser avec Marketo |
| [!UICONTROL Faux] | [!UICONTROL Faux] | L’enregistrement gagnant continue à **pas** être synchronisé avec Marketo |
| [!UICONTROL Faux] | [!UICONTROL Vrai] | L’enregistrement gagnant sera synchronisé avec Marketo |
| [!UICONTROL Vrai] | [!UICONTROL Faux] | L’enregistrement gagnant ne sera pas synchronisé avec Marketo |
