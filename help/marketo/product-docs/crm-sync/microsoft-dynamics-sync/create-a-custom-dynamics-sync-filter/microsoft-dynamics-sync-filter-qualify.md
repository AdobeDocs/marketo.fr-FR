---
unique-page-id: 10092977
description: Filtre de synchronisation Microsoft Dynamics - Qualification - Documents Marketo - Documentation du produit
title: Filtre de synchronisation Microsoft Dynamics - Qualification
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 6%

---

# Filtre de synchronisation Microsoft Dynamics : admissible {#microsoft-dynamics-sync-filter-qualify}

Lorsque vous souhaitez convertir un prospect en contact dans Microsoft Dynamics, veillez à utiliser ce processus de qualification par défaut. Ensuite, synchronisez-la avec Marketo Engage.

## Processus de conversion {#the-conversion-process}

Voici comment les filtres fonctionnent pendant le processus de conversion.

| Si le filtre de synchronisation des pistes est : | et le filtre de synchronisation des contacts est : | Résultat dans Marketo |
|---|---|---|
| false | false | Rien n’est synchronisé dans Marketo |
| Vrai | Vrai | Le contact est synchronisé dans Marketo |
| false | Vrai | Un nouvel enregistrement de contact est créé dans Marketo |
| Vrai | false | MS Dynamics met à jour les informations de piste dans Marketo mais l’enregistrement de contact n’est pas synchronisé |

>[!CAUTION]
>
>Nous ne prenons en charge que le processus de conversion de qualification prêt à l’emploi.
