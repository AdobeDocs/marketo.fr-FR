---
unique-page-id: 6848747
description: Descriptions des autorisations de rôle - Documents Marketo - Documentation du produit
title: Descriptions des autorisations de rôle
exl-id: 00963cd9-2d53-455f-bc6f-42a573468ff9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 19%

---

# Descriptions des autorisations de rôle {#descriptions-of-role-permissions}

Vous trouverez ci-dessous une liste de toutes les autorisations disponibles que vous pouvez affecter à vos rôles. Les autorisations sont généralement associées à des zones fonctionnelles spécifiques à l’intérieur de Marketo et peuvent vous aider à contrôler les zones et fonctionnalités auxquelles les utilisateurs ont accès.

Informations supplémentaires sur les autorisations :

* L’autorisation &quot;Accès&quot; accorde une autorisation de rôle à la vue et modifie parfois cette partie de l’application.
* Pour qu’un rôle ait accès aux sous-autorisations (&quot;Créer&quot;, &quot;Supprimer&quot;, etc.), il doit disposer de l’autorisation &quot;Accès&quot; à cette partie de l’application. Par exemple, si vous souhaitez autoriser une personne à modifier des campagnes, elle doit disposer de l’autorisation générale d’accès aux Activités marketing.
* Vous pouvez peut-être voir des actions ou des ressources que vous n’êtes pas autorisé à utiliser. Cependant, si vous essayez d&#39;y accéder, un message vous avertit de votre accès limité.

## Autorisations disponibles {#available-permissions}

Lorsque vous [créez ou modifiez un rôle](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), vous pouvez sélectionner les autorisations suivantes pour autoriser ce rôle en cochant les cases appropriées.

![](assets/createnewrole.png)

## Accès admin  {#access-admin}

Vue et modification des paramètres dans la section Mon compte de l’administrateur.

