---
unique-page-id: 6848747
description: Descriptions des autorisations de rôle - Documents Marketo - Documentation du produit
title: Descriptions des autorisations de rôle
exl-id: 00963cd9-2d53-455f-bc6f-42a573468ff9
source-git-commit: 27eb6dedaae60616fe871d0a3ac4f38b5b4ecfd4
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 19%

---

# Descriptions des autorisations de rôle {#descriptions-of-role-permissions}

Vous trouverez ci-dessous une liste de toutes les autorisations disponibles que vous pouvez affecter à vos rôles. Les autorisations sont généralement associées à des zones fonctionnelles spécifiques dans Marketo et peuvent vous aider à contrôler les zones et fonctionnalités auxquelles différents utilisateurs ont accès.

Informations supplémentaires sur les autorisations :

* L’autorisation &quot;Accès&quot; permet à un rôle d’afficher et parfois de modifier cette partie de l’application.
* Pour qu’un rôle ait accès aux sous-autorisations (&quot;Créer&quot;, &quot;Supprimer&quot;, etc.), il doit disposer de l’autorisation &quot;Accès&quot; à cette partie de l’application. Par exemple, si vous souhaitez autoriser une personne à modifier les campagnes, elle doit disposer d’une autorisation globale d’accès aux activités marketing.
* Vous pouvez peut-être voir des actions ou des ressources que vous n’êtes pas autorisé à utiliser. Cependant, si vous tentez d’y accéder, un message vous avertit de votre accès limité.

## Autorisations disponibles {#available-permissions}

Lorsque vous [création ou modification d’un rôle](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), vous pouvez sélectionner l’une des autorisations suivantes pour autoriser ce rôle en cochant les cases appropriées.

![](assets/descriptions-of-role-permissions-1.png)

## Accès admin  {#access-admin}

Affichez et apportez des modifications aux paramètres dans la section Mon compte de l’administrateur.

