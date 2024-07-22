---
unique-page-id: 11382815
description: Installation du module externe Marketo Outlook par le service informatique - Documents Marketo - Documentation du produit
title: Installation du module externe Marketo Outlook par le service informatique
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 1%

---

# Installation du module externe Marketo Outlook par le service informatique {#marketo-outlook-plugin-installation-by-it}

Parfois, les politiques de l’entreprise exigent que son équipe informatique installe tous les logiciels sur les ordinateurs de ses employés. Dans ce cas, le service informatique effectue souvent cette opération à distance à l’aide de son propre logiciel de déploiement. Ce document fournit les lignes de commande que vous utiliseriez comme entrées lors du processus de déploiement pour installer à distance le module externe Outlook.

>[!PREREQUISITES]
>
>[Configurez](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) la clé d’entreprise.

Exécutez la ligne de commande suivante en tant que compte d’utilisateur &quot;Système&quot; ou administrateur avec le commutateur /i à installer.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Pour le dépannage, vous pouvez activer la journalisation afin de créer un fichier journal de sortie.

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Pour spécifier l’emplacement des fichiers journaux, vous pouvez spécifier le chemin du fichier dans la ligne de commande.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>L’emplacement de stockage du fichier journal doit exister ou l’installation sera abandonnée.

Reportez-vous à la [liste complète des commutateurs](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) de Microsoft si vous souhaitez essayer différents niveaux de journalisation ou niveaux d’interface utilisateur.

>[!MORELIKETHIS]
>
>[Désinstallation du module externe Marketo Outlook par IT](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
