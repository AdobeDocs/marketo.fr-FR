---
description: Glossaire des activités d’actions Insight Sales - Documents Marketo - Documentation du produit
title: Glossaire de l’activité Actions de Sales Insight
exl-id: fd0f632c-6f0d-49f9-a805-0730595c81fd
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 4%

---

# Glossaire des activités [!DNL Sales Insight Actions] {#sales-insight-actions-activity-glossary}

En [!DNL Sales Insight Actions], lorsqu’un vendeur : ajoute un prospect à une campagne de vente, lui envoie un e-mail de vente ou passe un appel de vente sortant, il est enregistré dans l’historique des activités Marketo de ce prospect. En outre, lorsque le prospect consulte des e-mails, des ouvertures, des clics et des réponses, il est également consigné.

Les activités ci-dessous seront consignées dans le Marketo à partir de [!DNL Sales Insight Actions].

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
  <th rowspan="9">[!UICONTROL Send Sales Email]</th>
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
  <th rowspan="9">[!UICONTROL Open Sales Email]</th>
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
  <th rowspan="10">[!UICONTROL Clicked Sales Email]</th>
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
  <th rowspan="3">[!UICONTROL a répondu à un e-mail de vente]</th>
  <td>[!UICONTROL Reçu Par]</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="11">[!UICONTROL A Reçu Un Appel De Vente]</th>
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
  <th rowspan="6">[!UICONTROL Ajouter à la campagne de vente]</th>
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
  <th rowspan="6">[!UICONTROL Supprimer de la campagne de vente]</th>
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
   <td>ID unique de l’enregistrement de personne dans [!DNL Sales Insight Actions].</td> 
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
   <td>ID unique de la ressource de campagne de vente en [!DNL Sales Insight Actions].</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Campaign Name]</strong></td> 
   <td>Nom de la campagne de vente.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Campaign URL]</strong></td> 
   <td>[!DNL Sales Insight Actions] URL de la campagne de vente.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Email Subject]</strong></td> 
   <td>Objet de l’e-mail suivi d’un ID unique (par exemple : Mon objet (SIA-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Numéro de téléphone commercial appelé]</strong></td> 
   <td>Numéro de téléphone appelé par le service des ventes.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Template Name]</strong></td> 
   <td>Nom du modèle d’e-mail en [!DNL Sales Insight Actions].</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Template URL]</strong></td> 
   <td>[!DNL Sales Insight Actions] URL du modèle d’e-mail.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Envoyé Par]</strong></td>
   <td>Adresse électronique de la personne qui a envoyé l’e-mail.</td> 
  </tr> 
  <tr> 
   <td><strong>Source</strong></td> 
   <td>Source de l’activité. Sera défini comme « Tout » pour les activités [!DNL Sales Insight Actions] avant la version d’octobre 2021. Sera une « application de vente » pour les activités [!DNL Sales Insight Actions] après la version d’octobre 2021.</td>
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Template ID]</strong></td> 
   <td>Lorsque la source est Tout, l’ID du modèle est l’ID du modèle [!DNL Marketo Sales Insight Actions]. Utilisez cette option pour cibler un modèle spécifique plutôt qu’une ligne d’objet, qui peut exister dans plusieurs modèles.
</td> 
  </tr> 
 </tbody> 
</table>
