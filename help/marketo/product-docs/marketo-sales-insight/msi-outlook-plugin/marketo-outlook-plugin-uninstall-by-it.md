---
unique-page-id: 11382829
description: Désinstallation du module externe Marketo Outlook par l’informatique - Documents Marketo - Documentation du produit
title: Désinstallation du module externe Marketo Outlook par informatique
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 2%

---

# Désinstallation du module externe Marketo Outlook par informatique {#marketo-outlook-plugin-uninstall-by-it}

Voici comment le service informatique peut désinstaller le module externe Marketo Outlook à distance.

Exécutez la ligne de commande suivante en tant que &quot;Système&quot; ou compte d’utilisateur administrateur avec le commutateur /x à désinstaller.

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Pour la résolution des problèmes, vous pouvez activer la journalisation afin de créer un fichier journal de sortie.

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Pour spécifier l’emplacement des fichiers journaux, vous pouvez spécifier le chemin du fichier dans la ligne de commande.

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>La désinstallation du module externe à distance entraîne la fermeture forcée d’Outlook sur l’ordinateur de l’utilisateur.

Reportez-vous à la liste complète des commutateurs [&#128279;](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) de Microsoft si vous souhaitez essayer différents niveaux de journalisation ou niveaux d’interface utilisateur.