* Accéder au journal d’audit : permet aux utilisateurs d’accéder au journal d’audit des ressources et au journal d’audit de l’administrateur.
* Accès aux canaux : permet aux utilisateurs d’accéder uniquement à la balise Channel et non à d’autres balises personnalisées.
* Limite de communication d’accès : permet aux utilisateurs d’activer une limite de communication dans Admin
* Accès à la gestion de la relation client : permet aux utilisateurs d’accéder à la gestion de la relation client, comme Salesforce ou Microsoft Dynamics, dans Admin.
* Accès [Data.com](https://Data.com) - Donne aux utilisateurs l’accès à l’action de flux Data.com
* Accès à l’administrateur des courriers électroniques : permet aux utilisateurs de modifier les paramètres par défaut, tels que le désabonnement et les domaines de marque.
* Accès aux partenaires d’événement : permet aux utilisateurs d’accéder à LaunchPoint dans Admin.
* Gestion des champs d’accès : permet aux utilisateurs d’accéder à la gestion des champs dans Admin.
* Accéder au téléchargement de fichier : permet aux utilisateurs de charger des images et des fichiers dans Design Studio.
* Accès aux pages d’entrée : permet aux utilisateurs d’accéder aux pages d’entrée dans Admin.
* Emplacement d’accès : permet aux utilisateurs d’accéder à l’emplacement dans l’administration pour définir la langue, le paramètre régional, le fuseau horaire et la devise par défaut.
* Historique de connexion des accès : permet aux utilisateurs d’accéder à l’historique de connexion des utilisateurs dans le journal d’audit
* Paramètres de connexion d’accès : permet aux utilisateurs d’accéder aux paramètres de connexion dans les paramètres Administration pour la sécurité, les restrictions d’IP et les rapports de liste dynamique.
* Accès à l’activité personnalisée Marketo - Donne aux utilisateurs l’accès aux activités personnalisées Marketo dans Admin
* Accès à l’objet personnalisé de Marketo - Donne aux utilisateurs l’accès aux objets personnalisés de Marketo dans Admin
* Accès à Munchkin : les utilisateurs de GI ont accès à Munchkin dans Admin pour définir le code de suivi, le suivi des personnes et activer la configuration de l’API.
* Accès à Revenue Cycle Analytics : permet aux utilisateurs d’accéder à Revenue Cycle Analytics dans l’administration pour définir le résumé de synchronisation et l’attribution.
* Rôles d’accès : donne aux utilisateurs l’accès à la gestion et à la modification des rôles, mais pas aux utilisateurs.
* Accès à Sales Insight : permet aux utilisateurs de gérer Sales Insight dans Admin pour définir l’état, la configuration de l’API, la notation des personnes et d’autres paramètres.
* Connexion unique : permet aux utilisateurs de gérer l’authentification unique dans Admin pour activer SAML et utiliser les paramètres SAML et les URL de page de redirection.
* Accéder à la campagne dynamique : permet aux utilisateurs d’accéder à la campagne dynamique dans l’administration pour limiter les limitations sur les personnes qualifiées.
* Accès à l’API SOAP : permet aux utilisateurs d’accéder à la gestion des API SOAP dans les services web dans Admin.
* Accéder aux balises : permet aux utilisateurs d’accéder à toutes les balises personnalisées, à l’exception de la balise Canal.
* Accéder à la poitrine au trésor : donne aux utilisateurs l’accès aux fonctionnalités expérimentales de la poitrine au trésor dans l’administration
* Accès aux utilisateurs : donne aux utilisateurs l’accès à la modification et à la gestion des utilisateurs (mais pas aux rôles) dans l’administration.
* Accès aux webhooks : permet aux utilisateurs de se connecter aux webhooks dans Admin pour définir les détails et les mappages de réponse.
* Accéder aux espaces de travail et aux partitions : permet aux utilisateurs de créer, modifier et supprimer des espaces de travail et des partitions dans Admin.

## Accéder à l’API  {#access-api}

Donne aux utilisateurs l’accès au **API uniquement** **Rôle** accès aux différentes API répertoriées ci-dessous.

* Approuver les ressources
* Lancer la campagne
* Activité en lecture seule
* Métadonnées d’activité en lecture seule
* Ressources en lecture seule
* Campagne en lecture seule
* Société en lecture seule
* Objet personnalisé en lecture seule
* Individu en lecture seule
* Compte nommé en lecture seule
* Opportunité en lecture seule
* Commercial en lecture seule
* Activité en lecture/écriture
* Métadonnées d’activité en lecture/écriture
* Ressources accessibles en lecture/écriture
* Campagne accessible en lecture/écriture
* Société accessible en lecture/écriture
* Objet personnalisé accessible en lecture/écriture
* Individu accessible en lecture / écriture
* Compte nommé en lecture / écriture
* Opportunité accessible en lecture/écriture
* Commercial accessible en lecture/écriture

## Accès Analytics {#access-analytics}

Donne aux utilisateurs l’accès aux onglets Analytics, aux statistiques sur les e-mails, aux rapports et aux trois éléments ci-dessous, sauf s’ils ne sont pas cochés.

* Accéder à l’Explorateur des recettes : la désactivation supprime l’accès de l’utilisateur à l’Explorateur des recettes.
* Supprimer le rapport : la désélection supprime la possibilité pour l’utilisateur de supprimer des rapports.
* Exportation des données Analytics : la désélection supprime la possibilité pour l’utilisateur d’exporter des données Analytics.

## Accéder aux présentations du calendrier {#access-calendar-presentations}

Donne aux utilisateurs l’accès aux présentations du calendrier : permet d’afficher le bouton Presentations en bas de la page.

* Modifier le calendrier Presentations : permet aux utilisateurs de modifier des présentations dans le calendrier

## Accès au studio de conception {#access-design-studio}

Permet aux utilisateurs d’accéder à l’onglet Design Studio et à la vue de l’arborescence, mais pas aux détails.

* Accès e-mail
   * Modifier le courrier électronique : permet aux utilisateurs de modifier, créer et cloner des courriers électroniques.
      * Rendre le message électronique opérationnel : permet aux utilisateurs de rendre un message électronique opérationnel. Voir : [Rendre un message électronique opérationnel](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * Valider le courrier électronique : permet aux utilisateurs d’approuver les courriers électroniques.
      * Supprimer le courrier électronique : permet aux utilisateurs de supprimer des courriers électroniques.
      * Définir un domaine de marque : permet aux utilisateurs de travailler avec des domaines de marque. Voir : [Ajout d’un domaine de marque supplémentaire](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

* Accès modèle d&#39;e-mail

   * Approuver modèle d&#39;e-mail
   * Supprimer modèle d&#39;e-mail
   * Modifier le modèle de courrier électronique : modifiez, créez et clonez des modèles de courrier électronique.

* Accès formulaire

   * Approuver le formulaire
   * Supprimer formulaire
   * Modifier le formulaire : modifiez, créez et clonez des formulaires.

* Accès image

   * Supprimer image
   * Télécharger l&#39;image

* Accès page de destination

   * Approuver page de destination
   * Supprimer page de destination
   * Modifier la page d’entrée : modifiez, créez et clonez des pages d’entrée.

* Accès modèle de page de destination

   * Approuver modèle page de destination
   * Supprimer modèle page de destination
   * Modifier le modèle de page d’entrée : modifiez, créez et clonez des modèles de page d’entrée.

* Accès extrait

   * Approuver extrait
   * Supprimer extrait
   * Modifier extrait

* Accéder à l&#39;application sociale

   * Approuver l&#39;application sociale
   * Supprimer l&#39;application sociale
   * Modifier l&#39;application sociale

## Accès à la base de données {#access-database}

Visualisez la base de données et affichez et modifiez des listes dynamiques/statiques.

* Accès segmentation

   * Approuver segmentation
   * Supprimer segmentation
   * Modifier segmentation

* Supprimer individu
* Supprimer liste
* Modifier la personne : empêche la modification et l’exécution manuelles d’étapes à flux unique ; vous pouvez toujours modifier des personnes en exécutant des campagnes contre elles.
* Exporter une personne : exportez des feuilles de calcul à partir de vos listes de base de données.
* Importer l’objet personnalisé
* Importer la Liste
* Fusionner les personnes
* Exécuter des actions de flux unique : permet aux utilisateurs de s’exécuter. **Modifier la valeur des données** étape de flux sur les personnes de la base de données

* Afficher les données d’opportunité : masque les informations d’opportunité sur la page des détails de la personne.

## Accès activité marketing {#access-marketing-activities}

Affichez l’onglet Activités marketing, les campagnes et les dossiers de campagnes.

* Accéder à un message SMS

   * Approuver un message SMS
   * Supprimer un message SMS
   * Modifier un message SMS

* Accéder à la notification Push

   * Approuver la notification Push
   * Supprimer une notification Push
   * Modifier la notification Push

* Accéder aux récompenses
* Activer la campagne à déclencheurs
* Approuver le programme de messagerie électronique
* Reproduire une ressource marketing
* Supprimer ressource marketing
* Modifier les restrictions de la campagne
* Modifier ressource marketing
* Importer le programme
* Importer une liste
* Programmer une campagne par lot

Accéder à la SEO

* Gérer une SEO
* SEO standard

## Ciblage et personnalisation {#targeting-and-personalization}

* Gérer une personnalisation Web
* Éditeur de campagnes CRE
* Outil de lancement de campagnes CRE
* Éditeur de campagnes Web
* Outil de lancement de campagnes Web

Gestion de l&#39;espace de travail

* Accès administrateur pour un espace de travail spécifique (uniquement si les espaces de travail sont activés).
* Déplacer des ressources entre les espaces de travail (uniquement si les espaces de travail sont activés)
