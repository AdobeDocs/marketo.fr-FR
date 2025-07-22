---
unique-page-id: 11385020
description: Activer le contenu prédictif dans les e-mails - Documents Marketo - Documentation du produit
title: Activer le contenu prédictif dans les e-mails
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Activer le contenu prédictif dans les e-mails {#enable-predictive-content-in-emails}

Rendez une ou plusieurs images de votre e-mail prédictives, en adaptant l’expérience de chaque destinataire.

>[!NOTE]
>
>Il est recommandé d’activer plus de cinq éléments de contenu par catégorie et par source (e-mail, média enrichi, barre) avant de tester et d’utiliser le contenu prédictif. Plus de contenu vous donne un meilleur résultat prédictif.

>[!PREREQUISITES]
>
>Avant d’activer le contenu prédictif, vous devez :
>
>* **Préparation de votre contenu prédictif**
>
>   * [Modifier le contenu prédictif des e-mails](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"} ou
>   * [Modification du contenu prédictif pour les médias riches](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"} ou
>   * [Modifier le contenu prédictif de la barre de recommandations](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [Approuver un titre pour le contenu prédictif](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

## Ajout de contenu prédictif à l’aide de l’éditeur d’email 2.0 {#adding-predictive-content-using-the-email-editor}

1. Cliquez sur **[!UICONTROL Activités marketing]**.

   ![](assets/one.png)

1. Sélectionnez votre e-mail et cliquez sur **[!UICONTROL Modifier le brouillon]**.

   ![](assets/two.png)

1. Cliquez sur l’image à rendre prédictive. Lorsque l’icône en forme d’engrenage s’affiche, cliquez dessus et sélectionnez **[!UICONTROL Activer ContentAI]** (ContentAI est l’ancien nom du contenu prédictif).

   ![](assets/three.png)

1. Pour sélectionner une ou plusieurs catégories, cliquez sur le menu déroulant **[!UICONTROL Catégories]**, effectuez votre ou vos sélection(s), puis cliquez sur **[!UICONTROL Appliquer]**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Le choix de catégories spécifiques ou la modification de la mise en page prédictive est facultatif.

1. Votre image est maintenant prédictive. Répétez les étapes 3 et 4 pour obtenir des images supplémentaires (si vous le souhaitez).

   ![](assets/five.png)

1. Pour prévisualiser votre e-mail, cliquez sur **[!UICONTROL Aperçu]** dans le coin supérieur droit.

   ![](assets/six.png)

1. Pour afficher les différentes images possibles, cliquez sur **[!UICONTROL Actualiser]**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >L’image n’est pas sélectionnée **_tant que le destinataire n’a pas ouvert l’email_**. Ainsi, ce que vous voyez dans l’aperçu n’est qu’un exemple et ne sera pas nécessairement l’image que le destinataire voit.

1. Une fois la prévisualisation de l’e-mail terminée, cliquez sur le menu déroulant **[!UICONTROL Prévisualiser les actions]** et sélectionnez **[!UICONTROL Approuver et fermer]**. Ou, s’il vous reste des modifications à effectuer, cliquez sur **[!UICONTROL Modifier le brouillon]** à droite.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Lors de l’envoi d’un échantillon, une image aléatoire est sélectionnée.

Une fois que vous avez approuvé votre e-mail, il sera doté de contenu prédictif et prêt à être envoyé.

>[!CAUTION]
>
>Une fois qu’un destinataire ouvre l’e-mail, les images prédictives sont verrouillées. Si le contenu est supprimé ultérieurement, les destinataires verront une image endommagée là où le contenu se trouvait.

## Ajout de contenu prédictif lorsque vous n’utilisez pas l’éditeur d’email 2.0 {#adding-predictive-content-when-not-using-the-email-editor}

Si vous n’utilisez pas de modèle [Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md){target="_blank"}, il est possible d’ajouter du contenu prédictif à votre e-mail en balisant simplement une image de votre modèle en tant qu’élément d’image modifiable Marketo.

Découvrez la syntaxe spécifique à [Marketo ici](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target="_blank"}.

Voici un exemple de ce à quoi le code doit ressembler (il s’agit uniquement d’un exemple, ne copiez pas exactement le code ci-dessous).

**Exemple**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
