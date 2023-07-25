---
unique-page-id: 1900585
description: Ajout de sections modifiables aux modèles de courrier électronique v1.0 - Documents Marketo - Documentation du produit
title: Ajout de sections modifiables aux modèles de courrier électronique v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 2%

---

# Ajout de sections modifiables aux modèles de courrier électronique v1.0 {#add-editable-sections-to-email-templates-v1.0}

Si vous créez un modèle dans la version 1.0 de l’éditeur de modèles d’email, vous pouvez rendre n’importe quelle section modifiable en plaçant un `<div>` autour.

>[!NOTE]
>
>**Exemple**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Règles :

1. Le HTML doit toujours être valide.
1. La classe de **mktEditable** doit être inclus.
1. L’identifiant doit être unique dans ce HTML.
1. Aucun espace dans l’ID.

>[!CAUTION]
>
>Les instructions mktEditable ne peuvent pas être imbriquées.

Si vous souhaitez apprendre à le faire dans la version 2.0 de l’éditeur de modèles d’email, extrayez-le. [syntaxe du modèle d&#39;email](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
