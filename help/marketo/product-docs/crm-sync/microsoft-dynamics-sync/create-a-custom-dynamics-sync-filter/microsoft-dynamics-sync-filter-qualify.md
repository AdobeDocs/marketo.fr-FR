---
unique-page-id: 10092977
description: Découvrez le processus de qualification du filtre de synchronisation Dynamics lors de la conversion d’un prospect en contact. Découvrez comment les valeurs des filtres de synchronisation des leads et des contacts affectent la synchronisation Marketo.
title: Filtre de synchronisation Microsoft Dynamics - Qualifier
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/3jC9Y9fpBNjUzjE1Dy7JBuhNlYQpnc7kjF2LxV-hrp4'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '124'
ht-degree: 0%
---
# Filtre de synchronisation [!DNL Microsoft Dynamics] : qualifier {#microsoft-dynamics-sync-filter-qualify}

Lorsque vous souhaitez convertir un prospect en contact dans [!DNL Microsoft Dynamics], utilisez ce processus de qualification par défaut. Ensuite, synchronisez-le avec Marketo.

## Processus de conversion {#the-conversion-process}

| Si le filtre de synchronisation des prospects est : | et le filtre de synchronisation des contacts est : | Ceci est le résultat dans Marketo |
|---|---|---|
| [!UICONTROL Faux] | [!UICONTROL Faux] | Rien n’est synchronisé dans Marketo |
| [!UICONTROL Vrai] | [!UICONTROL Vrai] | Le contact est synchronisé dans Marketo |
| [!UICONTROL Faux] | [!UICONTROL Vrai] | Création d’un nouvel enregistrement de contact dans Marketo |
| [!UICONTROL Vrai] | [!UICONTROL Faux] | [!DNL MS Dynamics] met à jour les informations de lead dans Marketo, mais l’enregistrement du contact n’est pas synchronisé |

>[!CAUTION]
>
>Nous prenons uniquement en charge le processus de conversion Qualifier prêt à l’emploi.
