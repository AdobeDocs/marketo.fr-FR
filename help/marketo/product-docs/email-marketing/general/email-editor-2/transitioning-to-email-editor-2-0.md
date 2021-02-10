---
unique-page-id: 11373011
description: Passage à la version 2.0 de l’éditeur de courrier électronique - Documentation du marketing - Documentation du produit
title: Transition vers l’éditeur de messagerie 2.0
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# Passage à l’éditeur de courrier électronique 2.0 {#transitioning-to-email-editor}

À compter de la [version du 19 juin](/help/marketo/release-notes/2016/release-notes-spring-16.md), tous les abonnements de Marketo ont été convertis en Éditeur de courriel 2.0. [En savoir plus](https://nation.marketo.com/docs/DOC-7038) sur la dépréciation de l&#39;Éditeur de courriel 1.0.

Les courriers électroniques et les modèles de courrier électronique de votre abonnement doivent avoir un numéro de version. La version se trouve dans la page de résumé du fichier.

![](assets/five-5.png)

Par défaut, tous vos e-mails et modèles de courrier électronique existants seront marqués comme v1.0 s’ils ont été créés avant la version du printemps 16 ou après la version lorsque l’éditeur de courrier électronique 2.0 est désactivé. L’éditeur de messagerie 2.0 étant désormais automatiquement activé, le comportement suivant s’affiche :

* Lorsque vous créez un courrier électronique, le sélecteur de modèles de courrier électronique [](email-template-picker-overview.md) s’affiche et vous pouvez choisir un modèle de courrier électronique v2.0.
* Chaque fois que vous créez ou modifiez un courrier électronique à l’aide de la version 2.0 de l’Editeur de messagerie, le courrier électronique obtenu **toujours** est marqué comme v2.0 (même si vous avez utilisé un modèle de courrier électronique de la version 1.0).

Si votre abonnement contient des courriers électroniques de la version 1.0 avant le passage à la version 2.0 de l’éditeur de messagerie, vous constaterez le comportement suivant en fonction de l’état actuel de la ressource :

**Approuvé**  - Cliquez sur &quot;Modifier le brouillon&quot; pour créer un brouillon v2.0 du courrier électronique approuvé. Si vous approuvez ensuite le brouillon v2.0, l’état approuvé du courrier électronique devient v2.0 et il n’est pas possible de revenir à la version 1.0.\
**Version préliminaire**  - Le fait de cliquer sur &quot;Modifier le brouillon&quot; marquera automatiquement ce brouillon comme v2.0. À ce stade, il ne sera pas possible de supprimer et de revenir à la version 1.0 car il n&#39;existe pas de version approuvée de la ressource.
**Approuvé avec brouillon**  - Le fait de cliquer sur &quot;Modifier le brouillon&quot; marquera alors automatiquement ce brouillon comme v2.0. De ce fait, il n&#39;y a aucun moyen de rétablir le brouillon à v1.0.

Si votre abonnement dispose de modèles de courrier électronique v1.0 avant de passer à la version 2.0 de l’Editeur de messagerie, vous allez connaître le comportement suivant :

**Approuvé**  - Cliquez sur &quot;Modifier le brouillon&quot; pour créer un brouillon v2.0 du modèle de courrier électronique existant.
**Version préliminaire**  - Le fait de cliquer sur &quot;Modifier le brouillon&quot; marquera automatiquement ce brouillon comme v2.0. À ce stade, il ne sera pas possible de supprimer et de revenir à la version 1.0 car il n’existe pas de version approuvée de la ressource.
**Approuvé avec brouillon**  - Le fait de cliquer sur &quot;Modifier le brouillon&quot; marquera automatiquement ce brouillon comme v2.0. De ce fait, il n&#39;y a aucun moyen de rétablir le brouillon à v1.0.

Si vous approuvez un modèle de courrier électronique qui était précédemment v1.0 (dans l’un des états ci-dessus), le comportement suivant s’affiche :

Pour les e-mails v1.0 existants qui utilisaient le modèle (précédemment v1.0) :\
**Courrier électronique**  v1.0 approuvé - Un brouillon v2.0 sera créé pour ce courrier électronique, tout en utilisant le nouveau modèle v2.0 approuvé. Il recevra également toute modification de modèle.\
**Version préliminaire de courrier électronique**  v1.0 - Le brouillon restera dans la version 1.0 jusqu’à ce que vous cliquiez sur &quot;Modifier le brouillon&quot;. Ensuite, il sera automatiquement marqué comme v2.0 et recevra les modifications de modèle.\
**Approuvé avec un brouillon de courrier électronique**  v1.0 - Le brouillon restera dans la version 1.0 jusqu’à ce que vous cliquiez sur &quot;Modifier le brouillon&quot;. Ensuite, il sera automatiquement marqué comme v2.0 et recevra les modifications de modèle.

Pour les e-mails v2.0 existants qui utilisaient le modèle (précédemment v1.0) :\
**Courrier électronique**  v2.0 approuvé - Un brouillon v2.0 sera créé pour ce courrier électronique, tout en &quot;utilisant&quot; le modèle nouvellement approuvé, et recevra toute modification de modèle.\
**Version préliminaire v2.0 - Courriel**  - Le brouillon restera tel quel (v2.0) et recevra toute modification de modèle.\
**Approuvé avec le brouillon de la version v2.0 par courrier électronique**  - Le brouillon restera tel quel (v2.0) et recevra tout changement de modèle.

>[!CAUTION]
>
>Si vous approuvez un brouillon v2.0 d’un modèle de courrier électronique v1.0, le modèle deviendra v2.0. **il n’est pas possible de rétablir** le modèle en v1.0.

Éléments à noter

* Les e-mails approuvés sont **jamais** modifiés.

* Les modèles de courrier électronique approuvés sont **jamais** modifiés.

* Dans quelques cas **rares**, un e-mail v1.0 ne peut pas être ouvert dans l&#39;éditeur de messagerie 2.0. Si cela se produit, ignorez le brouillon et contactez l&#39;assistance marketing.

>[!MORELIKETHIS]
>
>* [Présentation de l’éditeur de courrier électronique 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Syntaxe du modèle de courriel](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)

