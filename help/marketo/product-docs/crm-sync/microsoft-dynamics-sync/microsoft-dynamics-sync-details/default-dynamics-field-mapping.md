---
description: Mappage des champs Dynamics par défaut - Documents Marketo - Documentation du produit
title: Mappage des champs Dynamics par défaut
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 09c70bb891f5cc93553c1f8dd0fb58dfd407fa81
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 42%

---

# Mappage des champs Dynamics par défaut {#default-dynamics-field-mapping}

Lors de la synchronisation initiale de votre compte Marketo avec Microsoft, Marketo effectue automatiquement ces associations entre vos champs Dynamics et Marketo intégrés.  Marketo synchronise également vos champs personnalisés sur vos pistes, comptes, opportunités et contacts.

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
      <th>Nom de l’API MS Dynamics</th>
    </tr>
    <tr>
      <td>Date de création - Microsoft</td>
      <td>Date de création</td>
      <td>created</td>
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
      <td>E-mail</td>
      <td>E-mail</td>
      <td>emailaddress1</td>
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
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Téléphone portable</td>
      <td>Téléphone mobile</td>
      <td>mobilphone</td>
    </tr>
    <tr>
      <td>Fax</td>
      <td>Fax</td>
      <td>fax</td>
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
      <td>État/province</td>
      <td>address1_statéorprovince</td>
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
      <td>lead sourcecode</td>
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
      <td>Désabonné</td>
      <td>Ne pas envoyer d’email en masse</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Évaluation d’un individu</td>
      <td>Classement</td>
      <td>qualitycode</td>
    </tr>
    <tr>
      <td>Adresse 2 - Microsoft</td>
      <td>Rue #2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Adresse 3 - Microsoft</td>
      <td>Rue 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Ne Pas Envoyer d'e-mail - Microsoft</td>
      <td>Ne pas autoriser les emails</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Ne Pas Faxer - Microsoft</td>
      <td>Ne pas autoriser les télécopieurs</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Ne Pas Envoyer de support marketing - Microsoft</td>
      <td>Matériel marketing</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Téléphone du domicile - Microsoft</td>
      <td>Téléphone du domicile </td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>Méthode De Contact Préférée À Microsoft</td>
      <td>Mode de communication privilégié</td>
      <td>preferred contactmethod code</td>
    </tr>
    <tr>
      <td>Sujet Microsoft</td>
      <td>Thème</td>
      <td>subject</td>
    </tr>
    <tr>
      <td>Date du dernier moment intéressant</td>
      <td>Date du dernier moment intéressant</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>Dernier moment intéressant desc</td>
      <td>Dernier moment intéressant desc</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>Dernier moment intéressant source</td>
      <td>Dernier moment intéressant source</td>
      <td>mkt_lead_interestingmomentsource</td>
    </tr>
    <tr>
      <td>Dernier moment intéressant</td>
      <td>Dernier moment intéressant</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>Société</td>
      <td>Nom de l’entreprise</td>
      <td>nomentreprise</td>
    </tr>
    <tr>
      <td>Évaluation relative</td>
      <td>Évaluation relative</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Priorité</td>
      <td>Priorité</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Urgence relative</td>
      <td>urgence</td>
      <td>mkt_urgence</td>
    </tr>
    <tr>
      <td>Objet</td>
      <td>Thème</td>
      <td>subject</td>
    </tr>
    <tr>
      <td>Chiffre d’affaires annuel</td>
      <td>Chiffre d’affaires annuel</td>
      <td>chiffre d’affaires</td>
    </tr>
  </tbody>
</table>

Les champs de piste ci-dessous sont synchronisés pour une utilisation interne.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Champ MS Dynamics</th>
      <th>Nom de l’API MS Dynamics</th>
    </tr>
    <tr>
      <td>Détenteur </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>created On</td>
      <td>created</td>
    </tr>
  </tbody>
</table>

## Champs de contact {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Champ Marketo</th>
      <th>Champ MS Dynamics</th>
      <th>Nom de l’API MS Dynamics</th>
    </tr>
    <tr>
      <td>Date de création - Microsoft</td>
      <td>Date de création</td>
      <td>created</td>
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
      <td>E-mail</td>
      <td>E-mail</td>
      <td>emailaddress1</td>
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
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Téléphone portable</td>
      <td>Téléphone mobile</td>
      <td>mobilphone</td>
    </tr>
    <tr>
      <td>Adresse</td>
      <td>Adresse 1 : Voie 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Ville</td>
      <td>Adresse 1 : Ville</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>État</td>
      <td>Adresse 1 : État/Province</td>
      <td>address1_statéorprovince</td>
    </tr>
    <tr>
      <td>Pays</td>
      <td>Adresse 1 : Pays/région</td>
      <td>address1_country</td>
    </tr>
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
      <td>Désabonné</td>
      <td>Ne pas envoyer d’email en masse</td>
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
      <td>Ne Pas Envoyer d'e-mail - Microsoft</td>
      <td>Ne pas autoriser les emails</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Téléphone du domicile - Microsoft</td>
      <td>Téléphone du domicile </td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>Méthode De Contact Préférée À Microsoft</td>
      <td>Méthode De Contact Préférée</td>
      <td>preferred contactmethod code</td>
    </tr>
    <tr>
      <td>Date du dernier moment intéressant</td>
      <td>Date du dernier moment intéressant</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>Dernier moment intéressant</td>
      <td>Dernier moment intéressant</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>Dernier moment intéressant source</td>
      <td>Dernier moment intéressant source</td>
      <td>mkt_lead_interestingmomentsource</td>
    </tr>
    <tr>
      <td>Dernier moment intéressant desc</td>
      <td>Dernier moment intéressant desc</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>Ne Pas Envoyer de support marketing - Microsoft</td>
      <td>Matériel marketing</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Ne Pas Faxer - Microsoft</td>
      <td>Ne Pas Faxer - Microsoft</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Priorité</td>
      <td>Priorité</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Urgence relative</td>
      <td>urgence</td>
      <td>mkt_urgence</td>
    </tr>
    <tr>
      <td>Évaluation relative</td>
      <td>Évaluation relative</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Notes du contact</td>
      <td>Description</td>
      <td>description </td>
    </tr>
    <tr>
      <td>Évaluation en tant qu’individu</td>
      <td>Évaluation des leads</td>
      <td>mkt_lead</td>
    </tr>
    <tr>
      <td>Notes du contact</td>
      <td>Description</td>
      <td>description </td>
    </tr>
  </tbody>
