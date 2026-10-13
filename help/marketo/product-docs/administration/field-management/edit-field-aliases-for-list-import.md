---
unique-page-id: 2360346
description: Créez et modifiez des alias de champ afin que les imports de liste avec des en-têtes de colonne inconnus soient mappés aux champs Marketo corrects.
title: Modifier les alias de champ pour l’import de liste
exl-id: 0cc2f4c8-6858-4b41-bae3-4a8d267efe88
feature: Field Management
TQID: 'https://experienceleague.adobe.com/LTuFa4OBnrBF5k8YHuLkamnfirQSa-NXFq534w21Xyk'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: f5e85a9b-a883-40d0-8759-f3651efb32e9
    internal-label: Field management
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 11%
---
# Modifier les alias de champ pour l’import de liste {#edit-field-aliases-for-list-import}

Lorsque vous importez une liste dont les en-têtes sont inconnus, vous pouvez créer des alias de champ pour simplifier les futures importations. Vous pouvez également modifier ces alias dans la gestion des champs.

>[!NOTE]
>
>**Autorisations d’administration requises**

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/edit-field-aliases-for-list-import-1.png)

1. Cliquez sur **[!UICONTROL Gestion des champs]**.

   ![](assets/edit-field-aliases-for-list-import-2.png)

1. Recherchez et sélectionnez le champ auquel vous souhaitez ajouter un alias.

   ![](assets/edit-field-aliases-for-list-import-3.png)

1. Dans la liste déroulante **[!UICONTROL Actions de champ]**, cliquez sur **[!UICONTROL Modifier les alias d’importation]**.

   ![](assets/edit-field-aliases-for-list-import-4.png)

1. Saisissez un alias et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/edit-field-aliases-for-list-import-5.png)

>[!TIP]
>
>Cliquez sur **[!UICONTROL Ajouter autre]** et saisissez d’autres alias si vous en avez besoin.

Désormais, si vous importez une feuille de calcul avec une colonne nommée « DOB », Marketo la reconnaîtra automatiquement comme étant sa « date de naissance » et importera les données dans le champ approprié.

![](assets/edit-field-aliases-for-list-import-6.png)
