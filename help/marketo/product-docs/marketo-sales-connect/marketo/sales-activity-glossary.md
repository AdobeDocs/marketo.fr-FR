---
description: Glossaire des activités de vente - Documents Marketo - Documentation produit
title: Glossaire des activités de vente
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: 42ddb44100a041a09ff4a68c02ccf6aabb2d953e
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 12%

---

# Glossaire des activités de vente {#sales-activity-glossary}

Dans Sales Connect, lorsqu&#39;un vendeur : ajoute une piste à une cadence de vente, leur envoie un e-mail ou effectue un appel à une activité, elle sera enregistrée dans l&#39;historique des activités Marketo. En outre, lorsque le prospect s’engage avec des e-mails, s’ouvre, les clics et les réponses sont également enregistrés.

Les activités ci-dessous seront enregistrées sur Marketo à partir de Sales Connect.

>[!NOTE]
>
>Ces activités et ces attributs peuvent être consommés à partir de notre API REST et Bulk.

## Activités {#activities}

<table>
 <tr>
  <th>Activité de vente</th>
  <th>Attribut</th>
 </tr>
 <tr>
  <th rowspan="9">Envoyer un e-mail de vente</th>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>ID du modèle</td>
 </tr>
 <tr>
  <td>URL du modèle de vente</td>
 </tr>
 <tr>
  <td>URL de campagne de vente</td>
 </tr>
 <tr>
  <td>Nom du modèle de vente</td>
 </tr>
 <tr>
  <td>Objet de la messagerie</td>
 </tr>
 <tr>
  <td>Nom de la campagne de vente</td>
 </tr>
 <tr>
  <td>ID de personne commerciale Marketo</td>
 </tr>
 <tr>
  <th rowspan="9">Ouvrir e-mail de vente</th>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>ID du modèle</td>
 </tr>
 <tr>
  <td>URL du modèle de vente</td>
 </tr>
 <tr>
  <td>URL de campagne de vente</td>
 </tr>
 <tr>
  <td>Nom du modèle de vente</td>
 </tr>
 <tr>
  <td>Objet de la messagerie</td>
 </tr>
 <tr>
  <td>Nom de la campagne de vente</td>
 </tr>
 <tr>
  <td>ID de personne commerciale Marketo</td>
 </tr>
 <tr>
  <th rowspan="10">E-mail de vente cliqué</th>
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
  <td>URL du modèle de vente</td>
 </tr>
 <tr>
  <td>URL de campagne de vente</td>
 </tr>
 <tr>
  <td>Nom du modèle de vente</td>
 </tr>
 <tr>
  <td>Objet de la messagerie</td>
 </tr>
 <tr>
  <td>Nom de la campagne de vente</td>
 </tr>
 <tr>
  <td>ID de personne commerciale Marketo</td>
 </tr>
