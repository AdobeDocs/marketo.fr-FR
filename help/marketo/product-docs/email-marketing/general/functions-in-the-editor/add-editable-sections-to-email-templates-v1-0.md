---
unique-page-id: 1900585
description: Découvrez comment ajouter des sections modifiables aux modèles d’e-mail dans la version 1.0. Permet aux utilisateurs de modifier des zones spécifiques tout en gardant le reste verrouillé.
title: Ajouter des sections modifiables à des modèles d’e-mail v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
TQID: https://experienceleague.adobe.com/j2rwpy7Bq-HH3-mva5FkDb3kKH8cvlH2hMUp0ic7sno
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 14%

---

# Ajouter des sections modifiables à des modèles d’e-mail v1.0 {#add-editable-sections-to-email-templates-v1.0}

Si vous créez un modèle dans l’éditeur de modèles d’e-mail v1.0, vous pouvez rendre n’importe quelle section modifiable en y ajoutant un `<div>` spécial.

>[!NOTE]
>
>**Exemple**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Règles :

1. L’HTML doit toujours être valide.
1. La classe de **mktEditable** doit être incluse.
1. L’ID doit être unique dans cette HTML.
1. Pas d’espace dans l’ID.

>[!CAUTION]
>
>Les instructions mktEditable ne peuvent pas être imbriquées.

Si vous souhaitez apprendre à le faire dans l’éditeur de modèles d’e-mail v2.0, consultez la section [Syntaxe du modèle d’e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
