---
description: Glossaire des activités de vente - Documents Marketo - Documentation du produit
title: Glossaire des activités de vente
hide: true
hidefromtoc: true
source-git-commit: 70f17106efe52ee742c8e31013e533fc36ce9835
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 17%

---

# Glossaire des activités de vente {#sales-activity-glossary}

Dans Sales Connect, lorsqu’un vendeur : ajoute une piste à une cadence de vente, leur envoie un email ou lance un appel à une activité ; elle est consignée dans l’historique des activités de Marketo. En outre, lorsque le prospect s’engage avec des emails, des ouvertures, des clics et des réponses, est également consigné.

Les activités ci-dessous seront consignées dans Marketo à partir de Sales Connect.

>[!NOTE]
>
>Ces activités et attributs peuvent être utilisés à partir de nos API REST et Bulk.

## Activités {#activities}

<table>
 <tr>
  <th>Activité de vente</th>
  <th>Attribut</th>
 </tr>
 <tr>
  <th rowspan="3">Envoyer un e-mail de vente</th>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>ID du modèle</td>
 </tr>
 <tr>
  <th rowspan="3">Ouvrir e-mail de vente</th>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>ID du modèle</td>
 </tr>
 <tr>
  <th rowspan="4">Courrier électronique de vente cliqué</th>
  <td>Lien</td>
 </tr>
 <tr>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>ID du modèle</td>
 </tr>
 <tr>
  <th rowspan="2">Courrier électronique de vente reçu</th>
  <td>Reçu par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <th rowspan="4">E-mail de vente renvoyé</th>
  <td>Détails</td>
 </tr>
 <tr>
  <td>ID du modèle</td>
 </tr>
 <tr>
  <td>Adresse e-mail</td>
 </tr>
 <tr>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <th rowspan="7">Appel de vente reçu</th>
  <td>Appel  Sales passé par</td>
 </tr>
 <tr>
  <td>État des appels commerciaux</td>
 </tr>
 <tr>
  <td>Objet des appels commerciaux</td>
 </tr>
 <tr>
  <td>Nom de la campagne commerciale</td>
 </tr>
 <tr>
  <td>URL de la campagne de ventes</td>
 </tr>
 <tr>
  <td>Numéro de téléphone de vente appelé</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <th rowspan="6">Ajouter à la campagne de ventes</th>
  <td>Nom de la campagne commerciale</td>
 </tr>
 <tr>
  <td>État des appels commerciaux</td>
 </tr>
 <tr>
  <td>URL de la campagne de ventes</td>
 </tr>
 <tr>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>Identifiant de campagne de ventes</td>
 </tr>
 <tr>
  <th rowspan="6">Supprimer de la campagne de ventes</th>
  <td>Nom de la campagne commerciale</td>
 </tr>
 <tr>
  <td>État des appels commerciaux</td>
 </tr>
 <tr>
  <td>URL de la campagne de ventes</td>
 </tr>
 <tr>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>Identifiant de campagne de ventes</td>
 </tr>
</table>

## Descriptions {#descriptions}

<table> 
 <tr>
  <th>Attribut</th>
  <th>Description</th>
 </tr>
 <tbody> 
  <tr> 
   <td><strong>Envoyé par</strong></td>
   <td>Adresse électronique de la personne qui a envoyé l’adresse électronique.</td> 
  </tr> 
  <tr> 
   <td><strong>Source</strong></td> 
   <td>Source de l’activité. Définit comme "Tout" pour les activités de connexion aux ventes.</td> 
  </tr> 
  <tr> 
   <td><strong>ID du modèle</strong></td> 
   <td>Lorsque la source est Tout, l’ID de modèle est l’ID de modèle Marketo Sales Connect. Utilisez cette option pour cibler un modèle spécifique au lieu d’une ligne d’objet, qui peut exister dans plusieurs modèles.
</td> 
  </tr> 
  <tr> 
   <td><strong>Reçu par</strong></td> 
   <td>Adresse électronique de la personne qui a envoyé l’adresse électronique.</td> 
  </tr> 
  <tr> 
   <td><strong>Détails</strong></td> 
   <td>Détails du message d’erreur de rebond.</td> 
  </tr> 
  <tr> 
   <td><strong>Adresse e-mail</strong></td> 
   <td>Adresse électronique qui a fait l’objet d’un rebond.</td> 
  </tr> 
 </tbody> 
</table>