<tr>
  <th rowspan="3">Réponse à l'e-mail de vente</th>
  <td>Reçu par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>ID de personne commerciale Marketo</td>
 </tr>
 <tr>
  <th rowspan="11">Appel de vente reçu</th>
  <td>Appel  Sales passé par</td>
 </tr>
 <tr>
  <td>Statut de l'appel de vente</td>
 </tr>
 <tr>
  <td>Objet d'appel de vente</td>
 </tr>
 <tr>
  <td>Nom de la campagne de vente</td>
 </tr>
 <tr>
  <td>URL de campagne de vente</td>
 </tr>
 <tr>
  <td>Numéro de téléphone de vente appelé</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>Durée de l'appel de vente</td>
 </tr>
 <tr>
  <td>URL de l’enregistrement de l’appel  Sales</td>
 </tr>
  <tr>
  <td>Réponse à l’appel  Sales par</td>
 </tr>
 <tr>
  <td>ID de personne commerciale Marketo</td>
 </tr>
 <tr>
  <th rowspan="6">Ajouter à la campagne de ventes</th>
  <td>Nom de la campagne de vente</td>
 </tr>
 <tr>
  <td>Statut de l'appel de vente</td>
 </tr>
 <tr>
  <td>URL de campagne de vente</td>
 </tr>
 <tr>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>ID campagne de vente</td>
 </tr>
 <tr>
  <th rowspan="6">Supprimer de la campagne Ventes</th>
  <td>Nom de la campagne de vente</td>
 </tr>
 <tr>
  <td>Statut de l'appel de vente</td>
 </tr>
 <tr>
  <td>URL de campagne de vente</td>
 </tr>
 <tr>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>ID campagne de vente</td>
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
   <td><strong>Détails</strong></td> 
   <td>Détails du message d’erreur Rebond.</td> 
  </tr> 
  <tr> 
   <td><strong>Adresse e-mail</strong></td> 
   <td>Adresse électronique qui a rebondi.</td> 
  </tr> 
  <tr> 
   <td><strong>Lien</strong></td> 
   <td>URL sur laquelle l’utilisateur a cliqué.</td> 
  </tr> 
  <tr> 
   <td><strong>ID de personne commerciale Marketo</strong></td> 
   <td>ID unique pour l'enregistrement de personne dans Sales Connect.</td> 
  </tr> 
  <tr> 
   <td><strong>Reçu par</strong></td> 
   <td>Adresse électronique de la personne qui a envoyé l’adresse électronique.</td> 
  </tr>
  <tr> 
   <td><strong>Réponse à l’appel  Sales par</strong></td> 
   <td>Nom de la personne qui a répondu à l'appel.</td> 
  </tr>
  <tr> 
   <td><strong>Durée de l'appel de vente</strong></td> 
   <td>Durée de l'appel en secondes.</td> 
  </tr>
  <tr> 
   <td><strong>Appel  Sales passé par</strong></td> 
   <td>Adresse électronique du vendeur qui a passé l'appel.</td> 
  </tr>
  <tr> 
   <td><strong>URL de l’enregistrement de l’appel  Sales</strong></td> 
   <td>URL de l’enregistrement des appels.</td> 
  </tr>
  <tr> 
   <td><strong>Statut de l'appel de vente</strong></td> 
   <td>Enregistrer l'état d'appel final de l'appel, qui inclut : terminé, aucune réponse, annulé, échec.</td> 
  </tr>
  <tr> 
   <td><strong>Objet d'appel de vente</strong></td> 
   <td>Résultat d'appel sélectionné par un utilisateur commercial dans le dialer.</td> 
  </tr>
  <tr> 
   <td><strong>ID campagne de vente</strong></td> 
   <td>ID unique pour l’actif Sales Campaign dans Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>Nom de la campagne de vente</strong></td> 
   <td>Nom de la campagne de vente.</td> 
  </tr>
  <tr> 
   <td><strong>URL de campagne de vente</strong></td> 
   <td>URL Sales Connect pour Sales Campaign.</td> 
  </tr>
  <tr> 
   <td><strong>Objet de courriel de vente</strong></td> 
   <td>Objet de la ligne de courrier électronique.</td> 
  </tr>
  <tr> 
   <td><strong>Numéro de téléphone de vente appelé</strong></td> 
   <td>Numéro de téléphone appelé par le service commercial.</td> 
  </tr>
  <tr> 
   <td><strong>Nom du modèle de vente</strong></td> 
   <td>Nom du modèle d'e-mail dans Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>URL du modèle de vente</strong></td> 
   <td>URL Sales Connect pour le modèle d’e-mail.</td> 
  </tr>
  <tr> 
   <td><strong>Envoyé par</strong></td>
   <td>Adresse électronique de la personne qui a envoyé l’adresse électronique.</td> 
  </tr> 
  <tr> 
   <td><strong>Source</strong></td> 
   <td>Source de l'activité. Sera défini sur "Tout" pour les activités Sales Connect.</td> 
  </tr> 
  <tr> 
   <td><strong>ID du modèle</strong></td> 
   <td>Lorsque la source est Tout, l’ID de modèle est l’ID de modèle Marketo Sales Connect. Utilisez cette option pour cibler un modèle spécifique au lieu d’une ligne d’objet, qui pourrait exister dans plusieurs modèles.
</td> 
  </tr> 
 </tbody> 
</table>
