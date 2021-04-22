---
description: Mappage des champs de dynamique par défaut - Docs Marketo - Documentation du produit
title: Mappage de champ dynamique par défaut
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 47%

---

# Mappage de champ dynamique par défaut {#default-dynamics-field-mapping}

Lors de la synchronisation initiale de votre compte Marketo avec Microsoft, Marketo crée automatiquement ces associations entre vos champs Dynamics intégrés et Marketo.  Marketo synchronise également vos champs personnalisés sur vos pistes, comptes, opportunités et contacts.

## Champs de leads {#lead-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Champ Marketo</th> 
   <th>Champ MS Dynamics</th> 
   <th>Nom de l'API MS Dynamics</th> 
  </tr> 
  <tr> 
   <td>Date de création - Microsoft</td> 
   <td>Date de création</td> 
   <td>créé</td> 
  </tr> 
  <tr> 
   <td>Titre</td> 
   <td>Titre</td> 
   <td>salutation</td> 
  </tr> 
  <tr> 
   <td>Prénom</td> 
   <td>Prénom</td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>Deuxième</td> 
   <td>Deuxième prénom</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Nom</td> 
   <td>Nom</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>Email</td> 
   <td>Courriel</td> 
   <td>email address1</td> 
  </tr> 
  <tr> 
   <td>Intitulé du poste</td> 
   <td>Intitulé du poste</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Téléphone</td> 
   <td>Téléphone de l'entreprise
</td> 
   <td>téléphone1</td> 
  </tr> 
  <tr> 
   <td>Mobile</td> 
   <td>Téléphone mobile</td> 
   <td>téléphone mobile</td> 
  </tr> 
  <tr> 
   <td>Fax</td> 
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
   <td>Pays</td> 
   <td>État/province</td> 
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
   <td>Source de personne</td> 
   <td>Source du lead</td> 
   <td>leadsourcecode</td> 
  </tr> 
  <tr> 
   <td>Statut Individu</td> 
   <td>Statut</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>Raison du statut</td> 
   <td>Raison du statut</td> 
   <td>statuscode</td> 
  </tr> 
  <tr> 
   <td>Notes du contact</td> 
   <td>Description</td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td>Ne pas appeler</td> 
   <td>Ne pas autoriser les appels téléphoniques</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>Désabonnement</td> 
   <td>Ne pas envoyer de courrier électronique en masse</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Évaluation d’un individu</td> 
   <td>Classement</td> 
   <td>code qualité</td> 
  </tr> 
  <tr> 
   <td>Adresse 2 - Microsoft</td> 
   <td>Rue 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Adresse 3 - Microsoft</td> 
   <td>Rue 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Ne Pas Envoyer d'e-mail - Microsoft </td> 
   <td>Ne pas autoriser les courriers électroniques</td> 
   <td>donotemail</td> 
  </tr> 
  <tr> 
   <td>Ne Pas Faxer - Microsoft </td> 
   <td>Ne pas autoriser les télécopies</td> 
   <td>donotfax</td> 
  </tr> 
  <tr> 
   <td>Ne pas envoyer de contenu marketing - Microsoft </td> 
   <td>Matériel marketing</td> 
   <td>donotsendmm</td> 
  </tr> 
  <tr> 
   <td>Téléphone du domicile - Microsoft </td> 
   <td>Téléphone du domicile </td> 
   <td>téléphone2</td> 
  </tr> 
  <tr> 
   <td>Méthode De Contact Préférée À Microsoft</td> 
   <td>Mode de communication privilégié</td> 
   <td>préférredcontactmethod code</td> 
  </tr> 
  <tr> 
   <td>Sujet Microsoft</td> 
   <td>Thème</td> 
   <td>objet</td> 
  </tr> 
 </tbody> 
</table>

## Champs contact {#contact-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Champ Marketo</th> 
   <th>Champ MS Dynamics</th> 
   <th>Nom de l'API MS Dynamics</th> 
  </tr> 
  <tr> 
   <td>Date de création - Microsoft</td> 
   <td>Date de création</td> 
   <td>créé</td> 
  </tr> 
  <tr> 
   <td>Titre</td> 
   <td>Titre</td> 
   <td>salutation</td> 
  </tr> 
  <tr> 
   <td>Prénom</td> 
   <td>Prénom</td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>Deuxième</td> 
   <td>Deuxième prénom</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Nom</td> 
   <td>Nom</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>Courriel</td> 
   <td>Courriel</td> 
   <td>email address1</td> 
  </tr> 
  <tr> 
   <td>Intitulé du poste</td> 
   <td>Intitulé du poste</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Téléphone</td> 
   <td>Téléphone de l'entreprise
