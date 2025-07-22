---
unique-page-id: 3571890
description: Activer les groupes de champs personnalisés pour l’analyse des performances du modèle (leads) - Documents Marketo - Documentation du produit
title: Activer les groupes de champs personnalisés pour l’analyse des performances du modèle (prospects)
exl-id: 417fd74f-d8f5-477b-b633-0fdfdd68b22b
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Activer les groupes de champs personnalisés pour l’analyse des performances du modèle (prospects) {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!PREREQUISITES]
>
>Classez les champs standard ou personnalisés en groupes pour la création de rapports via l’organisateur de champs de Marketo. Pour plus d’informations, consultez [Création de groupes de champs personnalisés via l’organisateur de champs](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md).

<table> 
 <tbody> 
  <tr> 
   <td colspan="3" rowspan="1"><p align="center"><strong>Comment l’activation d’un groupe de champs personnalisés affecte-t-elle plusieurs zones d’analyse dans l’Explorateur du cycle du chiffre d’affaires ?</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Que se passe-t-il lorsque... ?</strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>Impact sur le domaine <span class="uicontrol">Analyse des performances du modèle (prospects)</span></strong></p></td> 
   <td colspan="1" rowspan="1"><p><strong>Impact sur les domaines de l’analyse des leads, de l’analyse des campagnes et de l’analyse des opportunités</strong></p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Que se passe-t-il lorsque vous activez un groupe de champs personnalisés associé à un champ de prospect ou d’entreprise standard ?</strong></p></td> 
   <td colspan="1" rowspan="1"><p>Le groupe de champs personnalisés est activé pour la création de rapports dans la zone <span class="uicontrol">Analyse des performances du modèle (prospects)</span></p></td> 
   <td colspan="1" rowspan="1"><p>Pas D’Impact</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Que se passe-t-il lorsque vous activez un groupe de champs personnalisés associé à un champ personnalisé de personne ou d’entreprise ?</strong></p></td> 
   <td colspan="1" rowspan="1"><p>Le groupe de champs personnalisés est activé pour la création de rapports dans la zone <span class="uicontrol">Analyse des performances du modèle (prospects)</span></p></td> 
   <td colspan="1" rowspan="1"><p>Le champ personnalisé lui-même est activé pour la création de rapports dans les zones Analyse des prospects, Analyse des campagnes et Analyse des opportunités.</p><p><strong>REMARQUE :</strong> les groupes de champs personnalisés ne sont PAS pris en charge dans ces zones d’analyse. Par conséquent, les associations de groupes ne s’affichent pas dans l’Explorateur du cycle du chiffre d’affaires, <em>uniquement</em> dans le champ personnalisé.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour activer un groupe de champs personnalisé pour la création de rapports, procédez comme suit dans la zone [!UICONTROL Analyse des performances du modèle (prospects)].

1. Cliquez sur **[!UICONTROL Admin]**.

   ![](assets/one-1.png)

1. Cliquez sur **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/two-1.png)

1. Cliquez sur **[!UICONTROL Aucun]** en regard d’un groupe de champs vide. Si trois groupes de champs sont déjà activés et que vous souhaitez effectuer une modification, cliquez sur le nom du groupe de champs que vous souhaitez modifier.

   ![](assets/three.png)

1. Cliquez sur le menu déroulant **[!UICONTROL Champ]** et sélectionnez celui de votre choix.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Cet exemple a activé un groupe de champs personnalisés pour un champ standard (État). Par conséquent, seule la zone [!UICONTROL Analyse de la performance du modèle (prospects)] a été affectée. Si un groupe de champs personnalisés pour un champ de personne ou d’entreprise personnalisé avait été activé, le groupe activé s’affichait dans la section [!UICONTROL Analyse des performances du modèle (leads)] de l’onglet Synchroniser le résumé. Le nombre de champs personnalisés pour l’analyse des leads, des campagnes et des opportunités augmenterait d’une unité.

1. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/five-1.png)
