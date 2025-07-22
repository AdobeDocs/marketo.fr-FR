---
unique-page-id: 10092977
description: Filtre de synchronisation Microsoft Dynamics - Qualifier - Documents Marketo - Documentation du produit
title: Filtre de synchronisation Microsoft Dynamics - Qualifier
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 0%

---

# Filtre de synchronisation [!DNL Microsoft Dynamics] : qualifier {#microsoft-dynamics-sync-filter-qualify}

Lorsque vous souhaitez convertir un prospect en contact dans [!DNL Microsoft Dynamics], veillez à utiliser ce processus de qualification par défaut. Ensuite, synchronisez-le avec Marketo.

## Processus de conversion {#the-conversion-process}

Voici comment fonctionnent les filtres pendant le processus de conversion.

| Si le filtre de synchronisation des prospects est : | et le filtre de synchronisation des contacts est : | Ceci est le résultat dans Marketo |
|---|---|---|
| [!UICONTROL Faux] | [!UICONTROL Faux] | Rien n’est synchronisé dans Marketo |
| [!UICONTROL Vrai] | [!UICONTROL Vrai] | Le contact est synchronisé dans Marketo |
| [!UICONTROL Faux] | [!UICONTROL Vrai] | Création d’un nouvel enregistrement de contact dans Marketo |
| [!UICONTROL Vrai] | [!UICONTROL Faux] | [!DNL MS Dynamics] met à jour les informations de lead dans Marketo, mais l’enregistrement du contact n’est pas synchronisé |

>[!CAUTION]
>
>Nous prenons uniquement en charge le processus de conversion Qualifier prêt à l’emploi.
