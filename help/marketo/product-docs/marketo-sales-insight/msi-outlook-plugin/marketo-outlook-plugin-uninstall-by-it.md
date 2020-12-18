---
unique-page-id: 11382829
description: Désinstallation du module externe Marketo Outlook par le service informatique - Documentation du marketing - Documentation du produit
title: Désinstallation du module externe Marketo Outlook par le service informatique
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Désinstallation du module externe Marketo Outlook par le service informatique {#marketo-outlook-plugin-uninstall-by-it}

Voici comment le service informatique peut désinstaller le module externe Marketo Outlook à distance.

Exécutez la ligne de commande suivante en tant que &quot;Système&quot; ou compte utilisateur administratif avec le commutateur /x pour désinstaller.
`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Exemple**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Pour le dépannage, vous pouvez activer la journalisation pour créer un fichier journal de sortie.  `<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemple**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Pour spécifier l’emplacement des fichiers journaux, vous pouvez spécifier le chemin d’accès au fichier dans la ligne de commande.  `<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemple**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>La désinstallation du module externe à distance entraîne la fermeture forcée d&#39;Outlook sur l&#39;ordinateur de l&#39;utilisateur.

Veuillez consulter [la liste complète des commutateurs](https://support.microsoft.com/en-us/kb/227091) de Microsoft si vous souhaitez essayer différents niveaux de journalisation ou niveaux d&#39;interface utilisateur.