* Piste d&#39;audit d&#39;accès - Donne aux utilisateurs l&#39;accès à la piste d&#39;audit des ressources et à la piste d&#39;audit d&#39;administration
* Canaux d&#39;accès : donne aux utilisateurs l&#39;accès uniquement à la modification de la balise de Canal, et non à d&#39;autres balises personnalisées.
* Limite de communication d’accès : donne aux utilisateurs l’accès pour activer une limite de communication dans Admin
* Access CRM - Donne aux utilisateurs l&#39;accès à la gestion de la relation client, telle que Salesforce ou Microsoft Dynamics, dans Admin
* Accès [Data.com](https://Data.com) : donne aux utilisateurs l’accès à l’action de flux Data.com
* Accès à l’administrateur des courriels : permet aux utilisateurs d’accéder à l’administrateur des courriels afin de modifier les paramètres par défaut, tels que l’annulation de l’abonnement et l’identité graphique des domaines.
* Partenaires de Événement d&#39;accès - Donne aux utilisateurs l&#39;accès à LaunchPoint dans l&#39;administration
* Gestion des champs d’accès - Donne aux utilisateurs l’accès à la gestion des champs dans l’administration
* Téléchargement des fichiers d’accès : permet aux utilisateurs de télécharger des images et des fichiers vers Design Studio.
* Landings page d’accès - Donne aux utilisateurs l’accès aux Landings page dans l’administration
* Emplacement d’accès : donne aux utilisateurs l’accès à l’emplacement dans l’administration pour définir la langue, le paramètre régional, le fuseau horaire et la devise par défaut.
* Historique de connexion à l&#39;accès - Donne aux utilisateurs l&#39;accès à l&#39;historique de connexion à l&#39;utilisateur dans la piste d&#39;audit
* Paramètres de connexion d’accès : donne aux utilisateurs l’accès aux paramètres de connexion dans les paramètres d’administration de la sécurité, des restrictions d’adresse IP et des rapports de Liste dynamique.
* Accès à l’Activité personnalisée Marketo - Donne aux utilisateurs l’accès aux Activités personnalisées Marketo dans Admin
* Accès à l&#39;objet personnalisé Marketo - Donne aux utilisateurs l&#39;accès aux objets personnalisés Marketo dans Admin
* Accès à Munchkin - GIves les utilisateurs ont accès à Munchkin dans Admin, pour la définition du code de suivi, le suivi des personnes et l&#39;activation de la configuration de l&#39;API.
* Accès à l’analyse du cycle des recettes - Donne aux utilisateurs l’accès à l’analyse du cycle des recettes dans l’administration, pour la définition du résumé de synchronisation et de l’attribution.
* Rôles d’accès : donne aux utilisateurs l’accès à la gestion et à la modification des rôles, mais pas aux utilisateurs.
* Accès à Sales Insight - Donne aux utilisateurs l&#39;accès à la gestion de Sales Insight dans l&#39;administration, pour la définition de l&#39;état, de la configuration de l&#39;API, du score de personne et d&#39;autres paramètres.
* Accès à la connexion unique : donne aux utilisateurs l’accès à la gestion de la connexion unique dans l’administration, pour l’activation du langage SAML et l’utilisation des paramètres SAML et des URL de page de redirection.
* Accès à Smart Campaign - Donne aux utilisateurs l’accès à Smart Campaign dans l’administration, ce qui limite les limites imposées aux personnes qualifiées.
* Accès à l&#39;API SOAP - Donne aux utilisateurs l&#39;accès à la gestion des API SOAP dans les services Web dans Admin
* Balises d’accès : donne aux utilisateurs l’accès à toutes les balises personnalisées, à l’exception de la balise de Canal.
* Accès au coffre au trésor - Donne aux utilisateurs l&#39;accès aux fonctionnalités expérimentales du coffre au trésor dans l&#39;administration
* Utilisateurs d’accès : donne aux utilisateurs l’accès à la modification et à la gestion des utilisateurs (mais pas aux rôles) dans l’administration
* Accéder à des hameçons Web - Fournit aux utilisateurs des hameçons Web dans l’administration, pour définir des détails et des correspondances de réponses
* Accéder aux espaces de travail et aux partitions : donne aux utilisateurs l’accès à la création, à la modification et à la suppression des espaces de travail et des partitions dans l’administration.

## Accéder à l’API  {#access-api}

Donne aux utilisateurs disposant de l&#39;accès **API uniquement** **Rôle** aux API individuelles répertoriées ci-dessous.

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

Donne aux utilisateurs l’accès aux onglets Analytics, aux statistiques d’e-mail, aux rapports et aux trois éléments ci-dessous, sauf s’ils sont désactivés.

* Accès à l&#39;Explorateur des recettes - La désactivation supprime l&#39;accès de l&#39;utilisateur à l&#39;Explorateur des recettes.
* Supprimer le rapport - La désactivation supprime la possibilité pour l&#39;utilisateur de supprimer des rapports.
* Exportation des données Analytics - La désactivation supprime la possibilité pour l’utilisateur d’exporter des données Analytics.

## Accéder aux présentations du calendrier {#access-calendar-presentations}

Donne aux utilisateurs l&#39;accès aux présentations Calendrier - permet l&#39;affichage du bouton Presentations en bas.

* Modifier le calendrier Presentations : permet aux utilisateurs de modifier des présentations dans le calendrier

## Accès au studio de conception {#access-design-studio}

Donne aux utilisateurs l’accès à l’onglet Design Studio et à la vue de l’arborescence, mais pas aux détails.

* Accès e-mail
   * Modifier le courrier électronique : permet aux utilisateurs de modifier, créer et cloner des courriers électroniques.
      * Optimiser le courrier électronique : permet aux utilisateurs de rendre un courrier électronique opérationnel. Voir : [Optimiser un courriel](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * Approuver le courrier électronique : permet aux utilisateurs d&#39;approuver les courriers électroniques.
      * Supprimer un courrier électronique : permet aux utilisateurs de supprimer des courriers électroniques.
      * Définir un domaine de marque : permet aux utilisateurs de travailler avec des domaines de marque. Voir : [Ajouter un domaine de marque supplémentaire](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

* Accès modèle d&#39;e-mail

   * Approuver modèle d&#39;e-mail
   * Supprimer modèle d’e-mail
   * Modifier un modèle de courrier électronique - Modifier, créer et cloner des modèles de courrier électronique

* Accès formulaire

   * Supprimer formulaire
   * Modifier le formulaire - Modifier, créer et cloner des formulaires

* Accès image

   * Supprimer image
   * Télécharger l&#39;image

* Accès page de destination

   * Approuver page de destination
   * Supprimer page de destination
   * Modifier le Landing page - Modifier, créer et cloner des landings page

* Accès modèle de page de destination

   * Approuver modèle page de destination
   * Supprimer modèle de page de destination
   * Modifier un modèle de Landing page - Modifier, créer et cloner des modèles de landing page

* Accès extrait

   * Approuver l’extrait
   * Supprimer extrait
   * Modifier extrait

* Accéder à l&#39;application sociale

   * Approuver l&#39;application sociale
   * Supprimer l&#39;application sociale
   * Modifier l&#39;application sociale

## Accès à la base de données {#access-database}

Vue de la base de données ainsi que de la vue et modification des listes dynamiques/statiques.

* Accès segmentation

   * Approuver segmentation
   * Supprimer segmentation
   * Modifier segmentation

* Import liste avancé
* Supprimer l’individu
* Supprimer liste
* Modifier une personne - Empêche la modification manuelle et l&#39;exécution d&#39;étapes de flux simples ; vous pouvez toujours modifier des personnes en exécutant des campagnes contre elles.
* Exporter une personne - Exporter des feuilles de calcul à partir de vos listes de base de données
* Importer l’objet personnalisé
* Importer la liste
* Fusionner les personnes
* Exécuter des actions de flux unique : permet aux utilisateurs d&#39;exécuter l&#39;étape de flux **Modifier la valeur des données** sur les personnes de la base de données.

* Données d&#39;opportunité de vue - Masque les informations d&#39;opportunité sur la page de détails de la personne

## Accès activité marketing {#access-marketing-activities}

Vue de l’onglet Activités marketing, des campagnes et des dossiers de campagne.

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

* Accès administrateur pour un espace de travail spécifique (uniquement si les espaces de travail sont activés)
* Déplacement de fichiers entre les espaces de travail (uniquement si les espaces de travail sont activés)
