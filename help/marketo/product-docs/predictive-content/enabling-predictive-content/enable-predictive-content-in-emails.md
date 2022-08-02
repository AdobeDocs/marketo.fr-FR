---
unique-page-id: 11385020
description: Activation du contenu prédictif dans les emails - Documents Marketo - Documentation du produit
title: Activation du contenu prédictif dans les emails
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Activation du contenu prédictif dans les emails {#enable-predictive-content-in-emails}

Effectuez une ou plusieurs images dans la prédiction de votre email, en adaptant l&#39;expérience à chaque destinataire.

>[!NOTE]
>
>Il est recommandé d’activer plus de cinq éléments de contenu par catégorie et par source (email, média enrichi, barre) avant de tester et d’utiliser du contenu prédictif. Plus de contenu vous donne un meilleur résultat prédictif.

>[!PREREQUISITES]
>
>Avant d’activer le contenu prédictif, vous devez :
>
>* **Préparation de votre contenu prédictif**
   >
   >   * [Modifier le contenu prédictif pour les emails](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target=&quot;_blank&quot;} ou
   >   * [Modification du contenu prédictif pour le contenu multimédia enrichi](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target=&quot;_blank&quot;} ou
   >   * [Modifier le contenu prédictif pour la barre de recommandations](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target=&quot;_blank&quot;}
>
>* [Approbation d’un titre pour le contenu prédictif](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target=&quot;_blank&quot;}


## Ajout de contenu prédictif à l’aide de l’éditeur d’email 2.0 {#adding-predictive-content-using-the-email-editor}

1. Cliquez sur **Activités marketing**.

   ![](assets/one.png)

1. Sélectionnez votre adresse électronique et cliquez sur **Modifier le brouillon**.

   ![](assets/two.png)

1. Cliquez sur l’image que vous souhaitez rendre prédictive. Lorsque l’icône d’engrenage s’affiche, cliquez dessus et sélectionnez **Activation de ContentAI** (ContentAI est l’ancien nom de contenu prédictif).

   ![](assets/three.png)

1. Pour sélectionner une ou plusieurs catégories, cliquez sur le bouton **Catégories** , effectuez votre ou vos sélections, puis cliquez sur **Appliquer**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Il est facultatif de choisir des catégories spécifiques ou de modifier la disposition prédictive.

1. Votre image est maintenant prédictive. Répétez les étapes 3 et 4 pour d’autres images (si vous le souhaitez).

   ![](assets/five.png)

1. Pour prévisualiser votre email, cliquez sur **Aperçu** dans le coin supérieur droit.

   ![](assets/six.png)

1. Pour afficher d’autres images possibles, cliquez sur **Actualiser**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >L’image n’est pas sélectionnée. **_jusqu&#39;à ce que le destinataire ouvre l&#39;email_**. Donc ce que vous voyez dans l&#39;aperçu est juste un exemple, et ne sera pas nécessairement l&#39;image que le destinataire voit.

1. Une fois l&#39;aperçu de l&#39;email terminé, cliquez sur le bouton **Aperçu des actions** et sélectionnez **Approuver et fermer**. Ou, si vous avez encore des modifications à effectuer, cliquez sur **Modifier le brouillon** à droite.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Lors de l’envoi d’un exemple, une image aléatoire est sélectionnée.

Une fois votre email validé, il sera équipé de contenu prédictif et prêt à être envoyé !

>[!CAUTION]
>
>Une fois qu&#39;un destinataire ouvre l&#39;email, les images prédictives sont verrouillées. Si le contenu est supprimé par la suite, les destinataires verront une image rompue où se trouvait le contenu.

## Ajout de contenu prédictif lorsque vous n’utilisez pas l’éditeur d’email 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Si vous n’utilisez pas un [Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)Le modèle {target=&quot;_blank&quot;}, l’ajout de contenu prédictif à votre email peut être effectué simplement en balisant une image dans votre modèle en tant qu’élément d’image modifiable Marketo.

En savoir plus sur les [Syntaxe spécifique à Marketo ici](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target=&quot;_blank&quot;}.

Voici un exemple de ce à quoi le code doit ressembler (il s’agit uniquement d’un exemple, ne copiez pas exactement le code ci-dessous).

**Exemple**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
