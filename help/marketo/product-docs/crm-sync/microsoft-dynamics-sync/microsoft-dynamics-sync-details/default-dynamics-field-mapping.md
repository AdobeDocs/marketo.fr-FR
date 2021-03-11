---
description: Mappage des champs Dynamics par défaut - Documents marketing - Documentation du produit
title: Mappage de champ dynamique par défaut
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 1%

---


# Mappage de champ dynamique par défaut {#default-dynamics-field-mapping}

Lors de la synchronisation initiale de votre compte Marketo avec Microsoft, Marketo crée automatiquement ces associations entre vos champs Dynamics intégrés et Marketo.  Marketo synchronise également vos champs personnalisés sur vos pistes, comptes, opportunités et contacts.

## Champs de piste {#lead-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Champ marketing</th> 
   <th>Champ MS Dynamics</th> 
   <th>Nom de l'API MS Dynamics</th> 
  </tr> 
  <tr> 
   <td>Date de création Microsoft</td> 
   <td>Créé le</td> 
   <td>créé</td> 
  </tr> 
  <tr> 
   <td>Salutation</td> 
   <td>Salutation</td> 
   <td>salutation</td> 
  </tr> 
  <tr> 
   <td>Premier</td> 
   <td>Prénom</td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>Moyen</td> 
   <td>Nom du milieu</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Dernier</td> 
   <td>Nom</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>Courriel</td> 
   <td>Courriel</td> 
   <td>email address1</td> 
  </tr> 
  <tr> 
   <td>Titre de la tâche</td> 
   <td>Titre de la tâche</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Téléphone</td> 
   <td>Téléphone professionnel</td> 
   <td>téléphone1</td> 
  </tr> 
  <tr> 
   <td>Mobile</td> 
   <td>Téléphone mobile</td> 
   <td>téléphone mobile</td> 
  </tr> 
  <tr> 
   <td>Télécopie</td> 
   <td>Télécopie</td> 
   <td>télécopieur</td> 
  </tr> 
  <tr> 
   <td>Adresse</td> 
   <td>Rue 1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>Ville</td> 
   <td>Ville</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>État</td> 
   <td>Etat/Province</td> 
   <td>address1_stateorprovince</td> 
  </tr> 
  <tr> 
   <td>Pays</td> 
   <td>Pays/région</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>Code postal</td> 
   <td>Code postal</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Source de la personne</td> 
   <td>Source du prospect</td> 
   <td>leadsourcecode</td> 
  </tr> 
  <tr> 
   <td>Statut de la personne</td> 
   <td>Statut</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>Raison du statut</td> 
   <td>Raison du statut</td> 
   <td>statuscode</td> 
  </tr> 
  <tr> 
   <td>Notes sur les personnes</td> 
   <td>Description</td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td>Ne pas appeler</td> 
   <td>Ne pas autoriser les appels téléphoniques</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>Non abonné</td> 
   <td>Ne pas envoyer de courrier électronique en masse</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Évaluation de personne</td> 
   <td>Évaluation</td> 
   <td>code qualité</td> 
  </tr> 
  <tr> 
   <td>Adresse Microsoft 2</td> 
   <td>Rue 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Adresse Microsoft 3</td> 
   <td>Rue 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft Ne pas envoyer de courrier électronique</td> 
   <td>Ne pas autoriser les courriers électroniques</td> 
   <td>donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft ne télécopie pas</td> 
   <td>Ne pas autoriser les télécopies</td> 
   <td>donotfax</td> 
  </tr> 
  <tr> 
   <td>Microsoft n'envoie pas de matériel marketing</td> 
   <td>Matériel marketing</td> 
   <td>donotsendmm</td> 
  </tr> 
  <tr> 
   <td>Téléphone Microsoft Home</td> 
   <td>Téléphone d’accueil</td> 
   <td>téléphone2</td> 
  </tr> 
  <tr> 
   <td>Méthode De Contact Préférée À Microsoft</td> 
   <td>Méthode de contact préférée</td> 
   <td>préférredcontactmethod code</td> 
  </tr> 
  <tr> 
   <td>Rubrique Microsoft</td> 
   <td>Rubrique</td> 
   <td>objet</td> 
  </tr> 
 </tbody> 
</table>

