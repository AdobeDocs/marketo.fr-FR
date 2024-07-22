---
description: Mappage des champs Veeva par défaut - Documents Marketo - Documentation du produit
title: Mappage des champs Veeva par défaut
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 44%

---

# Mappage des champs Veeva par défaut {#default-veeva-field-mapping}

Lors de la synchronisation initiale de votre compte de Marketo Engage avec Veeva, Marketo effectue automatiquement ces associations entre vos champs intégrés Veeva et Marketo. Marketo synchronise également vos champs personnalisés dans vos comptes et contacts.

## Champs de contact {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Champ SFDC</th>
      <th>Champ Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Date de naissance</td>
      <td>Date de naissance</td>
    </tr>
    <tr>
      <td>Date de création</td>
      <td>Date de création SFDC</td>
    </tr>
    <tr>
      <td>Description du contact</td>
      <td>Notes du contact</td>
    </tr>
    <tr>
      <td>E-mail</td>
      <td>Adresse e-mail</td>
    </tr>
    <tr>
      <td>Télécopie professionnelle</td>
      <td>Numéro de fax</td>
    </tr>
    <tr>
      <td>Prénom</td>
      <td>Prénom</td>
    </tr>
    <tr>
      <td>Désabonnement par e-mail</td>
      <td>Désabonné</td>
    </tr>
    <tr>
      <td>Supprimé</td>
      <td>Suppression de SFDC</td>
    </tr>
    <tr>
      <td>Nom</td>
      <td>Nom</td>
    </tr>
    <tr>
      <td>Source du lead</td>
      <td>Source</td>
    </tr>
    <tr>
      <td>Évaluation des leads</td>
      <td>Évaluation</td>
    </tr>
    <tr>
      <td>MailingCity</td>
      <td>Ville</td>
    </tr>
    <tr>
      <td>MailingCountry</td>
      <td>Pays</td>
    </tr>
    <tr>
      <td>MailingPostalCode</td>
      <td>Code postal</td>
    </tr>
    <tr>
      <td>MailingState</td>
      <td>État</td>
    </tr>
    <tr>
      <td>MailingStreet</td>
      <td>Adresse</td>
    </tr>
    <tr>
      <td>Téléphone portable</td>
      <td>Numéro de téléphone mobile</td>
    </tr>
    <tr>
      <td>Téléphone de l'entreprise
</td>
      <td>Numéro de téléphone</td>
    </tr>
    <tr>
      <td>Titre</td>
      <td>Titre</td>
    </tr>
    <tr>
      <td>Titre</td>
      <td>Intitulé du poste</td>
    </tr>
  </tbody>
</table>

## Champs de compte {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Champ SFDC</th>
      <th>Champ Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Chiffre d'affaires annuel</td>
      <td>Chiffre d'affaires annuel</td>
    </tr>
    <tr>
      <td>Ville de facturation</td>
      <td>Ville de facturation</td>
    </tr>
    <tr>
      <td>Pays de facturation</td>
      <td>Pays de facturation</td>
    </tr>
    <tr>
      <td>Code postal de facturation</td>
      <td>Code postal de facturation</td>
    </tr>
    <tr>
      <td>État/province de facturation</td>
      <td>État de facturation</td>
    </tr>
    <tr>
      <td>Rue de facturation</td>
      <td>Adresse de facturation</td>
    </tr>
    <tr>
      <td>Description du compte</td>
      <td>Notes sur la société</td>
    </tr>
    <tr>
      <td>Industrie</td>
      <td>Industrie</td>
    </tr>
    <tr>
      <td>Supprimé</td>
      <td>Suppression de SFDC</td>
    </tr>
    <tr>
      <td>Nom de compte</td>
      <td>Nom de l’entreprise</td>
    </tr>
    <tr>
      <td>Employés</td>
      <td>Nombre d'employés</td>
    </tr>
    <tr>
      <td>Téléphone du compte</td>
      <td>Téléphone principal</td>
    </tr>
    <tr>
      <td>Code SIC</td>
      <td>Code SIC</td>
    </tr>
    <tr>
      <td>Site du compte</td>
      <td>Site</td>
    </tr>
    <tr>
      <td>Type de compte</td>
      <td>Type de SFDC</td>
    </tr>
    <tr>
      <td>Site web</td>
      <td>Site web</td>
    </tr>
  </tbody>
</table>

## Champs de système associés à Veeva dans Marketo (lecture seule) {#veeva-related-system-fields-in-marketo}

Ces champs sont créés dans Marketo mais ne peuvent pas être ajustés par les clients.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Champ</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Veeva Id</td>
      <td>L’identifiant Salesforce à 18 caractères</td>
    </tr>
    <tr>
      <td>Type de Veeva</td>
      <td>Contact. S’il est vide, le prospect n’existe que comme une personne dans Marketo</td>
    </tr>
    <tr>
      <td>Date de création de Veeva</td>
      <td>Date de création dans SFDC (peut différer de celle de création dans Marketo)</td>
    </tr>
    <tr>
      <td>Veeva est supprimée</td>
      <td>La personne se trouvait auparavant dans la SFDC mais a été supprimée et vit désormais uniquement dans Marketo.</td>
    </tr>
  </tbody>
</table>
