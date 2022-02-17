---
unique-page-id: 10099389
description: Versions du module externe Marketo pour Microsoft Dynamics - Documents Marketo - Documentation du produit
title: Versions du module externe Marketo pour Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
source-git-commit: 1379fcbdc0a8673b1d6cb17a9d573d3625d5a1b8
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 7%

---

# Versions du module externe Marketo pour Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

Lors de la première synchronisation avec Microsoft Dynamics, vous téléchargez la dernière version des modules externes de Marketo. Régulièrement, Marketo met à jour ces modules externes afin que vous puissiez revenir au même endroit pour télécharger la nouvelle version.

[Télécharger le dernier module externe](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) correspondant à votre version Dynamics.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Mise à jour de votre solution Dynamics {#updating-your-dynamics-solution}

1. Importez la dernière version de la solution par rapport à la version existante de votre Dynamics CRM (ex : si votre Dynamics CRM dispose de la version 1.4 et que la dernière version est 1.5, vous devez importer _over_ version 1.4).

1. La fenêtre contextuelle suivante s’affiche. Sélectionner **Mettre à jour** et **Conserver les personnalisations**, puis cliquez sur **Importer**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Dernières versions {#latest-versions}

>[!NOTE]
>
>Ces versions fonctionnent pour les versions on-premise et en ligne de Dynamics.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Version</th> 
   <th colspan="1">Date de publication</th> 
   <th>Remarques</th> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.1</td> 
   <td colspan="1">02/04/21</td> 
   <td colspan="1">Prise en charge de la synchronisation de champs à sélection multiple (cette fonctionnalité est disponible uniquement pour la version 9.X et ultérieure). .</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">Ajout de la prise en charge de la synchronisation Campaign avec MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">Ajout de la prise en charge des conditions d’usine permettant de contacter le processus de contact pour Microsoft Dynamics version 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">Correction de bogues : Erreur de processus métier lors de la tentative d’installation des solutions Marketo pour Dynamics 2013.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">Correction de bogues : Révision interne.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">Correction de bogues : Le module externe ne s’est pas abonné aux événements qui capturent le changement d’état de l’objet personnalisé. Ce correctif est spécifique à Dynamics CRM On Premise 2011. </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">Correction de bogues : Les mises à jour du rôle de contact d’opportunité n’étaient pas entièrement capturées.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>Correction de bogues : Une transaction de mise à jour inutile sur le rôle de personnalisation dans le journal marketing a été signalée lors de la création de l’opportunité. </p><p>Correction de bogues : Une transaction de suppression supplémentaire a été consignée lors de la suppression de l’entité customeropportunityrole.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">Correction de bogues : Mise à jour et suppression des objets personnalisés asynchrones.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">Correction de bogues : Lorsque le filtre de synchronisation du prospect était défini sur NON et que l’opportunité et le contact n’avaient pas de filtre de synchronisation, le journal de création n’était pas généré pour le contact et l’opportunité lorsque le prospect était qualifié.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>Correction de bogues : Un événement d’affectation était consigné lorsque le filtre de synchronisation était désactivé.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">Correction de bogues : Le client n’a pas pu créer de piste dans le CRM, car l’utilisateur de connexion ne disposait pas de l’autorisation de configuration Marketo.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">Correction de bogues : Création de limites d’accès pour les utilisateurs normaux de Dynamics afin de répondre aux problèmes de sécurité.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>Correction de bogues : Dans Dynamics, les mises à jour n’étaient pas synchronisées avec Marketo pour les étapes et les images.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">Correction de bogues : Les enregistrements de piste étaient synchronisés avec Marketo lorsque le filtre de synchronisation était défini sur false.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Téléchargement de la solution de gestion des leads Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
