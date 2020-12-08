---
unique-page-id: 6848747
description: Descriptions des autorisations de rôle - Documents marketing - Documentation du produit
title: Descriptions des autorisations de rôle
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---


# Descriptions des autorisations de rôle {#descriptions-of-role-permissions}

>[!NOTE]
>
>**FYI**
>
>Marketo est maintenant en train de normaliser la langue dans tous les abonnements. Vous pouvez donc voir des pistes dans votre abonnement et des personnes/personnes dans docs.marketo.com. Ces termes signifient la même chose ; cela n&#39;a aucune incidence sur les instructions relatives aux articles. Il y a aussi d&#39;autres changements. [En savoir plus](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Vous trouverez ci-dessous une liste de toutes les autorisations disponibles que vous pouvez affecter à vos rôles. Les autorisations sont généralement associées à des zones fonctionnelles spécifiques à l’intérieur de Marketing Cloud et peuvent vous aider à contrôler les zones et fonctionnalités auxquelles les utilisateurs ont accès.

Informations supplémentaires sur les autorisations :

* L’autorisation &quot;Accès&quot; accorde une autorisation de rôle à la vue et modifie parfois cette partie de l’application.
* Pour qu’un rôle ait accès aux sous-autorisations (&quot;Créer&quot;, &quot;Supprimer&quot;, etc.), il doit disposer de l’autorisation &quot;Accès&quot; à cette partie de l’application. Par exemple, si vous souhaitez autoriser une personne à modifier des campagnes, elle doit disposer de l’autorisation générale d’accès aux Activités marketing.
* Vous pouvez peut-être voir des actions ou des ressources que vous n’êtes pas autorisé à utiliser. Cependant, si vous essayez d&#39;y accéder, un message vous avertit de votre accès limité.

## Autorisations disponibles {#available-permissions}

Lorsque vous [créez ou modifiez un rôle](../../../../product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), vous pouvez sélectionner les autorisations suivantes pour autoriser ce rôle en cochant les cases appropriées.

![](assets/createnewrole.png)

## Administration d’accès  {#access-admin}

Vue et modification des paramètres dans la section Mon compte de l’administrateur.

