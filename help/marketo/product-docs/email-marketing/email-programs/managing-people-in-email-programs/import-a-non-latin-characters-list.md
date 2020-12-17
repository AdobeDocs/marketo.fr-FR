---
unique-page-id: 5472678
description: Importer une Liste de caractères non latins - Documents marketing - Documentation du produit
title: Importer une Liste de caractères non latins
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Importer une Liste de caractères non latins {#import-a-non-latin-characters-list}

Vous essayez d&#39;importer un fichier qui n&#39;est pas en anglais ? La liste semble parfaite lorsque vous l&#39;ouvrez avec Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Mais lorsque vous l’importez dans Marketo, vous pouvez constater que les caractères non anglais ne sont pas correctement sélectionnés.

![](assets/image2015-2-10-9-3a35-3a49.png)

En effet, le fichier n’est pas enregistré correctement pour que Marketo reconnaisse tous les caractères non latins. La bonne nouvelle, c&#39;est qu&#39;il y a quelques étapes simples à suivre pour y remédier.

1. Sélectionnez **Enregistrer sous...** dans le menu **Fichier** dans Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Sélectionnez **UTF-16 Unicode Text (.txt)** comme option **Format**. Le fichier sera codé de la façon dont Marketo peut les afficher.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo prend également en charge UTF-8, Shift-JIS ou EUC-JP.

1. Excel enregistre le nouveau fichier sous la forme d&#39;un fichier texte avec l&#39;extension .txt. Mais il convertit également toutes les virgules du fichier en onglets. Nous devons le refaire.

   >[!TIP]
   >
   >Vous pouvez ouvrir le fichier texte à l’aide du Bloc-notes **si vous utilisez Windows ou** TextEdit **si vous utilisez un Mac.**

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Sélectionnez un onglet dans le document et copiez-le.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Sélectionnez **Rechercher et remplacer..** dans le menu **Modifier**.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >L’action équivalente pour les utilisateurs de Windows est : **Modifier > Remplacer...**

1. Collez l’onglet que vous avez copié à l’étape 4 dans la première zone (à remplacer), puis tapez une virgule dans la seconde zone (remplacer par). Cliquez ensuite sur **Tous**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. Et voilà, toutes les virgules sont de retour et nous sommes prêts à rouler.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importez le nouveau fichier dans Marketing et les informations doivent s’afficher correctement cette fois-ci.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Tous les champs Date/Heure importés sont traités comme Heure centrale. Si vous avez des champs Date/Heure dans un fuseau horaire différent, vous pouvez utiliser une formule Excel pour le transformer en Heure centrale (Amérique/Chicago).

Nous savons que c&#39;est bizarre, mais ça marche. Heureuse importation !