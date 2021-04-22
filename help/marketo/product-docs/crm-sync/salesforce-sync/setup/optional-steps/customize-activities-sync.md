---
unique-page-id: 4719294
description: Synchronisation des Activités personnalisées - Documents Marketo - Documentation du produit
title: Personnaliser la synchronisation des Activités
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 12%

---

# Synchronisation des Activités personnalisée {#customize-activities-sync}

Si vous n&#39;utilisez pas Marketo Sales Insight, Marketo peut créer des enregistrements d&#39;historique des Activités de Salesforce pour certains événements. Voici comment les activer.

1. Accédez à **Admin**.

   ![](assets/admin.png)

1. Cliquez sur **Salesforce**, puis sur **Modifier les options de synchronisation**.

   ![](assets/two-1.png)

1. Cochez les cases en regard des activités que Marketo doit transmettre à Salesforce, puis cliquez sur **Enregistrer**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Une fois activée, Marketo repoussera l&#39;équivalent de trois mois d&#39;activité historique. Selon la quantité de données, _cette opération peut prendre plusieurs jours._ Les mises à jour survenant pendant la transmission des Activités initiales peuvent être retardées jusqu’à la fin de la synchronisation des Activités initiales.

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
   <td>A rempli le formulaire</td> 
   <td>Renseigner tout formulaire Marketo</td> 
  </tr> 
  <tr> 
   <td>Ajouté à la liste</td> 
   <td><p>Étape de flux : A été ajouté à une liste statique</p></td> 
  </tr> 
  <tr> 
   <td>E-mail envoyé</td> 
   <td>Étape de flux : A été envoyé un courrier électronique</td> 
  </tr> 
  <tr> 
   <td>E-mail remis au destinataire</td> 
   <td>Réception d’un courrier électronique (sans retour)</td> 
  </tr> 
  <tr> 
   <td>E-mail ouvert</td> 
   <td>Ouverture d’un courrier électronique (sans bloquer les images)</td> 
  </tr> 
  <tr> 
   <td>A Cliqué sur le lien dans l'e-mail</td> 
   <td>Cliquez sur un lien dans un courrier électronique envoyé par Marketo.</td> 
  </tr> 
  <tr> 
   <td>Supprimé de la liste</td> 
   <td>Étape de flux : A été supprimé d’une liste statique</td> 
  </tr> 
  <tr> 
   <td>Supprimer des flux</td> 
   <td>Étape de flux : Supprimer du flux</td> 
  </tr> 
  <tr> 
   <td>E-mail de vente envoyé</td> 
   <td>A été envoyé par courrier électronique via Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-mail de vente ouvert</td> 
   <td>Ouverture d’un courrier électronique envoyé via Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Cliquez sur le lien dans le courriel de vente</td> 
   <td>Cliquez sur un lien dans un courrier électronique envoyé par l’intermédiaire de Marketo Sales Insight.</td> 
  </tr> 
  <tr> 
   <td>E-mail de vente reçu</td> 
   <td>Un courrier électronique a été reçu et consigné par le représentant commercial dans le module externe MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Le terme &quot;courrier électronique de vente reçu&quot; **ne signifie pas** livraison. L&#39;état remis n&#39;est pas capturé pour les courriers électroniques envoyés via Sales Insight.

>[!TIP]
>
>Si vous souhaitez obtenir plus d&#39;informations Marketo dans Salesforce, consultez notre [produit Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md).
