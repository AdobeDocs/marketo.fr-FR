---
unique-page-id: 10092977
description: Filtre de synchronisation Microsoft Dynamics - Qualification - Documents Marketo - Documentation du produit
title: Filtre de synchronisation Microsoft Dynamics - Qualification
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Filtre de synchronisation Microsoft Dynamics : Qualifier {#microsoft-dynamics-sync-filter-qualify}

Lorsque vous souhaitez convertir un prospect en contact dans Microsoft Dynamics, veillez à utiliser ce processus de qualification par défaut. Ensuite, synchronisez-la avec Marketo.

## Processus de conversion {#the-conversion-process}

Voici comment les filtres fonctionnent pendant le processus de conversion.

| Si le filtre de synchronisation des pistes est : | et le filtre de synchronisation des contacts est : | Résultat dans Marketo |
|---|---|---|
| False | False | Rien n’est synchronisé dans Marketo |
| True | True | Le contact est synchronisé dans Marketo |
| False | True | Un nouvel enregistrement de contact est créé dans Marketo |
| True | False | MS Dynamics met à jour les informations de piste dans Marketo mais l’enregistrement de contact n’est pas synchronisé |

>[!CAUTION]
>
>Nous ne prenons en charge que le processus de conversion de qualification prêt à l’emploi.