* Piste d&#39;audit d&#39;accès - Donne aux utilisateurs l&#39;accès à la piste d&#39;audit des ressources et à la piste d&#39;audit d&#39;administration
* Canaux d&#39;accès : donne aux utilisateurs l&#39;accès uniquement à la modification de la balise de Canal, et non à d&#39;autres balises personnalisées.
* Limite de communication d’accès : donne aux utilisateurs l’accès pour activer une limite de communication dans Admin
* Access CRM - Donne aux utilisateurs l&#39;accès à la gestion de la relation client, telle que Salesforce ou Microsoft Dynamics, dans Admin
* Accès à [Data.com](http://Data.com) : donne aux utilisateurs l’accès à l’action de flux Data.com.
* Accès à l’administrateur des courriels : permet aux utilisateurs d’accéder à l’administrateur des courriels afin de modifier les paramètres par défaut, tels que l’annulation de l’abonnement et l’identité graphique des domaines.
* Partenaires de Événement d&#39;accès - Donne aux utilisateurs l&#39;accès à LaunchPoint dans l&#39;administration
* Gestion des champs d’accès - Donne aux utilisateurs l’accès à la gestion des champs dans l’administration
* Téléchargement des fichiers d’accès : permet aux utilisateurs de télécharger des images et des fichiers vers Design Studio.
* Landings page d’accès - Donne aux utilisateurs l’accès aux Landings page dans l’administration
* Emplacement d’accès : donne aux utilisateurs l’accès à l’emplacement dans l’administration pour définir la langue, le paramètre régional, le fuseau horaire et la devise par défaut.
* Historique de connexion à l&#39;accès - Donne aux utilisateurs l&#39;accès à l&#39;historique de connexion à l&#39;utilisateur dans la piste d&#39;audit
* Paramètres de connexion d’accès : donne aux utilisateurs l’accès aux paramètres de connexion dans les paramètres d’administration de la sécurité, des restrictions d’adresse IP et des rapports de Liste dynamique.
* Accès à l&#39;Activité personnalisée du marketing - Donne aux utilisateurs l&#39;accès aux Activités personnalisées du marketing dans l&#39;administration
* Accéder à l&#39;objet personnalisé Marketo - Donne aux utilisateurs l&#39;accès aux objets personnalisés Marketo dans Admin
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

## API d’accès  {#access-api}

Donne aux utilisateurs dotés du **rôle** **API uniquement** l’accès aux API individuelles répertoriées ci-dessous.

* Approbation des ressources
* Exécuter Campaign
* Activité en lecture seule
* Métadonnées d’Activité en lecture seule
* Fichiers en lecture seule
* Campaign en lecture seule
* Société en lecture seule
* Objet personnalisé en lecture seule
* Personne en lecture seule
* Compte nommé en lecture seule
* Opportunité en lecture seule
* Personne vendeuse en lecture seule
* Activité en lecture-écriture
* Métadonnées d’Activité en lecture-écriture
* Fichiers en lecture-écriture
* Campaign en lecture-écriture
* Société en lecture-écriture
* Objet personnalisé en lecture-écriture
* Personne en lecture-écriture
* Compte nommé en lecture-écriture
* Opportunité de lecture-écriture
* Personne vendeuse en lecture-écriture

Accès à Analytics

Donne aux utilisateurs l’accès aux onglets Analytics, aux statistiques d’e-mail, aux rapports et aux trois éléments ci-dessous, sauf s’ils sont désactivés.

* Accès à l&#39;Explorateur des recettes - La désactivation supprime l&#39;accès de l&#39;utilisateur à l&#39;Explorateur des recettes.
* Supprimer le rapport - La désactivation supprime la possibilité pour l&#39;utilisateur de supprimer des rapports.
* Exportation des données Analytics - La désactivation supprime la possibilité pour l’utilisateur d’exporter des données Analytics.

## Accéder au calendrier Presentations {#access-calendar-presentations}

Donne aux utilisateurs l&#39;accès aux présentations Calendrier ? ?- permet l&#39;affichage du bouton Presentations en bas ?

* Modifier le calendrier Presentations : permet aux utilisateurs de modifier des présentations dans le calendrier

## Access Design Studio {#access-design-studio}

Donne aux utilisateurs l’accès à l’onglet Design Studio et à la vue de l’arborescence, mais pas aux détails.

* Courriel d&#39;accès

   * Modifier le courrier électronique : permet aux utilisateurs de modifier, créer et cloner des courriers électroniques.

      * Optimiser le courrier électronique : permet aux utilisateurs de rendre un courrier électronique opérationnel. Voir : [Optimiser le courrier électronique](../../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)
   * Approuver le courrier électronique : permet aux utilisateurs d&#39;approuver les courriers électroniques.
   * Supprimer un courrier électronique : permet aux utilisateurs de supprimer des courriers électroniques.
   * Définir un domaine de marque : permet aux utilisateurs de travailler avec des domaines de marque. Voir : [Ajouter plusieurs domaines de marque](http://docs.marketo.com/display/docs/add+multiple+branding+domains)


* Accéder au modèle de courrier électronique

   * Approuver le modèle de courrier électronique
   * Supprimer le modèle de courrier électronique
   * Modifier un modèle de courrier électronique - Modifier, créer et cloner des modèles de courrier électronique

* Formulaire d&#39;accès

   * Supprimer le formulaire
   * Modifier le formulaire - Modifier, créer et cloner des formulaires

* Image d’accès

   * Supprimer l&#39;image
   * Télécharger l’image

* Landing page d&#39;accès

   * Approuver le Landing page
   * Supprimer le Landing page
   * Modifier le Landing page - Modifier, créer et cloner des landings page

* Modèle de Landing page d&#39;accès

   * Approuver le modèle de Landing page
   * Supprimer le modèle de Landing page
   * Modifier un modèle de Landing page - Modifier, créer et cloner des modèles de landing page

* Extrait d&#39;accès

   * Approuver un extrait de code
   * Supprimer un extrait de code
   * Modifier un extrait de code

* Accès à l’application Social

   * Approbation de l’application Social
   * Supprimer l’application Social
   * Modifier l’application Social

## Base de données d&#39;accès {#access-database}

Vue de la base de données ainsi que de la vue et modification des listes dynamiques/statiques.

* Segmentation des accès

   * Approuver la segmentation
   * Supprimer la segmentation
   * Modifier la segmentation

* Importation avancée de Liste
* Supprimer une personne
* Supprimer la Liste
* Modifier la personne - Empêche la modification manuelle et l&#39;exécution d&#39;étapes de flux simples ; vous pouvez toujours modifier des personnes en exécutant des campagnes contre elles.
* Exporter une personne - Exporter des feuilles de calcul à partir de vos listes de base de données
* Importer un objet personnalisé
* Liste d’importation
* Fusionner les personnes
* Exécuter des actions de flux unique : permet aux utilisateurs d&#39;exécuter l&#39;étape de flux **Modifier la valeur** des données sur les personnes de la base de données.

* Données d&#39;opportunité de vue - Masque les informations d&#39;opportunité sur la page de détails de la personne

## Accès aux Activités marketing {#access-marketing-activities}

Vue de l’onglet Activités marketing, des campagnes et des dossiers de campagne.

* Message SMS d&#39;accès

   * Approuver le message SMS
   * Supprimer un message SMS
   * Modifier le message SMS

* Notification Push d&#39;accès

   * Approuver la notification Push
   * Supprimer la notification Push
   * Modifier la notification Push

* Prix Access
* Activer le déclencheur Campaign
* Approuver le Programme de messagerie
* Cloner une ressource marketing
* Supprimer un actif marketing
* Modifier les restrictions Campaign
* Modifier le fichier marketing
* Programme d’importation
* Importation liste
* Planification de la Campaign par lot

Accès au référencement

* Administrer l’optimisation du référencement
* SEO standard

## Ciblage et personnalisation {#targeting-and-personalization}

* Administration de la personnalisation Web
* CRE Campaign Editor
* Lancement Campaign CRE
* Éditeur Web Campaign
* Lancement Web Campaign

Administration de Workspace

* Accès administrateur pour un espace de travail spécifique (uniquement si les espaces de travail sont activés)
* Déplacement de fichiers entre les espaces de travail (uniquement si les espaces de travail sont activés)

Accès à l&#39;application mobile
