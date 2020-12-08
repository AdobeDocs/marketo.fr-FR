---
unique-page-id: 10092977
description: Filtre Microsoft Dynamics Sync - Qualification - Documents marketing - Documentation du produit
title: Filtre Microsoft Dynamics Sync -Qualifier
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Filtre Microsoft Dynamics Sync : Qualifier {#microsoft-dynamics-sync-filter-qualify}

Pour convertir un prospect en contact dans Microsoft Dynamics, veillez à utiliser ce processus Qualify par défaut. Ensuite, synchronisez-la avec Marketo.

## Le processus de conversion {#the-conversion-process}

Voici comment fonctionnent les filtres pendant le processus de conversion.

| Si le filtre de synchronisation des pistes est : | et le filtre de synchronisation des contacts est : | Résultat de Marketo |
|---|---|---|
| False | False | Rien n&#39;est synchronisé dans Marketo |
| True | True | Le contact est synchronisé dans Marketo |
| False | True | Un nouvel enregistrement de contact est créé dans Marketo |
| True | False | MS Dynamics met à jour les informations de piste dans Marketo mais l&#39;enregistrement de contact n&#39;est pas synchronisé |

>[!CAUTION]
>
>Nous ne prenons en charge que le processus de conversion des qualifications prêt à l&#39;emploi.

