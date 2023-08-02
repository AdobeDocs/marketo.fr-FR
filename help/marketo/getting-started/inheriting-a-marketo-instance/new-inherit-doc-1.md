---
description: Hériter de Doc 1 - Documents Marketo - Documentation du produit
title: Hériter Doc 1
hide: true
hidefromtoc: true
source-git-commit: b6628cee17799801815f5b84c424399538eaf5ee
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 10%

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
   <td><li>Existe-t-il une restriction sur la taille d’une campagne dynamique ?</li>
<li>Si ce n’est pas le cas, envisagez d’en ajouter une. Nous vous recommandons de limiter les limites des campagnes intelligentes à 25 % de votre base de données afin d’éviter toute surcharge de communication ou de traitement de l’ensemble de votre base de données dans les workflows. Cela protège non seulement votre marque, mais également les performances de votre instance.</li></td>
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
   <td>Limites de communication</td> 
   <td><li>Y a-t-il des limites en place ? Votre entreprise a-t-elle des politiques pour lesquelles des limites de communication peuvent être nécessaires ?</li>
<li>Adobe recommande de limiter votre communication à 1 par jour et 3 par 7 jours, avec les emails non opérationnels bloqués.</li></td>
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
   <td>Balises</td> 
   <td><li>Combien de balises y a-t-il ? Combien de balises sont utilisées ? Dois-je ajouter des éléments ?</li>
<li>Les balises sont-elles requises dans vos programmes ?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Canaux</td> 
   <td><li>Combien de canaux y a-t-il ? Combien sont utilisés ?</li>
<li>Tous les statuts des programmes des canaux sont-ils appropriés ? Est-ce qu'ils affichent la progression dans le programme ?</li>
<li>Vos canaux sont-ils liés à des types de programmes spécifiques ?</li>
<li>Quels états sont considérés comme une réussite pour chaque canal ? Ces objectifs correspondent-ils à vos objectifs marketing ?</li>
<li>Le canal opérationnel est-il utilisé de manière appropriée ?</li>
<li>Pour le Report Builder avancé (Revenue Cycle Explorer\RCE), le comportement d’analyse de canal est-il défini pour s’aligner sur les pratiques de votre programme incorporant le coût de la période ?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Calendrier marketing (le cas échéant)</td> 
   <td><li>Combien y a-t-il de types d’entrée de calendrier ? Sont-ils toujours pertinents ?</li></td>
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
   <td>Gestion des champs</td> 
   <td><li>Combien de champs y a-t-il ? Cliquez sur "Exporter les noms des champs" pour consulter la liste de vos champs, champs personnalisés et noms d’API.</li>
<li>Combien de champs personnalisés y a-t-il ?</li>
<li>Combien de champs sont utilisés ? Sélectionnez "Exporter utilisé par" dans la liste déroulante Actions du champ pour passer en revue les ressources associées à un champ.</li>
<li>Combien sont synchronisés entre Marketo Engage et votre CRM ?</li>
<li>Les champs CRM sont-ils synchronisés avec les objets appropriés ?</li>
<li>Existe-t-il un affichage personnalisé des détails de personne ? Devrait-il y en avoir ?</li>
<li>Disposez-vous d’une convention d’affectation des noms pour vos champs en fonction de la source ? Si ce n’est pas le cas, envisagez d’implémenter cette méthode.</li>
<li>Les champs sont-ils bloqués ? Assurez-vous de comprendre pourquoi elles le sont.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Activités personnalisées</td> 
   <td><li>Existe-t-il des activités personnalisées ?</li>
<li>Si tel est le cas, cliquez dessus pour comprendre les activités qui ne sont pas liées à un formulaire Marketo, un email ou une landing page.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td> objets  personnalisés</td> 
   <td><li>Combien d’objets personnalisés y a-t-il ? Comment sont-ils synchronisés avec votre CRM ?</li>
<li>Comment ces objets personnalisés sont-ils utilisés par vos programmes et requêtes de liste ?</li></td>
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
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight (le cas échéant)</td> 
   <td><li>Le package MSI a-t-il été installé ?</li>
<li>Avez-vous effectué la mise à niveau vers la dernière version de Sales Insight ?</li>
<li>Avez-vous terminé la configuration de Sales Insight ?</li>
<li>Avez-vous donné accès à vos utilisateurs en fonction du nombre de sièges que vous avez achetés ?</li></td>
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
