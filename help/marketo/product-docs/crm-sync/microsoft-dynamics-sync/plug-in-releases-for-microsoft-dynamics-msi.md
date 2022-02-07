---
unique-page-id: 10099102
description: Versions de module externe pour Microsoft Dynamics MSI - Documents Marketo - Documentation du produit
title: Versions de module externe pour Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
source-git-commit: 7b22aec56d15826c1fecd2cf026c561c4df8531c
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 7%

---

# Versions de module externe pour Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

Lorsque vous vous synchronisez pour la première fois avec Microsoft Dynamics, vous téléchargez et installez la dernière version des plug-ins pour Marketo Sales Insight (MSI). Régulièrement, Marketo met à jour ces plug-ins afin que vous puissiez revenir au même endroit pour télécharger la nouvelle version.

Veuillez [télécharger le dernier module externe](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) correspondant à votre version Dynamics.

>[!NOTE]
>
>Ces versions fonctionnent pour les versions on-premise et en ligne de Dynamics.

## Mise à niveau de votre solution MSI {#upgrading-your-msi-solution}

1. Importez la dernière version de la solution. _sur la version existante_ de votre CRM Dynamics en appuyant sur la touche **Importer** dans Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Exemple : si votre Dynamics CRM dispose de la version 2.0.0.20 et que la dernière version est 2.0.0.21, vous devez importer _over_ version 2.0.0.20.

1. Cliquez sur **Suivant**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Sélectionner **Phase de mise à niveau** et **Conserver les personnalisations**, puis cliquez sur **Importer**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Cliquez sur **Suivant**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Après un import réussi, deux solutions MSI s’affichent : MarketoSalesInsight et MarketoSalesInsight_Upgrade. Sélectionnez l’ancienne solution et cliquez sur Appliquer la mise à niveau de la solution.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

Et voilà ! Après la mise à niveau, une seule solution MSI s’affiche.

## Mises à jour de version {#version-updates}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">Date de publication</th> 
   <th colspan="1">Version</th> 
   <th colspan="1">Remarques</th> 
  </tr> 
  <tr> 
   <td colspan="1">02/03/22</td> 
   <td colspan="1">2.0.0.27</td> 
   <td colspan="1">Disposition du compte pour les statistiques : Moments intéressants, changements de score, activités web, activités email</td> 
  </tr>
  <tr> 
   <td colspan="1">01/05/22</td> 
   <td colspan="1">2.0.0.26</td> 
   <td colspan="1">Score d’adoption du programme pour l’envoi d’un courrier électronique</td> 
  </tr>
  <tr> 
   <td colspan="1">10/28/21</td> 
   <td colspan="1">2.0.0.25</td> 
   <td colspan="1">Mesures de score d’adoption du produit, nouveau tableau de bord global (activité web, courrier électronique, meilleurs paris)</td> 
  </tr>
  <tr> 
   <td colspan="1">02/10/21</td> 
   <td colspan="1">2.0.0.22</td> 
   <td colspan="1">Suppression de l’audit automatique activé et modifications de la documentation sur la solution MSI</td> 
  </tr>
  <tr> 
   <td colspan="1">10/01/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">Bug Fix : Attribution de l’accès aux champs de configuration de l’API MSI aux utilisateurs ayant un rôle Sales Insight</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">Correction de bogues : Ajout d’un message de validation pour les enregistrements non synchronisés</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">Correction de bogues : Pour masquer le mot de passe secret MSI sur la configuration de l’API MSD</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">Correction de bogues : Pour modifier la validation de l’ID de rôle MSI pour afficher les boutons MSI</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">Correction de bogues : Afficher le champ propriétaire et rendre les champs non obligatoires</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">Correction de bogues : Suppression de la dépendance de lien de paramètre de plan de site MSD CRM</td> 
  </tr> 
 </tbody> 
</table>
