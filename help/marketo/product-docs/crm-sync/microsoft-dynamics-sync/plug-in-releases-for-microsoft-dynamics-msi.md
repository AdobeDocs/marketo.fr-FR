---
unique-page-id: 10099102
description: Versions de module externe pour Microsoft Dynamics MSI - Documents Marketo - Documentation du produit
title: Versions de module externe pour Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 8%

---

# Versions de module externe pour Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

Lorsque vous vous synchronisez pour la première fois avec Microsoft Dynamics, vous téléchargez et installez la dernière version des plug-ins pour Marketo Sales Insight (MSI). Régulièrement, Marketo Engage met à jour ces plug-ins afin que vous puissiez revenir au même endroit pour télécharger la nouvelle version.

Si vous utilisez la solution de synchronisation CRM native de Marketo vers Dynamics, veuillez [télécharger le dernier module externe](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} corresponding to your Dynamics release. For those who have a custom sync and have purchased Marketo Sales Insight, the [package is here](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>Ces versions fonctionnent pour les versions on-premise et en ligne de Dynamics.

## Mise à niveau de votre solution MSI {#upgrading-your-msi-solution}

1. Importez la dernière version de la solution. _sur la version existante_ de votre CRM Dynamics en appuyant sur la touche **[!UICONTROL Importer]** dans Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Exemple : si votre Dynamics CRM dispose de la version 2.0.0.20 et que la dernière version est 2.0.0.21, vous devez importer _over_ version 2.0.0.20.

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Sélectionner **[!UICONTROL Phase de mise à niveau]** et **[!UICONTROL Conserver les personnalisations]**, puis cliquez sur **[!UICONTROL Importer]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Cliquez sur **[!UICONTROL Suivant]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Après un import réussi, deux solutions MSI s’affichent : MarketoSalesInsight et MarketoSalesInsight_Upgrade. Sélectionnez l’ancienne solution et cliquez sur Apply Solution Upgrade.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

Et c&#39;est tout ! Après la mise à niveau, une seule solution MSI s’affiche.

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
   <th colspan="1">Notes</th> 
  </tr> 
  <tr> 
   <td colspan="1">02/03/22</td> 
   <td colspan="1">2.0.0.27</td> 
   <td colspan="1">Disposition du compte pour les statistiques : moments intéressants, changements de score, activités web, activités de courrier électronique.</td> 
  </tr>
  <tr> 
   <td colspan="1">01/05/22</td> 
   <td colspan="1">2.0.0.26</td> 
   <td colspan="1">Score d’adoption du programme pour envoyer un courrier électronique</td> 
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
   <td colspan="1">Bug Fix : attribution de l’accès aux champs de configuration de l’API MSI aux utilisateurs qui détiennent le rôle Sales Insight</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">Correction de bogue : ajout d’un message de validation pour les enregistrements non synchronisés</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">Correction de bogue : pour masquer le mot de passe secret MSI sur la configuration de l’API MSD</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">Bug Fix : pour modifier la validation de l’ID de rôle MSI pour l’affichage des boutons MSI</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">Bug Fix : affichez le champ propriétaire et rendez les champs non obligatoires</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">Bug Fix : suppression de la dépendance de lien du paramètre de plan de site MSD CRM</td> 
  </tr> 
 </tbody> 
</table>
