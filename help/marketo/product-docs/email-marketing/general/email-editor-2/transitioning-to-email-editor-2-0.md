---
unique-page-id: 11373011
description: Transition vers Email Editor 2.0 - Documents Marketo - Documentation du produit
title: Transition vers Email Editor 2.0
exl-id: eb9ec8cc-d6e8-4839-a4d9-608d2f264cbb
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 0%

---

# Transition vers Email Editor 2.0 {#transitioning-to-email-editor}

Depuis la version du 19 juin, tous les abonnements Marketo ont été transférés vers l’éditeur de messagerie 2.0. [En savoir plus](https://nation.marketo.com/docs/DOC-7038) sur l’obsolescence de l’éditeur de messagerie 1.0.

Les emails et les modèles d’email de votre abonnement doivent comporter un numéro de version. La version se trouve dans la page de résumé de la ressource.

![](assets/five-5.png)

Par défaut, tous les emails et modèles de courrier électronique existants seront marqués comme v1.0 s’ils ont été créés avant la version du printemps 16 ou après la version lorsque l’éditeur de courrier électronique 2.0 est désactivé. L’éditeur de messagerie 2.0 étant désormais activé automatiquement, le comportement suivant s’affiche :

* Lorsque vous créez un email, le [sélecteur de modèle d&#39;email](email-template-picker-overview.md) s&#39;affiche et vous pouvez choisir un modèle de courrier électronique v2.0.
* Chaque fois que vous créez ou modifiez un email avec Email Editor 2.0, l&#39;email résultant est **always** marqué comme v2.0 (même si vous avez utilisé un modèle de courrier électronique v1.0).

Si votre abonnement comporte des courriers électroniques v1.0 avant le passage à l’éditeur de messagerie 2.0, vous remarquerez le comportement suivant en fonction de l’état actuel de la ressource :

**Approuvé** - Cliquez sur &quot;Modifier le brouillon&quot; pour créer un brouillon v2.0 du courrier électronique approuvé. Si vous approuvez ensuite le brouillon v2.0, l’état approuvé de l’email devient v2.0 et il n’est pas possible de revenir à la version 1.0.\
**Version préliminaire** - Cliquez sur &quot;Modifier la version préliminaire&quot; pour marquer automatiquement ce brouillon comme v2.0. À ce stade, il ne sera pas possible d’ignorer et de restaurer la version 1.0, car il n’existe pas de version approuvée de la ressource.
**Approuvé avec brouillon** - Cliquez sur &quot;Modifier le brouillon&quot; pour marquer automatiquement ce brouillon comme v2.0. Pour cette raison, il n’est pas non plus possible de rétablir la version 1.0 du brouillon.

Si votre abonnement comporte des modèles de courrier électronique v1.0 avant de passer à Email Editor 2.0, le comportement suivant s’affiche :

**Approuvé** - Cliquez sur &quot;Modifier le brouillon&quot; pour créer un brouillon v2.0 du modèle de courrier électronique existant.
**Version préliminaire** - Cliquez sur &quot;Modifier la version préliminaire&quot; pour marquer automatiquement ce brouillon comme v2.0. À ce stade, il ne serait pas possible de supprimer et de restaurer la version 1.0, car il n’existe pas de version approuvée de la ressource.
**Approuvé avec brouillon** - Cliquez sur &quot;Modifier le brouillon&quot; pour marquer automatiquement ce brouillon comme v2.0. Pour cette raison, il n’est pas non plus possible de rétablir la version 1.0 du brouillon.

Si vous approuvez un modèle de courrier électronique qui était précédemment v1.0 (dans l’un des états ci-dessus), le comportement suivant s’affiche :

Pour les emails v1.0 existants qui utilisaient le modèle (précédemment v1.0) :\
**E-mail v1.0 approuvé** - Un brouillon v2.0 sera créé pour cet e-mail, en utilisant toujours le modèle v2.0 nouvellement approuvé. Il recevra également toutes les modifications de modèle.\
**Version préliminaire v1.0 email** - Le brouillon restera v1.0 jusqu’à ce que vous cliquiez sur &quot;Modifier le brouillon&quot;. Ensuite, il sera automatiquement marqué comme v2.0 et recevra toutes les modifications de modèle.\
**Approuvé avec brouillon de la version 1.0 email** - Le brouillon restera v1.0 jusqu’à ce que vous cliquiez sur &quot;Modifier brouillon&quot;. Ensuite, il sera automatiquement marqué comme v2.0 et recevra toutes les modifications de modèle.

Pour les emails v2.0 existants qui utilisaient le modèle (précédemment v1.0) :\
**E-mail v2.0 approuvé** - Un brouillon v2.0 sera créé pour cet e-mail, &quot;utilisant&quot; toujours le modèle nouvellement approuvé, et recevra toutes les modifications de modèle.\
**Version préliminaire v2.0 email** - Le brouillon restera tel quel (v2.0) et recevra toutes les modifications de modèle.\
**Approuvé avec brouillon de courrier électronique v2.0** - Le brouillon restera tel quel (v2.0) et recevra toutes les modifications de modèle.

>[!CAUTION]
>
>Si vous approuvez un brouillon v2.0 d’un modèle de courrier électronique v1.0, le modèle deviendra v2.0. Il existe **aucun moyen** de restaurer la version 1.0.

Informations à noter

* Les courriers électroniques approuvés sont **never** modifiés.

* Les modèles de courrier électronique approuvés sont **never** modifiés.

* Dans quelques **rares** cas, un email v1.0 ne peut pas être ouvert dans Email Editor 2.0. Si cela se produit, ignorez le brouillon et contactez le support Marketo.

>[!MORELIKETHIS]
>
>* [Présentation de l’éditeur de messagerie 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Syntaxe du modèle de courrier électronique](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)