</td> 
   <td>téléphone1</td> 
  </tr> 
  <tr> 
   <td>Mobile</td> 
   <td>Téléphone mobile</td> 
   <td>téléphone mobile</td> 
  </tr> 
  <tr> 
   <td>Adresse</td> 
   <td>Adresse 1 : Voie 1</td> 
   <td>address1_line1</td> 
   <tr> 
   <td>Ville</td> 
   <td>Adresse 1 : Ville</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>Pays</td> 
   <td>Adresse 1 : État/Province</td> 
   <td>address1_stateorprovince</td> 
  </tr> 
  <tr> 
   <td>Pays</td> 
   <td>Adresse 1 : Pays/région</td> 
   <td>address1_country</td> 
   <tr> 
   <td>Code postal</td> 
   <td>Adresse 1 : Code postal</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Statut Individu</td> 
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
   <td>Désabonnement</td> 
   <td>Ne pas envoyer de courrier électronique en masse</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Adresse 2 - Microsoft</td> 
   <td>Adresse 1 : Voie 2</td> 
   <td>address1_line2</td> 
  </tr> 
   <tr> 
   <td>Adresse 3 - Microsoft</td> 
   <td>Adresse 1 : Voie 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Ne Pas Envoyer d'e-mail - Microsoft </td> 
   <td>Ne pas autoriser les courriers électroniques</td> 
   <td>donotemail</td> 
  </tr> 
  <tr> 
   <td>Téléphone du domicile - Microsoft </td> 
   <td>Téléphone du domicile </td> 
   <td>téléphone2</td> 
  </tr> 
  <tr> 
   <td>Méthode De Contact Préférée À Microsoft</td> 
   <td>Méthode De Contact Préférée</td> 
   <td>préférredcontactmethod code</td> 
  </tr> 
 </tbody> 
</table>

## Champs de compte {#account-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Champ Marketo</th> 
   <th>Champ MS Dynamics</th> 
   <th>Nom de l'API MS Dynamics</th> 
  </tr> 
  <tr> 
   <td>Compte (a)</td> 
   <td>Compte</td> 
   <td>accountid</td> 
  </tr> 
  <tr> 
   <td>Adresse de facturation</td> 
   <td>Adresse 1 : Voie 1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>Ville de facturation</td> 
   <td>Adresse 1 : Ville</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>Pays de facturation</td> 
   <td>Adresse 1 : Pays/région</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>Code postal de facturation</td> 
   <td>Adresse 1 : Code postal</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Adresse de facturation 2 - Microsoft</td> 
   <td>Adresse 1 : Voie 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Adresse de facturation 3 - Microsoft</td> 
   <td>Adresse 1 : Voie 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Téléphone principal</td> 
   <td>Téléphone principal</td> 
   <td>téléphone1</td> 
  </tr> 
  <tr> 
   <td>Type d’entreprise</td> 
   <td>Type d’entreprise</td> 
   <td>business-stypecode</td> 
  </tr> 
  <tr> 
   <td>Numéro de compte Microsoft</td> 
   <td>Numéro de compte</td> 
   <td>numéro de compte</td> 
  </tr> 
  <tr> 
   <td>Statut de la société Microsoft</td> 
   <td>Statut</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>Chiffre d'affaires annuel</td> 
   <td>Chiffre d'affaires annuel</td> 
   <td>chiffre d’affaires</td> 
  </tr> 
  <tr> 
   <td>Notes sur société</td> 
   <td>Description</td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td>Secteur</td> 
   <td>Secteur</td> 
   <td>code industriel</td> 
  </tr> 
  <tr> 
   <td>Code SIC</td> 
   <td>Code SIC</td> 
   <td>sic</td> 
  </tr> 
  <tr> 
   <td>Site Internet</td> 
   <td>Site Internet</td> 
   <td>site</td> 
  </tr> 
 </tbody> 
</table>

## Champs système liés à Microsoft dans Marketo (lecture seule) {#microsoft-related-system-fields-in-marketo}

Ces champs sont créés dans Marketo mais ne peuvent pas être ajustés par les clients.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Champ Marketo</th> 
   <th>Description</th> 
  </tr> 
  <tr> 
   <td>Type Microsoft</td> 
   <td>Piste ou Contact. S'il est vide, le prospect n'existe qu'en tant que personne à Marketo</td> 
  </tr> 
  <tr> 
   <td>Date de création - Microsoft</td> 
   <td>Date créée dans MS Dynamics (peut être différente de la date créée dans Marketo)</td> 
  </tr> 
  <tr> 
   <td>Microsoft est supprimé</td> 
   <td>La personne se trouvait auparavant dans Microsoft mais a été supprimée et vit maintenant uniquement à Marketo.</td> 
  </tr> 
 </tbody> 
</table>
