---
unique-page-id: 5472678
description: Importation d’une liste de caractères non latins - Documents Marketo - Documentation du produit
title: Importation d’une liste de caractères non latins
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# Importation d’une liste de caractères non latins {#import-a-non-latin-characters-list}

Vous essayez d&#39;importer un fichier qui n&#39;est pas en anglais ? La liste semble parfaite lorsque vous l’ouvrez avec Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Mais lorsque vous l’importez dans Marketo, il se peut que les caractères non anglais ne soient pas correctement sélectionnés.

![](assets/image2015-2-10-9-3a35-3a49.png)

Cela est dû au fait que le fichier n’est pas enregistré correctement pour que Marketo reconnaisse tous les caractères non latins. La bonne nouvelle, c&#39;est qu&#39;il y a quelques étapes simples que vous pouvez suivre pour y remédier.

1. Sélectionnez **Enregistrer sous...** dans le menu **Fichier** dans Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Choisissez **UTF-16 Unicode Text (.txt)** comme option **Format**. Le fichier sera alors codé de la manière dont Marketo peut les afficher.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo prend également en charge UTF-8, Shift-JIS ou EUC-JP.

1. Excel enregistre le nouveau fichier sous la forme d’un fichier texte avec une extension .txt. Mais il convertit également toutes les virgules du fichier en onglets. Nous devons le refaire.

   >[!TIP]
   >
   >Vous pouvez ouvrir le fichier texte à l’aide de **Notepad** si vous utilisez Windows ou **TextEdit** si vous utilisez un Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Sélectionnez un onglet dans le document et copiez-le.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Sélectionnez **Rechercher et remplacer...** dans le menu **Modifier**.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >L’action équivalente pour les utilisateurs de Windows est : **Modifier > Remplacer...**.

1. Collez l’onglet que vous avez copié à l’étape 4 dans la première zone (à remplacer), puis saisissez une virgule dans la seconde zone (remplacer par). Cliquez ensuite sur **All**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. Et voilà, toutes les virgules sont de retour et nous sommes prêts à rouler.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importez le nouveau fichier dans Marketo et les informations doivent s&#39;afficher correctement cette fois-ci.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Les champs Date/Heure importés sont traités comme heure centrale. Si des champs Date/Heure se trouvent dans un fuseau horaire différent, vous pouvez utiliser une formule Excel pour les transformer en heure normale du Centre (Amérique/Chicago).

Nous savons que c&#39;est bizarre, mais ça marche. Bon import !
