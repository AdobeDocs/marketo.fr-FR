---
description: Mappage  [!DNL Veeva]  Champ Par Défaut - Documents Marketo - Documentation Du Produit
title: Mappage  [!DNL Veeva]  champs par défaut
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 47%

---

# Mappage par défaut des champs de [!DNL Veeva] {#default-veeva-field-mapping}

Lorsque vous synchronisez initialement votre compte Marketo Engage avec [!DNL Veeva], Marketo effectue automatiquement ces associations entre vos champs intégrés [!DNL Veeva] et Marketo. Marketo synchronisera également vos champs personnalisés sur vos comptes et contacts.

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
      <td>Score</td>
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
      <td>Revenus annuels</td>
      <td>Revenus annuels</td>
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
      <td>Code Postal De Facturation</td>
      <td>Code postal de facturation</td>
    </tr>
    <tr>
      <td>Province/état de facturation</td>
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
      <td>Secteur industriel</td>
      <td>Secteur industriel</td>
    </tr>
    <tr>
      <td>Supprimé</td>
      <td>Suppression de SFDC</td>
    </tr>
    <tr>
      <td>Nom de compte</td>
      <td>Nom de la société</td>
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

## Champs système liés au [!DNL Veeva] dans Marketo (lecture seule) {#veeva-related-system-fields-in-marketo}

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
      <td>[!DNL Veeva] ID</td>
      <td>Identifiant de [!DNL Salesforce] de 18 caractères</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] Type</td>
      <td>Contact. Si ce champ est vide, le prospect n’existe que comme personne dans Marketo</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] Date de création</td>
      <td>Date de création dans SFDC (peut être différente de la date de création dans Marketo)</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] est supprimé</td>
      <td>Cette personne se trouvait auparavant dans SFDC, mais a été supprimée. Elle vit désormais uniquement dans Marketo</td>
    </tr>
  </tbody>
</table>
