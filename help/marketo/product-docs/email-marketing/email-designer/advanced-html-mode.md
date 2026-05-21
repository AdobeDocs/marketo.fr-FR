---
solution: Marketo Engage
product: marketo
title: Modification de modèles d’e-mail à l’aide de l’éditeur HTML avancé
description: Découvrez comment afficher et modifier le code source HTML brut dans le Designer de messagerie Marketo Engage, y compris les mécanismes de sécurisation, les étapes d’accès et les principales limitations.
level: Intermediate
feature: Email Designer
exl-id: b030e56a-de70-4b0d-9788-04a01235cffb
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Modification de modèles d’e-mail à l’aide de l’éditeur HTML avancé {#advanced-html-mode}

Le mode HTML avancé vous permet d’afficher et de modifier le code source brut des modèles d’e-mail directement depuis l’interface de Designer d’e-mail [!DNL Marketo Engage].

Cette fonctionnalité vous permet d’insérer des expressions avancées directement dans la source. Lorsque vous revenez à la vue visuelle (Bureau), le contenu est rendu à nouveau afin que vous puissiez vérifier son aspect et continuer à le modifier dans l’une ou l’autre des vues.

## Mécanismes de sécurisation {#guardrails}

Lorsque vous utilisez l’éditeur HTML avancé, les mécanismes de sécurisation suivants protègent la compatibilité du contenu et définissent les attentes.

* L’éditeur HTML avancé **ne valide pas** votre code. Il ne vérifie pas les erreurs de syntaxe ou les mises en page rompues. Examinez attentivement votre contenu avant d’enregistrer.

* Les futures mises à jour du système peuvent remplacer les modifications apportées aux balises par défaut. **Vos modifications peuvent ne pas persister**.

* Prise en charge de [!DNL Adobe] **impossible de résoudre les problèmes** causés par le code personnalisé et les modifications manuelles. Conservez une sauvegarde de votre contenu au cas où vous auriez besoin d’effectuer une restauration.

* Vous ne pouvez pas simuler le contenu dans la vue HTML avancée. Basculez vers la vue Bureau pour prévisualiser votre contenu.

* Pour garantir la compatibilité du contenu, **vous ne pouvez pas enregistrer** dans la vue HTML avancée. Revenez à la vue Bureau lorsque vous êtes prêt à enregistrer vos modifications.

## Accès au mode HTML avancé {#access-html-mode}

Pour ouvrir l’éditeur HTML avancé et modifier la source du modèle, procédez comme suit.

1. Ouvrez ou [créez un modèle d’e-mail](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template) dans le Designer d’e-mail.

1. Dans l’écran _Modifier le modèle d’e-mail_, cliquez sur le bouton HTML dans le coin supérieur droit.

   ![](assets/advanced-html-mode-1.png){width="800" zoomable="yes"}

1. Lors de la première ouverture de l’éditeur HTML avancé, un message d’avertissement s’affiche. Cliquez sur **[!UICONTROL OK]** lorsque vous avez terminé.

   ![](assets/advanced-html-mode-2.png)

   >[!NOTE]
   >
   >Cet avertissement s’affiche la première fois que vous ouvrez l’éditeur HTML avancé et se réinitialise chaque mois.

1. L’éditeur HTML avancé s’affiche.

   ![](assets/advanced-html-mode-3.png){width="800" zoomable="yes"}

1. Ajoutez les modifications souhaitées au contenu de votre e-mail.

   >[!WARNING]
   >
   >Veillez à saisir le code HTML et CSS correct, car il n’existe aucun processus de validation de la syntaxe et la prise en charge d’Adobe ne peut pas vous aider à effectuer les modifications dans HTML.

1. La simulation et l’enregistrement de contenu ne sont pas disponibles dans la vue HTML avancée pour des raisons de compatibilité. Revenez à la vue Bureau pour prévisualiser votre contenu et enregistrer vos modifications.

   ![](assets/advanced-html-mode-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Vos modifications sont conservées lorsque vous changez de vue.
