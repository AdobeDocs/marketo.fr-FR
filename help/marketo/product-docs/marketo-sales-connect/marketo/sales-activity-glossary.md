---
description: Glossaire des activités commerciales - Documents Marketo - Documentation du produit
title: Glossaire des activités de vente
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 7%

---

# Glossaire des activités de vente {#sales-activity-glossary}

Dans Sales Connect, lorsqu’un vendeur : ajoute un prospect à une cadence de vente, lui envoie un e-mail ou passe un appel dans le cadre d’une activité, il est enregistré dans l’historique des activités Marketo. En outre, lorsque le prospect consulte des e-mails, les ouvertures, les clics et les réponses sont également consignés.

Les activités ci-dessous seront consignées dans le Marketo à partir de [!DNL Sales Connect].

>[!NOTE]
>
>Ces activités et attributs peuvent être consommés à partir de notre API REST et Bulk.

## Activités {#activities}

<table>
 <tr>
  <th>Activité Sales</th>
  <th>Attribut</th>
 </tr>
 <tr>
  <th rowspan="9">Envoyer un e-mail de vente</th>
  <td>[!UICONTROL Envoyé Par]</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>URL [!UICONTROL Sales Template]</td>
 </tr>
 <tr>
  <td>URL [!UICONTROL Sales Campaign]</td>
 </tr>
 <tr>
  <td>Nom du modèle de vente </td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="9"> Ouvrir l’e-mail commercial</th>
  <td>[!UICONTROL Envoyé Par]</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="10">E-mail de vente cliqué</th>
  <td>[!UICONTROL Link]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Envoyé Par]</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
<tr>
  <th rowspan="3">A répondu à l'e-mail commercial</th>
  <td>[!UICONTROL Reçu Par]</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="11">Appel de vente reçu</th>
  <td>[!UICONTROL Sales Call Made By]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Numéro de téléphone commercial appelé]</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Duration]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Recording URL]</td>
 </tr>
  <tr>
  <td>[!UICONTROL Sales Call Answered By]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="6">Ajouter à la campagne de ventes</th>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Envoyé Par]</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign ID]</td>
 </tr>
 <tr>
  <th rowspan="6">Supprimer de la campagne de ventes</th>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Envoyé Par]</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign ID]</td>
 </tr>
 <tr>
  <th rowspan="5">E-mail de rebond de ventes</th>
  <td>Détails</td>
 </tr>
 <tr>
  <td>E-mail</td>
 </tr>
 <tr>
  <td>Envoyé par</td>
 </tr>
 <tr>
  <td>Identifiant du vendeur Marketo</td>
 </tr>
 <tr>
  <td>ID du modèle</td>
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
   <td><strong>[!UICONTROL Details]</strong></td>
   <td>Détails du message d’erreur de rebond.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Email]</strong></td>
   <td>Adresse e-mail ayant fait l’objet d’un rebond.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Link]</strong></td>
   <td>URL sur laquelle l’utilisateur a cliqué.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Marketo Sales Person ID]</strong></td>
   <td>ID unique de l’enregistrement de personne dans [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Reçu Par]</strong></td>
   <td>Adresse électronique de la personne qui a envoyé l’e-mail.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Answered By]</strong></td>
   <td>Nom de la personne qui a répondu à l’appel.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Duration]</strong></td>
   <td>Durée de l’appel en secondes.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Made By]</strong></td>
   <td>Adresse électronique du vendeur qui a passé l'appel.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Recording URL]</strong></td>
   <td>URL de l’enregistrement des appels.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Status]</strong></td>
   <td>Enregistre le statut de l’appel final qui inclut : terminé, pas de réponse, annulé, échec.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Subject]</strong></td>
   <td>Résultat de l’appel sélectionné par un commercial dans le composeur.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign ID]</strong></td>
   <td>ID unique de la ressource de campagne de vente en [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign Name]</strong></td>
   <td>Nom de la campagne de vente.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign URL]</strong></td>
   <td>[!DNL Sales Connect] URL de la campagne de vente.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Email Subject]</strong></td>
   <td>Ligne d'objet de l'e-mail suivie d'un identifiant unique (par exemple : Mon objet (MSC-12345678)</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Numéro de téléphone commercial appelé]</strong></td>
   <td>Numéro de téléphone appelé par le service des ventes.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Template Name]</strong></td>
   <td>Nom du modèle d’e-mail en [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Template URL]</strong></td>
   <td>[!DNL Sales Connect] URL du modèle d’e-mail.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Envoyé Par]</strong></td>
   <td>Adresse électronique de la personne qui a envoyé l’e-mail.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Source]</strong></td>
   <td>Source de l’activité. Sera défini comme « Tout » pour les activités [!DNL Sales Connect] avant la version d’octobre 2021. Sera une « application de vente » pour les activités [!DNL Sales Connect] après la version d’octobre 2021.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Template ID]</strong></td>
   <td>Lorsque la source est Tout, l’ID du modèle est l’ID du modèle [!DNL Marketo Sales Connect]. Utilisez cette option pour cibler un modèle spécifique plutôt qu’une ligne d’objet, qui peut exister dans plusieurs modèles.
</td>
  </tr>
 </tbody>
</table>
