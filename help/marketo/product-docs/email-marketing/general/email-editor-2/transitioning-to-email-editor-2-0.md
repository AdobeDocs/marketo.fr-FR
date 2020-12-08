---
unique-page-id: 11373011
description: Passage à la version 2.0 de l’éditeur de courrier électronique - Documentation du marketing - Documentation du produit
title: Transition vers l’éditeur de messagerie 2.0
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---


# Transition vers l’éditeur de messagerie 2.0 {#transitioning-to-email-editor}

Depuis la version [du](../../../../release-notes/2016/release-notes-spring-16.md)19 juin 2010, tous les abonnements de Marketo ont été convertis en Éditeur de courriel 2.0. [En savoir plus](https://nation.marketo.com/docs/DOC-7038) sur l&#39;obsolescence de l&#39;Éditeur de courriel 1.0.

Les courriers électroniques et les modèles de courrier électronique de votre abonnement doivent avoir un numéro de version. La version se trouve dans la page de résumé du fichier.

![](assets/five-5.png)

Par défaut, tous vos e-mails et modèles de courrier électronique existants seront marqués comme v1.0 s’ils ont été créés avant la version du printemps 16 ou après la version lorsque l’éditeur de courrier électronique 2.0 est désactivé. L’éditeur de messagerie 2.0 étant désormais automatiquement activé, le comportement suivant s’affiche :

* Lorsque vous créez un courriel, le sélecteur [de modèles de](email-template-picker-overview.md) courriel s’affiche et vous pouvez choisir un modèle de courriel v2.0.
* Chaque fois que vous créez ou modifiez un courrier électronique à l’aide de la version 2.0 de l’Editeur de messagerie, le courrier électronique qui en résulte est **toujours** marqué comme v2.0 (même si vous avez utilisé un modèle de courrier électronique de la version 1.0).

Si votre abonnement contient des courriers électroniques de la version 1.0 avant le passage à la version 2.0 de l’éditeur de messagerie, vous constaterez le comportement suivant en fonction de l’état actuel de la ressource :

**Approuvé** - Cliquez sur &quot;Modifier le brouillon&quot; pour créer un brouillon v2.0 du courrier électronique approuvé. Si vous approuvez ensuite le brouillon v2.0, l’état approuvé du courrier électronique devient v2.0 et il n’est pas possible de revenir à la version 1.0.\
**Version préliminaire** - Le fait de cliquer sur &quot;Modifier le brouillon&quot; marquera automatiquement ce brouillon comme v2.0. À ce stade, il ne sera pas possible de supprimer et de revenir à la version 1.0 car il n&#39;existe pas de version approuvée de la ressource.\
**Approuvé avec brouillon** - Cliquez sur &quot;Modifier le brouillon&quot; pour marquer automatiquement ce brouillon comme v2.0. De ce fait, il n&#39;y a aucun moyen de rétablir le brouillon à v1.0.

Si votre abonnement dispose de modèles de courrier électronique v1.0 avant de passer à la version 2.0 de l’Editeur de messagerie, vous allez connaître le comportement suivant :

**Approuvé** - Cliquez sur &quot;Modifier le brouillon&quot; pour créer un brouillon v2.0 du modèle de courrier électronique existant.\
**Version préliminaire** - Le fait de cliquer sur &quot;Modifier le brouillon&quot; marquera automatiquement ce brouillon comme v2.0. À ce stade, il ne sera pas possible de supprimer et de revenir à la version 1.0 car il n’existe pas de version approuvée de la ressource.\
**Approuvé avec brouillon** - Le fait de cliquer sur &quot;Modifier le brouillon&quot; marquera automatiquement ce brouillon comme v2.0. De ce fait, il n&#39;y a aucun moyen de rétablir le brouillon à v1.0.

Si vous approuvez un modèle de courrier électronique qui était précédemment v1.0 (dans l’un des états ci-dessus), le comportement suivant s’affiche :

Pour les e-mails v1.0 existants qui utilisaient le modèle (précédemment v1.0) :\
**Courrier électronique** v1.0 approuvé - Un brouillon v2.0 sera créé pour ce courrier électronique, tout en utilisant le nouveau modèle v2.0 approuvé. Il recevra également toute modification de modèle.\
**Version préliminaire de courrier électronique** v1.0 : le brouillon restera dans la version 1.0 jusqu’à ce que vous cliquiez sur &quot;Modifier le brouillon&quot;. Ensuite, il sera automatiquement marqué comme v2.0 et recevra les modifications de modèle.\
**Approuvé avec le brouillon de la version 1.0 par courrier électronique** - Le brouillon restera dans la version 1.0 jusqu’à ce que vous cliquiez sur &quot;Modifier le brouillon&quot;. Ensuite, il sera automatiquement marqué comme v2.0 et recevra les modifications de modèle.

Pour les e-mails v2.0 existants qui utilisaient le modèle (précédemment v1.0) :\
**Courrier électronique** v2.0 approuvé - Un brouillon v2.0 sera créé pour ce courrier électronique, tout en &quot;utilisant&quot; le modèle nouvellement approuvé, et recevra toute modification de modèle.\
**Version préliminaire de courrier électronique** v2.0 : le brouillon restera tel quel (v2.0) et recevra toute modification de modèle.\
**Approuvé avec le brouillon de la version v2.0 par courrier électronique** - Le brouillon restera tel quel (v2.0) et recevra tout changement de modèle.

>[!CAUTION]
>
>Si vous approuvez un brouillon v2.0 d’un modèle de courrier électronique v1.0, le modèle deviendra v2.0. Il **n’est pas possible** de le rétablir dans v1.0.

Éléments à noter

* Les courriels approuvés **ne sont jamais** modifiés.

* Les modèles de courrier électronique approuvés **ne sont jamais** modifiés.

* Dans quelques **rares** cas, un courrier électronique v1.0 ne peut pas être ouvert dans l’éditeur de courrier électronique 2.0. Si cela se produit, ignorez le brouillon et contactez l’assistance marketing.

>[!NOTE]
>
>**Articles connexes**
>
>* [Présentation de l’éditeur de courrier électronique 2.0](email-editor-v2-0-overview.md)
>* [Syntaxe du modèle de courriel](email-template-syntax.md)

>