## Champs de contact {#contact-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Champ marketing</th> 
   <th>Champ MS Dynamics</th> 
   <th>Nom de l'API MS Dynamics</th> 
  </tr> 
  <tr> 
   <td>Date de création Microsoft</td> 
   <td>Créé le</td> 
   <td>créé</td> 
  </tr> 
  <tr> 
   <td>Salutation</td> 
   <td>Salutation</td> 
   <td>salutation</td> 
  </tr> 
  <tr> 
   <td>Premier</td> 
   <td>Prénom</td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>Moyen</td> 
   <td>Nom du milieu</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Dernier</td> 
   <td>Nom</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>Courriel</td> 
   <td>Courriel</td> 
   <td>email address1</td> 
  </tr> 
  <tr> 
   <td>Titre de la tâche</td> 
   <td>Titre de la tâche</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Téléphone</td> 
   <td>Téléphone professionnel</td> 
   <td>téléphone1</td> 
  </tr> 
  <tr> 
   <td>Mobile</td> 
   <td>Téléphone mobile</td> 
   <td>téléphone mobile</td> 
  </tr> 
  <tr> 
   <td>Adresse</td> 
   <td>Adresse 1 : Rue 1</td> 
   <td>address1_line1</td> 
   <tr> 
   <td>Ville</td> 
   <td>Adresse 1 : Ville</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>État</td> 
   <td>Adresse 1 : Etat/Province</td> 
   <td>address1_stateorprovince</td> 
  </tr> 
  <tr> 
   <td>Pays</td> 
   <td>Adresse 1 : Pays/région</td> 
   <td>address1_country</td> 
   <tr> 
   <td>Code postal</td> 
   <td>Adresse 1 : Code postal</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Statut de la personne</td> 
   <td>Statut</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>Raison du statut</td> 
   <td>Raison du statut</td> 
   <td>statuscode</td> 
  </tr> 
   <tr> 
   <td>Ne pas appeler</td> 
   <td>Ne pas autoriser les appels téléphoniques</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>Non abonné</td> 
   <td>Ne pas envoyer de courrier électronique en masse</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Adresse Microsoft 2</td> 
   <td>Adresse 1 : Rue 2</td> 
   <td>address1_line2</td> 
  </tr> 
   <tr> 
   <td>Adresse Microsoft 3</td> 
   <td>Adresse 1 : Rue 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft Ne pas envoyer de courrier électronique</td> 
   <td>Ne pas autoriser les courriers électroniques</td> 
   <td>donotemail</td> 
  </tr> 
  <tr> 
   <td>Téléphone Microsoft Home</td> 
   <td>Téléphone d’accueil</td> 
   <td>téléphone2</td> 
  </tr> 
  <tr> 
   <td>Méthode De Contact Préférée À Microsoft</td> 
   <td>Méthode De Contact Préférée</td> 
   <td>préférredcontactmethod code</td> 
  </tr> 
 </tbody> 
</table>

## Champs du compte {#account-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Champ marketing</th> 
   <th>Champ MS Dynamics</th> 
   <th>Nom de l'API MS Dynamics</th> 
  </tr> 
  <tr> 
   <td>Compte a)</td> 
   <td>Compte</td> 
   <td>accountid</td> 
  </tr> 
  <tr> 
   <td>Adresse de facturation</td> 
   <td>Adresse 1 : Rue 1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>Ville de facturation</td> 
   <td>Adresse 1 : Ville</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>Pays de facturation</td> 
   <td>Adresse 1 : Pays/région</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>Code postal de facturation</td> 
   <td>Adresse 1 : Code postal</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Adresse de facturation Microsoft 2</td> 
   <td>Adresse 1 : Rue 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Adresse de facturation Microsoft 3</td> 
   <td>Adresse 1 : Rue 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Téléphone principal</td> 
   <td>Téléphone principal</td> 
   <td>téléphone1</td> 
  </tr> 
  <tr> 
   <td>Type d'entreprise</td> 
   <td>Type d'entreprise</td> 
   <td>business-stypecode</td> 
  </tr> 
  <tr> 
   <td>Numéro de compte Microsoft</td> 
   <td>Numéro de compte</td> 
   <td>numéro de compte</td> 
  </tr> 
  <tr> 
   <td>État de la Société Microsoft</td> 
   <td>Statut</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>Recettes annuelles</td> 
   <td>Recettes annuelles</td> 
   <td>recette</td> 
  </tr> 
  <tr> 
   <td>Notes de société</td> 
   <td>Description</td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td>Industrie</td> 
   <td>Industrie</td> 
   <td>code industriel</td> 
  </tr> 
  <tr> 
   <td>Code SIC</td> 
   <td>Code SIC</td> 
   <td>sic</td> 
  </tr> 
  <tr> 
   <td>Site Web</td> 
   <td>Site Web</td> 
   <td>site</td> 
  </tr> 
 </tbody> 
</table>

## Champs système liés à Microsoft dans Marketo (lecture seule) {#microsoft-related-system-fields-in-marketo}

Ces champs sont créés dans Marketing mais ne peuvent pas être ajustés par les clients.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Champ marketing</th> 
   <th>Description</th> 
  </tr> 
  <tr> 
   <td>Type Microsoft</td> 
   <td>Piste ou Contact. S'il est vide, le prospect n'existe qu'en tant que personne sur le marché</td> 
  </tr> 
  <tr> 
   <td>Date de création Microsoft</td> 
   <td>Date créée dans MS Dynamics (peut être différente de la date créée dans Marketo)</td> 
  </tr> 
  <tr> 
   <td>Microsoft est supprimé</td> 
   <td>La personne était dans Microsoft mais a été supprimée et vit maintenant uniquement dans Marketo.</td> 
  </tr> 
 </tbody> 
</table>
