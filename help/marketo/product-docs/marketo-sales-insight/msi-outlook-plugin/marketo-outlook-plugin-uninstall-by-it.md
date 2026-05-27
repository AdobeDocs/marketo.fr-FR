---
unique-page-id: 11382829
description: Découvrez comment le service informatique peut désinstaller le plug-in Marketo Outlook. Supprimez le complément des ordinateurs des utilisateurs, si nécessaire.
title: Désinstallation du plug [!DNL Outlook] in Marketo par le service informatique
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/p2CjKHycrJRHLpphyn2qsUEKP-dWh2OlTezwrOn9Ljw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
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

Veuillez consulter la liste complète des commutateurs de [](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) si vous souhaitez essayer différents niveaux de journalisation ou d&#39;interface utilisateur.
