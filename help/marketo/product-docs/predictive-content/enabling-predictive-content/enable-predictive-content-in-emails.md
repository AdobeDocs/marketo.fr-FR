---
unique-page-id: 11385020
description: Activer le contenu prédictif dans les courriels - Documents marketing - Documentation du produit
title: Activer le contenu prédictif dans les courriers électroniques
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Activer le contenu prédictif dans les courriers électroniques {#enable-predictive-content-in-emails}

Créez une ou plusieurs images prédictives dans votre message électronique, en adaptant l’expérience à chaque destinataire.

>[!NOTE]
>
>Il est recommandé d’activer plus de cinq éléments de contenu par catégorie et par source (courriel, média enrichi, barre) avant de tester et d’utiliser le contenu prédictif. Plus de contenu vous donne un meilleur résultat prédictif.

>[!PREREQUISITES]
>
>Avant d’activer le contenu prédictif. vous devez :
>
>* [Préparation du contenu prédictif](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md)
>* [Approbation d’un titre pour le contenu prédictif](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Ajouter du contenu prédictif à l’aide de l’éditeur Email 2.0 {#adding-predictive-content-using-the-email-editor}

1. Cliquez sur Activités **** marketing.

   ![](assets/one.png)

1. Sélectionnez votre adresse électronique et cliquez sur **Modifier le brouillon**.

   ![](assets/two.png)

1. Cliquez sur l’image à rendre prédictive. Lorsque l’icône représentant un engrenage apparaît, cliquez dessus et sélectionnez **Activer le contenu`AI`** (le contenu`AI` est l’ancien nom du contenu prédictif).

   ![](assets/three.png)

1. Pour sélectionner une ou plusieurs catégories, cliquez sur la liste déroulante **Catégories** , effectuez votre sélection, puis cliquez sur **Appliquer**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Le choix de catégories spécifiques ou la modification de la disposition prédictive est facultatif.

1. Votre image est maintenant prédictive. Répétez les étapes 3 et 4 pour d’autres images (si nécessaire).

   ![](assets/five.png)

1. Pour prévisualisation de votre courrier électronique, cliquez sur **Prévisualisation** dans le coin supérieur droit.

   ![](assets/six.png)

1. Pour vue d’autres images possibles, cliquez sur **Actualiser**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >L’image n’est pas sélectionnée **_tant que le destinataire n’a pas ouvert le courrier électronique_**. Ce que vous voyez dans la prévisualisation n&#39;est qu&#39;un exemple, et ne sera pas nécessairement l&#39;image que voit le destinataire.

1. Une fois que vous avez terminé de prévisualiser votre courrier électronique, cliquez sur la liste déroulante Actions **de** Prévisualisation et sélectionnez **Approuver et fermer**. Si vous avez encore des modifications à effectuer, cliquez sur **Modifier le brouillon** sur la droite.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Lors de l’envoi d’un échantillon, une image aléatoire est sélectionnée.

Une fois votre e-mail approuvé, il sera équipé de Contenu Prédictif et prêt à être envoyé !

>[!CAUTION]
>
>Lorsqu’un destinataire ouvre le courrier électronique, les images prédictives sont verrouillées. Si le contenu est supprimé par la suite, les destinataires verront une image rompue où se trouvait le contenu.

## Ajouter du contenu prédictif lorsque vous n’utilisez pas l’éditeur Email 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Si vous n’utilisez pas de modèle [E-mail 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) , il est possible d’ajouter du contenu prédictif à votre courriel simplement en balisant une image de votre modèle en tant qu’élément d’image modifiable du marketing.

Découvrez la syntaxe spécifique au [marketing ici](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements).

Voici un exemple de ce à quoi devrait ressembler le code (il s&#39;agit seulement d&#39;un exemple, ne copiez pas exactement le code ci-dessous).

**Exemple**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="http://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
