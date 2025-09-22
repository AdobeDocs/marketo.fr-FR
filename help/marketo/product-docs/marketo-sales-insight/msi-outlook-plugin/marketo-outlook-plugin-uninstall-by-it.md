---
unique-page-id: 11382829
description: Désinstallation du plug [!DNL Outlook] in Marketo par le service informatique - Documents Marketo - Documentation du produit
title: Désinstallation du plug [!DNL Outlook] in Marketo par le service informatique
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 2%

---

# Désinstallation du plug-in Marketo [!DNL Outlook] par le service informatique {#marketo-outlook-plugin-uninstall-by-it}

Voici comment le service informatique peut désinstaller le plug-in Marketo [!DNL Outlook] à distance.

Exécutez la ligne de commande suivante en tant que « Système » ou un compte utilisateur d’administration avec le commutateur /x à désinstaller.

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

À des fins de dépannage, vous pouvez activer la journalisation pour créer un fichier journal de sortie.

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Pour spécifier l’emplacement des fichiers journaux, vous pouvez spécifier le chemin d’accès au fichier dans la ligne de commande.

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemple**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>La désinstallation à distance du plug-in entraîne la fermeture forcée des [!DNL Outlook] sur l’ordinateur de l’utilisateur.

Veuillez consulter la liste complète des commutateurs de [Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) si vous souhaitez essayer différents niveaux de journalisation ou d&#39;interface utilisateur.
