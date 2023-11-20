---
unique-page-id: 4719294
description: Personnalisation de la synchronisation des activités - Documents Marketo - Documentation du produit
title: Personnalisation de la synchronisation des activités
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 12%

---

# Personnalisation de la synchronisation des activités {#customize-activities-sync}

Si vous n’utilisez pas Marketo Sales Insight, Marketo Engage peut créer des enregistrements d’historique des activités Salesforce pour certains événements. Voici comment les activer.

1. Accédez à **[!UICONTROL Administration]**.

   ![](assets/admin.png)

1. Cliquez sur **[!DNL Salesforce]**, puis cliquez sur **[!UICONTROL Modifier les options de synchronisation]**.

   ![](assets/two-1.png)

1. Cochez les cases en regard des activités que Marketo doit transmettre à Salesforce, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Une fois activé, Marketo génère l’historique des activités pour trois mois. Selon la quantité de données, _cela peut prendre plusieurs jours._. Les mises à jour survenant pendant la notification push initiale des activités peuvent être retardées jusqu’à ce que la synchronisation initiale des activités soit terminée.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>Type d'activité</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Formulaire rempli</td> 
   <td>Remplir tout formulaire Marketo</td> 
  </tr> 
  <tr> 
   <td>Ajouté à la liste</td> 
   <td><p>Étape de flux : a été ajoutée à une liste statique</p></td> 
  </tr> 
  <tr> 
   <td>E-mail envoyé</td> 
   <td>Étape de flux : a été envoyé un email</td> 
  </tr> 
  <tr> 
   <td>E-mail remis au destinataire</td> 
   <td>Réception d’un email (sans rebond)</td> 
  </tr> 
  <tr> 
   <td>E-mail ouvert</td> 
   <td>A ouvert un email (sans bloquer les images)</td> 
  </tr> 
  <tr> 
   <td>Lien ayant fait l’objet d’un clic dans l’e-mail</td> 
   <td>Clic sur un lien dans un email envoyé par Marketo</td> 
  </tr> 
  <tr> 
   <td>Supprimé de la liste</td> 
   <td>Étape de flux : a été supprimée d’une liste statique.</td> 
  </tr> 
  <tr> 
   <td>Supprimer du flux</td> 
   <td>Étape de flux : supprimer du flux</td> 
  </tr> 
  <tr> 
   <td>E-mail de vente envoyé</td> 
   <td>A été envoyé par courrier électronique via Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-mail de vente ouvert</td> 
   <td>Ouverture d’un courrier électronique envoyé par le biais de Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Clic sur le lien dans l’email de vente</td> 
   <td>Clic sur un lien dans un e-mail envoyé via Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-mail de vente reçu</td> 
   <td>Un courrier électronique a été reçu et consigné par le représentant commercial dans le module externe MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;Adresse électronique de vente reçue&quot; _not_ moyenne diffusée. L’état Distribué n’est pas capturé pour les emails envoyés via Sales Insight.

>[!TIP]
>
>Si vous souhaitez obtenir plus d’informations Marketo dans Salesforce, consultez notre [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} produit.
