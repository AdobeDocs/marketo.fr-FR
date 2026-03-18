---
unique-page-id: 1900585
description: Découvrez comment ajouter des sections modifiables aux modèles d’e-mail dans la version 1.0. Permet aux utilisateurs de modifier des zones spécifiques tout en gardant le reste verrouillé.
title: Ajouter des sections modifiables à des modèles d’e-mail v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '110'
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
