---
unique-page-id: 10099102
description: Versions de modules externes pour Microsoft Dynamics MSI - Marketo Docs - Documentation sur les produits
title: Versions de plug-in pour Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 5%

---

# Versions de module externe pour Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

Lors de la première synchronisation avec Microsoft Dynamics, vous téléchargez et installez la dernière version des modules complémentaires pour Marketo Sales Insight (MSI). Régulièrement, Marketo met à jour ces plug-ins afin que vous puissiez revenir au même endroit pour télécharger la nouvelle version.

Veuillez [télécharger le dernier module externe](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) correspondant à votre version de Dynamics.

>[!NOTE]
>
>Ces versions fonctionnent pour les versions sur site et en ligne de Dynamics.

## Mise à niveau de votre solution MSI {#upgrading-your-msi-solution}

1. Importez la dernière version de la solution _sur la version existante_ de votre Dynamics CRM en appuyant sur le bouton **Importer** de Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Exemple : si votre Dynamics CRM a la version 2.0.0.20 et que la dernière version est 2.0.0.21, vous importez _sur_ la version 2.0.0.20.

1. Cliquez sur **Suivant**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Sélectionnez **Phase de mise à niveau** et **Conserver les personnalisations**, puis cliquez sur **Importer**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Cliquez sur **Suivant**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Après une importation réussie, vous verrez deux solutions MSI : MarketoSalesInsight et MarketoSalesInsight_Upgrade. Sélectionnez l’ancienne solution et cliquez sur Appliquer la mise à niveau de la solution.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

Et c&#39;est tout ! Après la mise à niveau, vous ne verrez qu&#39;une seule solution MSI.

## Mises à jour de la version {#version-updates}

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
   <td colspan="1">01/10/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">Correctif : Affectation de l’accès aux champs de configuration de l’API MSI aux utilisateurs bénéficiant du rôle Sales Insight</td> 
  </tr> 
  <tr> 
   <td colspan="1">20/07/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">Correctif : Ajouter un message de validation pour les enregistrements non synchronisés</td> 
  </tr> 
  <tr> 
   <td colspan="1">12/06/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">Correctif : Pour masquer le mot de passe secret MSI sur la configuration de l’API MSD</td> 
  </tr> 
  <tr> 
   <td colspan="1">26/05/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">Correctif : Pour modifier la validation de l’ID de rôle MSI pour l’affichage des boutons MSI</td> 
  </tr> 
  <tr> 
   <td colspan="1">21/05/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">Correctif : Afficher le champ de propriétaire et rendre les champs non obligatoires</td> 
  </tr> 
  <tr> 
   <td colspan="1">28/04/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">Correctif : Suppression de la dépendance de lien de paramètre de plan de site MSD CRM</td> 
  </tr> 
 </tbody> 
</table>
