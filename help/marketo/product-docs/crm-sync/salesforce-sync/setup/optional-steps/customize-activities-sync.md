---
unique-page-id: 4719294
description: Synchronisation des Activités personnalisées - Documentation marketing - Documentation du produit
title: Personnaliser la synchronisation des Activités
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---


# Synchronisation des Activités personnalisée {#customize-activities-sync}

Si vous n&#39;utilisez pas Marketing Insight Sales Insight, Marketo peut créer des enregistrements d&#39;historique des Activités de Salesforce pour certains événements. Voici comment les activer.

1. Accédez à **Admin**.

   ![](assets/admin.png)

1. Cliquez sur **Salesforce**, puis sur **Modifier les options de synchronisation**.

   ![](assets/two-1.png)

1. Cochez les cases en regard des activités que vous souhaitez que Marketo envoie à Salesforce, puis cliquez sur **Enregistrer**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Une fois activé, Marketo repoussera trois mois d&#39;activité historique. Selon la quantité de données, _cette opération peut prendre plusieurs jours._ Les mises à jour survenant pendant la transmission des Activités initiales peuvent être retardées jusqu’à la fin de la synchronisation des Activités initiales.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>Type d'Activité</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Formulaire rempli</td> 
   <td>Remplir tout formulaire de marketing</td> 
  </tr> 
  <tr> 
   <td>Ajouté à la liste</td> 
   <td><p>Étape de flux : A été ajouté à une liste statique</p></td> 
  </tr> 
  <tr> 
   <td>Courriel envoyé</td> 
   <td>Étape de flux : A été envoyé un courrier électronique</td> 
  </tr> 
  <tr> 
   <td>Livraison par courrier électronique</td> 
   <td>Réception d’un courrier électronique (sans retour)</td> 
  </tr> 
  <tr> 
   <td>E-mail ouvert</td> 
   <td>Ouverture d’un courrier électronique (sans bloquer les images)</td> 
  </tr> 
  <tr> 
   <td>Lien cliqué dans le courrier électronique</td> 
   <td>Cliquez sur un lien dans un courrier électronique envoyé par Marketo.</td> 
  </tr> 
  <tr> 
   <td>Supprimé de la liste</td> 
   <td>Étape de flux : A été supprimé d’une liste statique</td> 
  </tr> 
  <tr> 
   <td>Supprimer du flux</td> 
   <td>Étape de flux : Supprimer du flux</td> 
  </tr> 
  <tr> 
   <td>Adresse électronique de vente envoyée</td> 
   <td>A été envoyé par courrier électronique via Marketing Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Adresse électronique de vente ouverte</td> 
   <td>Ouverture d’un courrier électronique envoyé par l’intermédiaire de Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Cliquez sur le lien dans le courriel de vente</td> 
   <td>Cliquez sur un lien dans un courrier électronique envoyé par le biais de Marketing Cloud Sales Insight.</td> 
  </tr> 
  <tr> 
   <td>Adresse électronique de vente reçue</td> 
   <td>Un courrier électronique a été reçu et consigné par le représentant commercial dans le module externe MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Le terme &quot;courrier électronique de vente reçu&quot; **ne signifie pas** livraison. L&#39;état remis n&#39;est pas capturé pour les courriers électroniques envoyés via Sales Insight.

>[!TIP]
>
>Si vous souhaitez obtenir plus d&#39;informations sur le marketing dans Salesforce, consultez notre [produit Marketing Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md).
