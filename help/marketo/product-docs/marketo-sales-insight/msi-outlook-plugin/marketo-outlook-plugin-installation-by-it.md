---
unique-page-id: 11382815
description: Installation du plug [!DNL Outlook] in Marketo par le service informatique - Documents Marketo - Documentation du produit
title: Installation du plug [!DNL Outlook] in Marketo par le service informatique
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 1%

---

# Installation du plug-in Marketo [!DNL Outlook] par le service informatique {#marketo-outlook-plugin-installation-by-it}

Parfois, les stratégies d&#39;entreprise exigent que leur équipe informatique installe tous les logiciels sur les ordinateurs de leurs employés. Dans ces cas, le service informatique effectue souvent cette opération à distance à l’aide de son propre logiciel de déploiement. Ce document fournit les lignes de commande que vous utiliserez comme entrées pendant le processus de déploiement pour installer à distance le plug-in Outlook.

>[!PREREQUISITES]
>
>[Configurer](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) la clé d’entreprise.

Exécutez la ligne de commande suivante en tant que « Système » ou compte utilisateur d’administration avec le commutateur /i à installer.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

À des fins de dépannage, vous pouvez activer la journalisation pour créer un fichier journal de sortie.

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Pour spécifier l’emplacement des fichiers journaux, vous pouvez spécifier le chemin d’accès au fichier dans la ligne de commande.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>L&#39;emplacement de stockage du fichier journal doit exister ou l&#39;installation sera abandonnée.

Veuillez consulter la liste complète des commutateurs de [Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) si vous souhaitez essayer différents niveaux de journalisation ou d&#39;interface utilisateur.

>[!MORELIKETHIS]
>
>[Désinstallation du plug [!DNL Outlook] in Marketo par le service informatique](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
