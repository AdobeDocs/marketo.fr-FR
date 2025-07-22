---
unique-page-id: 5472678
description: Importer une liste de caractères non latins - Documents Marketo - Documentation du produit
title: Importer une liste de caractères non latins
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Importer une liste de caractères non latins {#import-a-non-latin-characters-list}

Vous essayez d&#39;importer un fichier qui n&#39;est pas en anglais ? La liste s’affiche parfaitement lorsque vous l’ouvrez avec Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Cependant, lorsque vous l’importez dans Marketo, il se peut que les caractères non anglais ne soient pas correctement récupérés.

![](assets/image2015-2-10-9-3a35-3a49.png)

En effet, le fichier n’est pas enregistré correctement pour que Marketo puisse reconnaître tous les caractères non latins. La bonne nouvelle est qu’il existe quelques étapes simples que vous pouvez suivre pour résoudre le problème.

1. Sélectionnez **[!UICONTROL Enregistrer sous]...** dans le menu **[!UICONTROL Fichier]** d’Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Choisissez **[!UICONTROL Texte Unicode UTF-16 (.txt)]** comme option **[!UICONTROL Format]**. Cela encode le fichier de la manière dont Marketo peut les afficher.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo prend également en charge UTF-8, Shift-JIS ou EUC-JP.

1. Excel enregistre le nouveau fichier en tant que fichier texte avec une extension .txt. Mais elle convertit également toutes les virgules du fichier en onglets. Nous devons le changer à nouveau.

   >[!TIP]
   >
   >Vous pouvez ouvrir le fichier texte en utilisant **[!DNL Notepad]** si vous utilisez Windows ou **[!DNL TextEdit]** si vous utilisez un Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Sélectionnez un onglet dans le document et copiez-le.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Sélectionnez **[!UICONTROL Rechercher et remplacer]...** dans le menu **[!UICONTROL Modifier]**.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >L’action équivalente pour les utilisateurs de Windows est : **[!UICONTROL Modifier] > [!UICONTROL Remplacer]...**

1. Collez l’onglet que vous avez copié à l’étape 4 dans la première zone (à remplacer), puis saisissez une virgule dans la seconde zone (à remplacer par). Cliquez ensuite sur **[!UICONTROL Tout]**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. Et voilà, toutes les virgules sont de retour et nous sommes prêts à rouler.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importez le nouveau fichier dans Marketo et cette fois, les informations doivent s’afficher correctement.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Tous les champs de date et d’heure importés sont traités comme des champs d’heure centrale. Si vous avez des champs date/heure dans un fuseau horaire différent, vous pouvez utiliser une formule Excel pour les transformer en Heure du Centre (Amérique/Chicago).

On sait que c&#39;est bizarre, mais ça marche. Bonne importation !
