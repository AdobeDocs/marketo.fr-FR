---
unique-page-id: 11382535
description: Utilisation d’URL dans mes jetons - Documents Marketo - Documentation du produit
title: Utilisation d’URL dans mes jetons
exl-id: 6830c621-4d94-4f31-a608-2f7b2aced88c
feature: Tokens
source-git-commit: 165dca2573f340ede147866c3a30707bbfb6857c
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Utilisation d’URL dans mes jetons {#using-urls-in-my-tokens}

Suivez les étapes ci-dessous pour utiliser Mes jetons afin d’insérer des URL dans vos e-mails.

1. Sélectionnez votre programme et cliquez sur **Mes jetons**.

   ![](assets/one-4.png)

1. Sélectionnez le **Texte** Mon jeton, faites-le glisser et déposez-le sur la zone de travail.

   ![](assets/two-4.png)

1. Attribuez un nom unique au jeton, saisissez une URL (sans le champ https://) et cliquez sur **Enregistrer**.

   ![](assets/three-4.png)

   >[!CAUTION]
   >
   >**Utilisation de http/https...**
   >
   >* Pour vous assurer que les clics sont suivis dans votre e-mail, ne saisissez **pas** https:// _à l’intérieur_ la valeur du jeton. Utilisez-le en dehors du jeton, comme indiqué à l’étape 7.
   >
   >* Nous vous recommandons vivement de ne pas exclure le http/https. Si vous le faites, la [version web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} de votre e-mail risque de s’afficher incorrectement.

1. Sélectionnez l’e-mail dans votre programme.

   ![](assets/four-3.png)

1. Cliquez sur **Modifier le brouillon**.

   ![](assets/five-3.png)

1. Double-cliquez dans la zone de texte pour modifier.

   ![](assets/six-1.png)

1. N’importe où dans votre e-mail, saisissez `https://` (sans laisser d’espace après), puis cliquez sur l’icône Insérer un jeton .

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Vous avez bien sûr également la possibilité de saisir des `http://` si votre site n’utilise pas https.

1. Recherchez votre jeton Mon jeton, sélectionnez-le, puis cliquez sur **Insérer**.

   ![](assets/eight.png)

1. Mettez en surbrillance le jeton https:// et , puis appuyez sur Ctrl/Cmd+X (Ctrl = Windows/Cmd = Mac) pour couper le texte.

   ![](assets/nine.png)

1. Mettez en surbrillance le texte que le lien doit afficher et cliquez sur l’icône Insérer/Modifier le lien .

   ![](assets/ten.png)

1. Appuyez sur Ctrl/Cmd+V pour coller le contenu dans la zone **URL**, puis cliquez sur **Insérer**.

   ![](assets/eleven.png)

1. Cliquez sur **Enregistrer**.

   ![](assets/twelve.png)

   Et c&#39;est fini ! Votre URL sera renseignée après l’envoi, et grâce à votre placement de https:// devant le jeton, un lien trackable sera généré.