</table>

Les champs Contact ci-dessous sont synchronisés pour une utilisation interne.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Champ MS Dynamics</th>
      <th>Nom de l’API MS Dynamics</th>
    </tr>
    <tr>
      <td>Détenteur </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>created On</td>
      <td>created</td>
    </tr>
    <tr>
      <td>parentcustomerid</td>
      <td>Nom de l’entreprise</td>
    </tr>
  </tbody>
</table>

## Champs de compte {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Champ Marketo</th>
      <th>Champ MS Dynamics</th>
      <th>Nom de l’API MS Dynamics</th>
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
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Type d’entreprise</td>
      <td>Type d’entreprise</td>
      <td>business esstypecode</td>
    </tr>
    <tr>
      <td>Numéro de compte Microsoft</td>
      <td>Numéro de compte</td>
      <td>accountnumber</td>
    </tr>
    <tr>
      <td>Statut de la société Microsoft</td>
      <td>Statut</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Chiffre d’affaires annuel</td>
      <td>Chiffre d’affaires annuel</td>
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
      <td>industrycode</td>
    </tr>
    <tr>
      <td>Code SIC</td>
      <td>Code SIC</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Site Internet</td>
      <td>Site Internet</td>
      <td>site web</td>
    </tr>
    <tr>
      <td>Nombre d’employés</td>
      <td>Nombre d’employés</td>
      <td>numberofemployee</td>
    </tr>
    <tr>
      <td>Code SIC</td>
      <td>Code SIC</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Société</td>
      <td>Nom du compte</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Nombre d’employés</td>
      <td>Nombre d’employés</td>
      <td>numberofemployee</td>
    </tr>
  </tbody>
</table>

Les champs Compte ci-dessous sont synchronisés pour une utilisation interne.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Champ MS Dynamics</th>
      <th>Nom de l’API MS Dynamics</th>
    </tr>
    <tr>
      <td>Détenteur </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>created On</td>
      <td>created</td>
    </tr>
  </tbody>
</table>

## Champs d’opportunités {#opportunity-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Champ Marketo</th>
      <th>Champ MS Dynamics</th>
      <th>Nom de l’API MS Dynamics</th>
    </tr>
    <tr>
      <td>Probabilité de fermeture</td>
      <td>La probabilité</td>
      <td>closeprobabilité</td>
    </tr>
    <tr>
      <td>Étape</td>
      <td>état</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Date de fermeture réelle</td>
      <td>Date de fermeture réelle</td>
      <td>actualclosedate</td>
    </tr>
    <tr>
      <td>Nom</td>
      <td>Thème</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Valeur estimée</td>
      <td>Estimation Recettes</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>Description</td>
      <td>Description</td>
      <td>description</td>
    </tr>
  </tbody>
</table>

Les champs Compte ci-dessous sont synchronisés pour une utilisation interne.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Champ MS Dynamics</th>
      <th>Nom de l’API MS Dynamics</th>
    </tr>
    <tr>
      <td>Détenteur </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>Opportunité</td>
      <td>opportunitésId</td>
    </tr>
    <tr>
      <td>Client potentiel</td>
      <td>customerId</td>
    </tr>
  </tbody>
</table>

## Champs système associés à Microsoft dans Marketo (lecture seule) {#microsoft-related-system-fields}

Les champs ci-dessous sont créés dans Marketo mais ne peuvent pas être ajustés par les utilisateurs.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Champ Marketo</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>Type Microsoft</td>
      <td>Prospérité ou Contact. S’il est vide, le prospect n’existe que comme une personne dans Marketo</td>
    </tr>
    <tr>
      <td>Date de création - Microsoft</td>
      <td>Date de création dans MS Dynamics (peut différer de celle créée dans Marketo)</td>
    </tr>
    <tr>
      <td>Microsoft est supprimé</td>
      <td>La personne se trouvait auparavant dans Microsoft mais a été supprimée et vit désormais uniquement dans Marketo.</td>
    </tr>
  </tbody>
</table>
