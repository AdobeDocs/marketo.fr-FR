---
unique-page-id: 10099389
description: Versions du module externe Marketo pour Microsoft Dynamics - Documents Marketo - Documentation du produit
title: Versions du module externe Marketo pour Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 492a43045bdf77243e4600eeb2223e750a35859b
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Versions du module externe Marketo pour Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

Lors de la première synchronisation avec Microsoft Dynamics, vous téléchargez la dernière version des modules externes de Marketo. Régulièrement, Marketo met à jour ces modules externes afin que vous puissiez revenir au même endroit pour télécharger la nouvelle version.

[Télécharger le dernier module externe](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} correspondant à votre version Dynamics.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Mise à jour de votre solution Dynamics {#updating-your-dynamics-solution}

1. Importez la dernière version de la solution par rapport à la version existante de votre CRM Dynamics (par exemple, si votre CRM Dynamics dispose de la version 1.4 et que la dernière version est la version 1.5), vous devez importer _over_ version 1.4).

1. La fenêtre contextuelle suivante s’affiche. Sélectionner **Mettre à jour** et **Conserver les personnalisations**, puis cliquez sur **Importer**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Dernières versions {#latest-versions}

>[!NOTE]
>
>Ces versions fonctionnent pour les versions on-premise et en ligne de Dynamics.

<table> 
 <tbody> 
  <tr> 
   <th>Version</th> 
   <th>Date de publication</th> 
   <th>Notes</th> 
  </tr>
  <tr> 
   <td>5.0.2.1</td> 
   <td>10/13/23</td> 
   <td>Correction de bogues : correction de bogues liés à la synchronisation des entités personnalisées.</td> 
  </tr> 
  <tr> 
   <td>5.0.2.0</td> 
   <td>03/24/23</td> 
   <td>Correction de bogues : correction de bogues qui empêchaient la fusion de contacts sur MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td>5.0.1.8</td> 
   <td>03/27/23</td> 
   <td>Correction de bogue : empêche le module externe d’écraser d’autres personnalisations sur les éléments d’IU dans MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td>5.0.1.1</td> 
   <td>02/04/21</td> 
   <td>Prise en charge de la synchronisation de champs à sélection multiple (cette fonctionnalité est disponible uniquement pour la version 9.X et ultérieure).</td> 
  </tr> 
  <tr> 
   <td>4.2.0.0</td> 
   <td>10/16/20</td> 
   <td>Ajout de la prise en charge de la synchronisation Campaign avec MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.24</td> 
   <td>8/22/18</td> 
   <td>Ajout de la prise en charge des conditions d’usine permettant de contacter le processus de contact pour Microsoft Dynamics version 9.x.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.23</td> 
   <td>6/27/18</td> 
   <td>Bug Fix : erreur de processus métier lors de la tentative d’installation des solutions Marketo pour Dynamics 2013.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.22</td> 
   <td>9/29/17</td> 
   <td>Correction de bogue : révision interne.</td> 
  </tr> 
  <tr> 
   <td><p>4.0.0.21</p></td> 
   <td>11/9/16</td> 
   <td>Bug Fix : le module externe n’a pas souscrit aux événements qui capturent le changement d’état de l’objet personnalisé. Ce correctif est spécifique à Dynamics CRM On Premise 2011.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.20</td> 
   <td>7/22/16</td> 
   <td>Correction de bogue : les mises à jour du rôle de contact d’opportunité n’étaient pas entièrement capturées.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.19</td> 
   <td>6/28/16</td> 
   <td>Correction de bogue : une transaction de mise à jour inutile sur le rôle d’opportunité client dans le journal marketing a été signalée lors de la création de l’opportunité.<p>Correction de bogue : une transaction de suppression supplémentaire était consignée lors de la suppression de l’entité customeropportunityrole .</td> 
  </tr> 
  <tr> 
   <td>4.0.0.18</td> 
   <td>5/31/16</td> 
   <td>Correction de bogue : rendu la mise à jour et la suppression des objets personnalisés asynchrones.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.17</td> 
   <td>4/8/16</td> 
   <td>Correction de bogue : lorsque le filtre de synchronisation du prospect était défini sur NO et que l’opportunité et le contact n’avaient pas de filtre de synchronisation, le journal de création n’était pas généré pour le contact et l’opportunité lorsque le prospect était qualifié.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.16</td> 
   <td>3/29/16</td> 
   <td>Correction de bogue : un événement d’affectation était consigné lorsque le filtre de synchronisation était désactivé.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.15</td> 
   <td>3/3/16</td> 
   <td>Correction de bogue : le client n’a pas pu créer de piste dans le CRM, car l’utilisateur de connexion n’avait pas l’autorisation de configuration Marketo.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.14</td> 
   <td>1/18/16</td> 
   <td>Correction de bogue : création de limites d’accès pour les utilisateurs normaux de Dynamics afin de répondre aux problèmes de sécurité.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.13</td> 
   <td>12/30/15</td> 
   <td>Bug Fix : les mises à jour dans Dynamics n’étaient pas synchronisées avec Marketo pour les étapes et les images.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.12</td> 
   <td>11/12/15</td> 
   <td>Bug Fix : les enregistrements de piste étaient synchronisés avec Marketo lorsque le filtre de synchronisation était défini sur false.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Téléchargement de la solution de gestion des leads Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
