---
unique-page-id: 10092977
description: Filtre Microsoft Dynamics Sync - Qualification - Docs Marketo - Documentation du produit
title: Filtre Microsoft Dynamics Sync -Qualifier
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Filtre Microsoft Dynamics Sync : Qualifier {#microsoft-dynamics-sync-filter-qualify}

Pour convertir un prospect en contact dans Microsoft Dynamics, veillez à utiliser ce processus Qualify par défaut. Ensuite, synchronisez-la avec Marketo.

## Processus de conversion {#the-conversion-process}

Voici comment fonctionnent les filtres pendant le processus de conversion.

| Si le filtre de synchronisation des pistes est : | et le filtre de synchronisation des contacts est : | Résultat dans Marketo |
|---|---|---|
| Faux | Faux | Rien n&#39;est synchronisé au Marketo |
| Vrai | Vrai | Le contact est synchronisé dans Marketo |
| Faux | Vrai | Un nouvel enregistrement de contact est créé dans Marketo |
| Vrai | Faux | MS Dynamics met à jour les informations de piste dans Marketo mais l&#39;enregistrement de contact n&#39;est pas synchronisé |

>[!CAUTION]
>
>Nous ne prenons en charge que le processus de conversion des qualifications prêt à l&#39;emploi.
