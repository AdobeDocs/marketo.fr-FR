---
unique-page-id: 1900585
description: Ajouter des sections modifiables aux modèles de courrier électronique v1.0 - Documents marketing - Documentation du produit
title: Ajouter des sections modifiables aux modèles de courrier électronique v1.0
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Ajouter des sections modifiables aux modèles de courrier électronique v1.0 {#add-editable-sections-to-email-templates-v1.0}

Si vous créez un modèle dans la version 1.0 de l’éditeur de modèles de courrier électronique, vous pouvez rendre n’importe quelle section modifiable en y plaçant un `<div>` cadre spécial.

>[!NOTE]
>
>**Exemple**
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Règles :

1. Le code HTML doit toujours être valide.
1. La classe de **mktEditable** doit être incluse.
1. L’ID doit être unique dans ce code HTML.
1. Aucun espace dans l’identifiant.

>[!CAUTION]
>
>Les instructions mktEditable ne peuvent pas être imbriquées.

Si vous souhaitez savoir comment procéder dans la version 2.0 de l’éditeur de modèles de courrier électronique, extrayez la syntaxe [du modèle de](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)courrier électronique.
