---
unique-page-id: 4719294
description: Personnalisation De La Synchronisation Des Activités - Documents Marketo - Documentation Du Produit
title: Personnaliser la synchronisation des activités
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Personnaliser la synchronisation des activités {#customize-activities-sync}

Si vous n’utilisez pas Marketo Sales Insight, Marketo Engage peut créer des enregistrements d’historique des activités Salesforce pour certains événements. Voici comment les activer.

>[!NOTE]
>
>La synchronisation Salesforce/Marketo Engage ne transmet aucune activité à Salesforce qui s’est produite avant que la personne ne soit transmise à Salesforce.

1. Accédez à **[!UICONTROL Admin]**.

   ![](assets/customize-activities-sync-1.png)

1. Cliquez sur **[!DNL Salesforce]**, puis sur **[!UICONTROL Modifier les options de synchronisation]**.

   ![](assets/two-1.png)

1. Cochez les cases en regard des activités que Marketo doit pousser vers Salesforce, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Une fois activé, Marketo intégrera l’historique de l’activité pendant trois mois. Selon la quantité de données, _cette opération peut prendre plusieurs jours_. Les mises à jour qui se produisent pendant la notification push initiale des activités peuvent être retardées jusqu’à ce que la synchronisation initiale des activités soit terminée.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>Type d’activité</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Formulaire rempli]</td> 
   <td>A rempli un formulaire Marketo</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ajouté à la liste]</td> 
   <td><p>Étape de flux : a été ajouté à une liste statique</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email sent]</td> 
   <td>Étape de flux : un e-mail a été envoyé</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email diffusé]</td> 
   <td>A reçu un e-mail (sans rebond)</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL E-mail ouvert]</td> 
   <td>A ouvert un email (sans bloquer les images)</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Clic sur un lien dans un e-mail]</td> 
   <td>A cliqué sur un lien dans un e-mail envoyé par Marketo</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Supprimé de la liste]</td> 
   <td>Étape de flux : a été supprimé d’une liste statique</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remove from flow]</td> 
   <td>Étape de flux : supprimer du flux</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sales email sent]</td> 
   <td>Un e-mail a été envoyé via Marketo Sales Insight.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL E-mail de vente ouvert]</td> 
   <td>A ouvert un e-mail envoyé via Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cliquez sur le lien dans l’e-mail de vente]</td> 
   <td>A cliqué sur un lien dans un e-mail envoyé via Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sales email received]</td> 
   <td>Un e-mail a été reçu et enregistré par le représentant commercial dans le plug-in MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>« E-mail de vente reçu » ne signifie _envoyé_. Le statut Diffusé n’est pas capturé pour les e-mails envoyés via Sales Insight.

>[!TIP]
>
>Si vous souhaitez obtenir plus d’informations sur Marketo dans Salesforce, consultez notre produit [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
