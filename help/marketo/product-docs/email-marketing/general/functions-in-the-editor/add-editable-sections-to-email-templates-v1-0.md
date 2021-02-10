---
unique-page-id: 1900585
description: Ajouter des sections modifiables aux modèles de courrier électronique v1.0 - Documents marketing - Documentation du produit
title: Ajouter des sections modifiables aux modèles de courrier électronique v1.0
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Ajouter des sections modifiables aux modèles de courrier électronique v1.0 {#add-editable-sections-to-email-templates-v1.0}

Si vous créez un modèle dans la version 1.0 de l’éditeur de modèles de courrier électronique, vous pouvez rendre toute section modifiable en y plaçant un `<div>` spécial.

>[!NOTE]
>
>**Exemple**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Règles :

1. Le code HTML doit toujours être valide.
1. La classe **mktEditable** doit être incluse.
1. L’ID doit être unique dans ce code HTML.
1. Aucun espace dans l’identifiant.

>[!CAUTION]
>
>Les instructions mktEditable ne peuvent pas être imbriquées.

Si vous souhaitez savoir comment procéder dans la version 2.0 de l’éditeur de modèles de courrier électronique, extrayez [la syntaxe du modèle de courrier électronique](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
