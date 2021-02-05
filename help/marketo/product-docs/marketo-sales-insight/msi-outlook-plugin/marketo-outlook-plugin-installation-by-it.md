---
unique-page-id: 11382815
description: Installation du module externe Marketo Outlook par le service informatique - Docs Marketo - Documentation du produit
title: Installation du module externe Marketo Outlook par le service informatique
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---


# Installation du module externe Marketo Outlook par IT {#marketo-outlook-plugin-installation-by-it}

Parfois, les stratégies d’entreprise exigent que l’équipe informatique installe tous les logiciels sur les ordinateurs de ses employés. Dans ces cas, le service informatique effectue souvent cette opération à distance en utilisant son propre logiciel de déploiement. Ce document fournit les lignes de commande que vous utiliseriez comme entrées lors du processus de déploiement pour installer à distance le module Outlook.

>[!PREREQUISITES]
>
>[Définissez ](http://docs.marketo.com/display/DOCS/Install+the+Marketo+Add-in+for+Outlook+with+an+Enterprise+Key) la clé d’entreprise.

Exécutez la ligne de commande suivante en tant que &quot;système&quot; ou compte utilisateur administratif avec le commutateur /i à installer.  `<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemple**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Pour le dépannage, vous pouvez activer la journalisation pour créer un fichier journal de sortie.  `<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemple**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Pour spécifier l’emplacement des fichiers journaux, vous pouvez spécifier le chemin d’accès au fichier dans la ligne de commande.  `<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemple**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>L&#39;emplacement d&#39;enregistrement du fichier journal doit exister ou l&#39;installation doit être abandonnée.

Veuillez consulter [la liste complète des commutateurs](https://support.microsoft.com/en-us/kb/227091) de Microsoft si vous souhaitez essayer différents niveaux de journalisation ou niveaux d&#39;interface utilisateur.

>[!MORELIKETHIS]
>
>[Désinstallation du module externe Marketo Outlook par le service informatique](marketo-outlook-plugin-uninstall-by-it.md)

