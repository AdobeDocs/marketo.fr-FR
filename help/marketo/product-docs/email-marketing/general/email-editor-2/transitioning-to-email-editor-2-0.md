---
unique-page-id: 11373011
description: Transition vers Email Editor 2.0 - Documents Marketo - Documentation du produit
title: Transition vers l’éditeur d’e-mail 2.0
exl-id: eb9ec8cc-d6e8-4839-a4d9-608d2f264cbb
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: b3bc6a7ec14a513e4b294852d066f9e3d0f74ef8
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 0%

---

# Transition vers l’éditeur d’e-mail 2.0 {#transitioning-to-email-editor}

Depuis la version du 19 juin, tous les abonnements Marketo ont été transférés vers l’éditeur d’e-mail 2.0. [En savoir plus](https://nation.marketo.com/docs/DOC-7038) sur l’obsolescence de l’éditeur d’e-mail 1.0.

Les e-mails et les modèles d’e-mail de votre abonnement doivent avoir un numéro de version. La version se trouve dans la page de résumé de la ressource.

![](assets/five-5.png)

Par défaut, tous vos e-mails et modèles d’e-mail existants seront marqués comme v1.0 s’ils ont été créés avant la version du printemps 16 ou après la version lorsque l’éditeur d’e-mail 2.0 est désactivé. Avec l’éditeur d’e-mail 2.0 désormais automatiquement activé, le comportement suivant s’affiche :

* Lorsque vous créez un e-mail, le [sélecteur de modèle d’e-mail](email-template-picker-overview.md) s’affiche et vous pouvez choisir un modèle d’e-mail v2.0.
* Chaque fois que vous créez ou modifiez un e-mail avec l’éditeur d’e-mail 2.0, l’e-mail qui en résulte **toujours** est marqué comme v2.0 (même si vous avez utilisé un modèle d’e-mail v1.0).

Si votre abonnement comporte des e-mails v1.0 avant de passer à l’éditeur d’e-mail 2.0, vous constaterez le comportement suivant en fonction de l’état actuel de la ressource :

**Approuvé** - Cliquez sur « Modifier le brouillon » pour créer un brouillon v2.0 de l’e-mail approuvé. Si vous approuvez ensuite le brouillon v2.0, l’état approuvé de l’e-mail devient v2.0 et il n’est pas possible de revenir à la v1.0.\
**Brouillon** - Cliquez sur « Modifier le brouillon » pour marquer automatiquement ce brouillon comme v2.0. À ce stade, il ne sera pas possible de supprimer et de revenir à la version 1.0, car il n’existe aucune version approuvée de la ressource.
**Approuvé avec le brouillon** - Cliquez sur « Modifier le brouillon » pour marquer automatiquement ce brouillon comme v2.0. Pour cette raison, il n’est pas non plus possible de rétablir le brouillon vers la version 1.0.

Si votre abonnement comporte des modèles d’e-mail v1.0 avant de passer à l’éditeur d’e-mail 2.0, le comportement suivant se produira :

**Approuvé** - Cliquez sur « Modifier le brouillon » pour créer un brouillon v2.0 du modèle d’e-mail existant.
**Brouillon** - Cliquez sur « Modifier le brouillon » pour marquer automatiquement ce brouillon comme v2.0. À ce stade, il ne serait pas possible d’annuler et de revenir à la version 1.0, car il n’existe aucune version approuvée de la ressource.
**Approuvé avec le brouillon** - Cliquez sur « Modifier le brouillon » pour marquer automatiquement ce brouillon comme v2.0. Pour cette raison, il n’est pas non plus possible de rétablir le brouillon vers la version 1.0.

Si vous approuvez un modèle d’e-mail qui était auparavant version 1.0 (dans l’un des états ci-dessus), le comportement suivant s’affiche :

Pour les e-mails existants de la version 1.0 qui utilisaient le modèle (anciennement v1.0) :\
**E-mail v1.0 approuvé** - Un brouillon v2.0 sera créé pour cet e-mail, en utilisant toujours le modèle v2.0 nouvellement approuvé. Il recevra également toutes les modifications apportées au modèle.\
**E-mail brouillon v1.0** - Le brouillon reste v1.0 jusqu’à ce que vous cliquiez sur « Modifier le brouillon ». Ensuite, il sera automatiquement marqué comme v2.0 et recevra toutes les modifications du modèle.\
**Approuvé avec l’e-mail Brouillon v1.0** - Le brouillon reste dans la version 1.0 jusqu’à ce que vous cliquiez sur « Modifier le brouillon ». Ensuite, il sera automatiquement marqué comme v2.0 et recevra toutes les modifications du modèle.

Pour les e-mails v2.0 existants qui utilisaient le modèle (anciennement v1.0) :\
**E-mail v2.0 approuvé** - Un brouillon v2.0 sera créé pour cet e-mail, en « utilisant » toujours le modèle nouvellement approuvé, et recevra toutes les modifications du modèle.\
**E-mail brouillon v2.0** - Le brouillon reste tel quel (v2.0) et reçoit toutes les modifications du modèle.\
**Approuvé avec l’e-mail Draft v2.0** - Le brouillon reste tel quel (v2.0) et reçoit les modifications du modèle.

>[!CAUTION]
>
>Si vous approuvez le brouillon v2.0 d’un modèle d’e-mail v1.0, le modèle devient v2.0. Il n’est **pas possible** de le rétablir dans la version 1.0.

Éléments à noter

* Les e-mails approuvés ne sont **jamais** modifiés.

* Les modèles d’e-mail approuvés ne sont **jamais** modifiés.

* Dans certains **rares**, un e-mail v1.0 ne peut pas être ouvert dans l’éditeur d’e-mail 2.0. Si cela se produit, ignorez le brouillon et contactez l’assistance Marketo.

>[!MORELIKETHIS]
>
>* [Présentation de l’éditeur d’e-mail 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Syntaxe du modèle d&#39;e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)
