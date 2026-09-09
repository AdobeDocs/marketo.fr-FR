---
unique-page-id: 4720779
description: Découvrez les dossiers dans les programmes pour organiser des campagnes intelligentes et des ressources. Créer, renommer et supprimer des dossiers.
title: Présentation des dossiers
exl-id: 2ea914f6-ca64-4e87-806c-93beba075ab2
TQID: https://experienceleague.adobe.com/wAE129LK3Pk-CB5SSQqqSV50ng085soYsm4JHfh0CuI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: b77e1a1e72b89e7cdef5733dbb2de4405ebf3b07
workflow-type: tm+mt
source-wordcount: 427
ht-degree: 1%

---

# Compréhension des dossiers {#understanding-folders}

Les dossiers d’un programme peuvent être utilisés pour organiser vos campagnes intelligentes et vos ressources. Elles sont différentes des [dossiers de campagne](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.md).

## Création d’un dossier {#create-a-folder}

1. Accédez à la zone **[!UICONTROL Activités marketing]**.

   ![](assets/ma.png)

1. Cliquez avec le bouton droit sur un programme et sélectionnez **[!UICONTROL Nouveau dossier]**.

   ![](assets/image2015-4-20-18-3a45-3a14.png){width="600" zoomable="yes"}

1. Nommez le nouveau dossier et appuyez sur **[!UICONTROL Entrée]**.

   ![](assets/image2015-4-20-18-3a46-3a57.png){width="600" zoomable="yes"}

Le nouveau dossier est maintenant prêt pour vos ressources locales.

## Renommer un dossier {#rename-a-folder}

1. Cliquez avec le bouton droit sur le dossier et sélectionnez **[!UICONTROL Renommer le dossier]**.

   ![](assets/image2015-4-20-18-3a49-3a10.png){width="600" zoomable="yes"}

1. Saisissez un nouveau nom et appuyez sur **[!UICONTROL Entrée]**.

   ![](assets/image2015-4-20-18-3a52-3a30.png){width="600" zoomable="yes"}

## Suppression d’un dossier {#delete-a-folder}

>[!NOTE]
>
>Assurez-vous que le dossier est vide avant de le supprimer.

1. Cliquez avec le bouton droit sur le dossier et sélectionnez **[!UICONTROL Supprimer le dossier]**.

   ![](assets/image2015-4-20-18-3a55-3a51.png){width="600" zoomable="yes"}

## Archiver un dossier {#archive-a-folder}

Dans Marketo, vous avez la possibilité de convertir des dossiers existants en dossiers d’archives. Les dossiers d’archives existent dans [!UICONTROL Activités marketing], [!UICONTROL Base de données] et [!UICONTROL Design Studio].

![](assets/image2015-4-20-19-3a3-3a46.png){width="600" zoomable="yes"}

Lorsque vous archivez un dossier :

* Le dossier et les ressources ne sont plus visibles dans les résultats de recherche. Si vous recherchez un programme ou un événement situé dans un dossier archivé, les résultats renvoient une vue réduite du dossier archivé
* Les ressources du dossier n’apparaissent plus dans les suggestions automatiques
* Les modèles archivés ne sont pas disponibles lors de la création d’un e-mail ou d’une landing page dans Design Studio
* Les pages archivées ne peuvent pas être utilisées dans les groupes de test de page de destination

Fonctionnalité qui ne sera **pas** modifiée lors de l’archivage :

* La recherche globale trouve toujours des résultats dans les dossiers archivés
* Vous pouvez utiliser un filtre pour sélectionner les ressources archivées à utiliser dans les rapports

### Désactiver les campagnes sur l’archive {#disable-campaigns-archive}

Lorsqu’un dossier ou un programme est archivé, ou qu’une campagne dynamique active est déplacée dans un dossier déjà archivé, Marketo Engage arrête l’exécution des campagnes affectées :

* Les **Campagnes déclenchées** sont désactivées.
* Les exécutions en attente des campagnes **par lots** sont annulées.
* **Les campagnes exécutables** n’ont pas d’état d’exécution, aucune action n’est donc entreprise.

**Actions prises en charge**

Les actions suivantes désactivent les campagnes :

* Glisser-déposer un **dossier** contenant les campagnes actives dans un dossier archivé
* Effectuez un glisser-déposer d’un **programme** (tout type) contenant des campagnes actives dans un dossier archivé
* Glisser-déposer une **campagne intelligente unique** dans un dossier archivé
* Cliquez avec le bouton droit de la souris **Déplacer** sur une seule campagne dynamique dans un dossier archivé.
* Cliquez avec le bouton droit de la souris **Déplacer le dossier** sur un dossier contenant des campagnes actives dans un dossier archivé
* Cliquez avec le bouton droit **Déplacer** sur un programme contenant des campagnes actives dans un dossier archivé
* Cliquez avec le bouton droit **Convertir en dossier archivé** dans un dossier pour l’archiver sur place sans le déplacer.

>[!NOTE]
>
>Si une campagne intelligente à l’intérieur du dossier ou du programme en cours d’archivage est référencée ailleurs (par exemple, via une étape de flux « Demander la campagne »), l’archivage est bloqué pour empêcher de rompre cette autre campagne.
