---
description: Hériter de Doc 1 - Documents Marketo - Documentation du produit
title: Hériter Doc 1
hide: true
hidefromtoc: true
source-git-commit: 3c7eb2fc2e64898e12f08743225c0b802bf97474
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 21%

---

# Hériter Doc 1 {#inherit-doc-1}

L’audit d’une instance héritée peut ressembler à un

Avez-vous hérité d’une instance de Marketo Engage existante d’un autre administrateur ? Si c&#39;est le cas, cet article est pour vous.

>[!TIP]
>
>Si vous êtes un nouvel utilisateur Marketo Engage et que vous ne connaissez pas beaucoup des termes, consultez la section [Glossaire Marketo](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Utilisateurs et rôles {#users-and-roles}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Zone</th> 
   <th>Objectif de la révision</th>
   <th>Colonne 3</th>
  </tr> 
  <tr> 
   <td>Utilisateurs</td> 
   <td><li>Combien d’utilisateurs y a-t-il ?</li>
<li>Certains utilisateurs doivent-ils avoir expiré ?</li>
<li>Votre entreprise a-t-elle des politiques concernant la suppression d’utilisateurs ?</li> 
<li>Combien d’utilisateurs disposent d’autorisations d’administrateur ?</li>
<li>L’un de ces utilisateurs doit-il être remplacé par d’autres rôles ?</li> 
<li>Qui sont les utilisateurs de l’API dans cette instance ?</li></td>
   <td>3.1</td>
  </tr>
  <tr> 
   <td>Rôles</td> 
   <td><li>Combien y a-t-il de rôles ?</li>  
<li>Quels droits/accès possède chaque rôle ? Y a-t-il des ajustements ?</li>
<li>Combien d’utilisateurs y a-t-il par rôle ?</li>
<li>À quelle fréquence les utilisateurs se connectent-ils ?</li>
<li>Chaque utilisateur de l’API possède-t-il son propre rôle d’utilisateur ? Si ce n’est pas le cas, envisagez de mettre en oeuvre cette méthode pour faciliter le dépannage.</li> 
<li>Vos rôles utilisateur et autorisations sont-ils conformes aux politiques de confidentialité des données de votre entreprise ?</li></td>
   <td>3.2</td>
  </tr>
  <tr> 
   <td>Documentation interne</td> 
   <td><li>Les utilisateurs et les rôles sont-ils clairement définis dans votre organisation ?</li>
<li>Quel est votre processus pour ajouter un nouvel utilisateur/administrateur ?</li></td>
   <td>3.3</td>
  </tr>
  <tr> 
   <td>Environnement de test (le cas échéant)</td> 
   <td><li>Disposez-vous d’une instance sandbox ? Si tel est le cas, passez en revue les catégories ci-dessus pour votre environnement de test.</li>
<li>L’importation de programme est-elle liée à votre environnement de test ?</li></td>
   <td>3,4</td>
  </tr>
 </tbody> 
</table>

## Journal d&#39;audit {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Zone</th> 
   <th>Objectif de la révision</th>
   <th>Colonne 3</th>
  </tr> 
  <tr> 
   <td>Journal d'audit</td> 
   <td><li>Qui travaille dans l’instance ?</li></td>
   <td>3.1</td>
  </tr>
 </tbody> 
</table>

## Espaces de travail et partitions {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Zone</th> 
   <th>Objectif de la révision</th>
   <th>Colonne 3</th>
  </tr> 
  <tr> 
   <td>Espaces de travail et partitions</td> 
   <td><li>Combien d'espaces de travail et/ou de partitions avez-vous ?</li>
<li>Quel est le but Principal de chaque espace de travail et de chaque partition ?</li>
<li>Ont-ils besoin d'être contrôlés ou modifiés ?</li>
<li>Quelle est la relation entre vos espaces de travail et vos partitions ?</li>
<li>Combien d’utilisateurs ont accès à chaque espace de travail ?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Documentation interne</td> 
   <td><li>Comment les espaces de travail et les partitions sont-ils définis ?</li>
<li>Quel est votre processus pour ajouter des espaces de travail à votre instance ou ajouter des utilisateurs à un espace de travail ?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Campagnes intelligentes {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Zone</th> 
   <th>Objectif de la révision</th>
   <th>Colonne 3</th>
  </tr> 
  <tr> 
   <td>Paramètres de la campagne intelligente</td> 
   <td><li>Y a-t-il des limites en place ? Votre entreprise a-t-elle des politiques pour lesquelles des limites de communication peuvent être nécessaires ?</li>
<li>Adobe recommande de limiter votre communication à 1 par jour et 3 par 7 jours avec les emails non opérationnels bloqués.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Limites de communication {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Zone</th> 
   <th>Objectif de la révision</th>
   <th>Colonne 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Balises {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Zone</th> 
   <th>Objectif de la révision</th>
   <th>Colonne 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Gestion de la base de données {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Zone</th> 
   <th>Objectif de la révision</th>
   <th>Colonne 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Intégrations {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Zone</th> 
   <th>Objectif de la révision</th>
   <th>Colonne 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Coffre au trésor {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Zone</th> 
   <th>Objectif de la révision</th>
   <th>Colonne 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Divers {#miscellaneous}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Zone</th> 
   <th>Objectif de la révision</th>
   <th>Colonne 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
