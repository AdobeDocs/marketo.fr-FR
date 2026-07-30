---
description: Découvrez comment activer la fonctionnalité Désactiver les campagnes intelligentes lors de l’archivage, qui désactive automatiquement les campagnes lorsqu’un dossier ou un programme est archivé dans Marketo.
title: Désactiver les campagnes intelligentes sur l’archive
feature: Administration
hide: true
source-git-commit: 526d10bb96e059d251a76ca720ff81ab42ee9516
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Désactiver les campagnes intelligentes sur l’archive {#disable-smart-campaigns-on-archive}

Lorsque cette fonctionnalité est activée, l’archivage d’un dossier ou d’un programme désactive automatiquement ses campagnes afin d’éviter toute activité inattendue.

Lorsqu’un dossier ou un programme est archivé, ou qu’une campagne dynamique active est déplacée dans un dossier déjà archivé, Marketo Engage arrête l’exécution des campagnes affectées :

* Les **Campagnes déclenchées** sont désactivées.
* Les exécutions en attente des campagnes **par lots** sont annulées.
* **Les campagnes exécutables** n’ont pas d’état d’exécution, aucune action n’est donc entreprise.

## Activation {#how-to-enable}

1. Dans la section **Admin**, cliquez sur **Coffre au trésor**.

   ![Le menu de navigation d’administration avec Treasure Chest mis en surbrillance](assets/disable-smart-campaigns-on-archive-1.png)

1. Faites défiler l’écran jusqu’à _Désactiver les campagnes intelligentes sur l’archive_ et cliquez sur **Modifier**.

   ![Page des paramètres Treasure Chest affichant la ligne Désactiver les campagnes intelligentes sur l’archive avec le bouton Modifier](assets/disable-smart-campaigns-on-archive-2.png)

1. Sélectionnez la case à cocher **Activé** et cliquez sur **Enregistrer**.

   ![Boîte de dialogue Désactiver les campagnes intelligentes dans l’archive affichant la case à cocher Activé et le bouton Enregistrer](assets/disable-smart-campaigns-on-archive-3.png)

<table>
  <tr>
    <td><b>Activé (coché)</b></td>
    <td>L’archivage désactive chaque campagne, conformément aux règles ci-dessus.</td>
  </tr>
  <tr>
    <td><b>Désactivé (non coché)</b></td>
    <td>L’archivage d’un dossier ou d’un programme fonctionne toujours, mais les campagnes restent en cours d’exécution ou sont planifiées en l’état.</td>
  </tr>
</table>

>[!IMPORTANT]
>
>Après avoir activé ce paramètre, vous devez actualiser votre navigateur pour que la modification soit prise en compte.

## Actions prises en charge

Les actions suivantes désactivent les campagnes lorsque l’option _Désactiver les campagnes intelligentes sur l’archive_ est activée :

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
