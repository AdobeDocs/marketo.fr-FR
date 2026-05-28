---
unique-page-id: 14352464
description: Découvrez les tableaux de bord de création de rapports dans Salesforce qui utilisent les données Sales Connect. Affichez les activités d’appel et d’e-mail dans les rapports et tableaux de bord Salesforce.
title: Tableaux de bord de rapports dans Salesforce
exl-id: f27ba3e1-210b-46df-81b5-e794826d36c7
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/lMQ6PcQxFGVRh9FuQw8iHeM4Q5EZX8KwApQzw8jjdMg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 214
ht-degree: 3%

---

# Tableaux de bord de rapports dans Salesforce {#reporting-dashboards-in-salesforce}

Découvrez comment configurer des tableaux de bord ci-dessous.

## Ouvrir et cliquer sur le rapport {#open-and-click-report}

1. Sélectionnez le type d’enregistrement **[!UICONTROL Tâches et Événements]**.
1. Définissez les paramètres de rapport en fonction de la période et de la structure hiérarchique de votre choix.
1. Ajoutez un filtre pour supprimer les e-mails internes consignés dans [!DNL Salesforce] (par exemple, Société/Compte différent de Marketo).
1. Sélectionnez le format de rapport **[!UICONTROL Résumé]**.
1. Ajoutez au rapport les champs Objet, Affecté et Ventes Marketo sur lesquelles l’utilisateur a cliqué/Ventes Marketo vues .
1. Double-cliquez sur **[!UICONTROL Ajouter une formule]** dans le volet Champs .
1. Ajoutez un nom à la formule, sélectionnez **[!UICONTROL Pourcentage]** au format, puis **[!UICONTROL Regroupement 1]**.
1. Sélectionnez **[!UICONTROL Ventes Marketo sur lesquelles vous avez cliqué/Ventes Marketo consultées]** puis **[!UICONTROL Somme]** dans les champs de résumé.
1. Ajoutez un signe diviser à la formule, puis sélectionnez **[!UICONTROL Nombre d’enregistrements]** dans les champs Résumé - _Enregistrer sous_.

## Rapport sur les performances des modèles {#template-performance-report}

1. Personnalisez le rapport Ouverture et clic pour inclure les champs suivants : _Enregistrer sous_.

## Rapport sur le volume des modèles {#template-volume-report}

1. Modifiez le Rapport de performances des modèles et incluez le filtre « Modèle de vente Marketo différent de vide ».
1. Supprimez le champ Marketo Sales Clicked - _Enregistrer sous_.

## Rapport des comptes de tendance {#trending-accounts-report}

1. Sélectionnez Activités avec type d’enregistrement Comptes .
1. Configurez les paramètres et champs de rapport comme indiqué ci-dessous : _Enregistrer sous_.
