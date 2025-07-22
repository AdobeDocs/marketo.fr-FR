---
unique-page-id: 10099389
description: Versions du plug-in Marketo pour  [!DNL Microsoft Dynamics]  - Documentation de Marketo - Documentation du produit
title: Versions du plug-in Marketo pour  [!DNL Microsoft Dynamics]
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Versions du plug-in Marketo pour [!DNL Microsoft Dynamics] {#marketo-plugin-releases-for-microsoft-dynamics}

Lors de la première synchronisation avec [!DNL Microsoft Dynamics], vous téléchargez la dernière version des modules externes pour Marketo. Marketo met régulièrement à jour ces plug-ins afin que vous puissiez revenir au même endroit pour télécharger la nouvelle version.

[Téléchargez le dernier plug-in](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) correspondant à votre version [!DNL Dynamics].

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Mise à jour de votre solution [!DNL Dynamics] {#updating-your-dynamics-solution}

1. Importez la dernière version de la solution par rapport à la version existante de votre CRM [!DNL Dynamics] (par exemple, si votre CRM [!DNL Dynamics] dispose de la version 1.4 et que la dernière version est la version 1.5, vous devez importer _plus_ la version 1.4).

1. Le pop-up suivant s’affiche. Sélectionnez **Mettre à jour** et **Conserver les personnalisations**, puis cliquez sur **Importer**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Dernières versions {#latest-versions}

>[!NOTE]
>
>Ces versions fonctionnent pour les versions on-premise et en ligne d’[!DNL Dynamics].

<table> 
 <tbody> 
  <tr> 
   <th style="width:15%">Version</th> 
   <th style="width:20%">Date de publication</th> 
   <th style="width:65%">Notes</th> 
  </tr>
  <tr> 
   <td>5.0.2.1</td> 
   <td>1/19/24</td> 
   <td>Correction de bugs : correction de bugs liés à la synchronisation d’entités personnalisées.</td> 
  </tr> 
  <tr> 
   <td>5.0.2.0</td> 
   <td>03/24/23</td> 
   <td>Correction de bugs : correction de bugs qui empêchaient la fusion de contacts sur MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">Ajout de la prise en charge de la synchronisation de la campagne avec MS [!DNL Dynamics].</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">Ajout de la prise en charge du processus de qualification de lead à contacter prêt à l’emploi pour [!DNL Microsoft Dynamics] version 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">Correction de bug : erreur de processus d’entreprise lors de l’installation des solutions Marketo pour [!DNL Dynamics] 2013.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.24</td> 
   <td>8/22/18</td> 
   <td>Ajout de la prise en charge du processus de qualification de lead à contacter prêt à l’emploi pour Microsoft Dynamics version 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">Correction de bug : le plug-in ne s’abonnait pas aux événements qui capturent le changement d’état de l’objet personnalisé. Ce correctif est spécifique à [!DNL Dynamics] CRM On-Premise 2011. </td> 
  </tr> 
  <tr> 
   <td>4.0.0.22</td> 
   <td>9/29/17</td> 
   <td>Correction de bugs : révision interne.</td> 
  </tr> 
  <tr> 
   <td><p>4.0.0.21</p></td> 
   <td>11/9/16</td> 
   <td>Correction de bug : le plug-in ne s’abonnait pas aux événements qui capturent le changement d’état de l’objet personnalisé. Ce correctif est spécifique à Dynamics CRM On Premise 2011.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.20</td> 
   <td>7/22/16</td> 
   <td>Correction de bug : les mises à jour du rôle de contact d’opportunité n’étaient pas entièrement capturées.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.19</td> 
   <td>6/28/16</td> 
   <td>Correction de bug : une transaction de mise à jour inutile sur le rôle customeropportunitydans le journal marketo a été notée lors de la création de l’opportunité.<p>Correction de bug : une transaction de suppression supplémentaire était consignée lors de la suppression de l’entité de rôle customeropportunityrole.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.18</td> 
   <td>5/31/16</td> 
   <td>Correction de bug : la mise à jour et la suppression des objets personnalisés étaient asynchrones.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.17</td> 
   <td>4/8/16</td> 
   <td>Correction de bug : lorsque le filtre de synchronisation du prospect était défini sur NON et que l’opportunité et le contact n’avaient pas de filtre de synchronisation, le journal de création n’était pas généré pour le contact et l’opportunité lorsque le prospect était qualifié.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.16</td> 
   <td>3/29/16</td> 
   <td>Correction de bug : un événement d’affectation était consigné lorsque le filtre de synchronisation était désactivé.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.15</td> 
   <td>3/3/16</td> 
   <td>Correction de bug : le client ne pouvait pas créer de prospect dans CRM, car l’utilisateur connecté ne disposait pas de l’autorisation Configuration Marketo.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">Correction de bug : création de limites d’accès pour les utilisateurs et utilisatrices [!DNL Dynamics] normaux afin de résoudre les problèmes de sécurité.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>Correction de bug : les mises à jour dans [!DNL Dynamics] ne se synchronisaient pas avec Marketo pour les étapes et les images.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.12</td> 
   <td>11/12/15</td> 
   <td>Correction de bug : les enregistrements de lead étaient synchronisés avec Marketo lorsque le filtre de synchronisation était défini sur false.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Télécharger la solution de gestion des prospects Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
