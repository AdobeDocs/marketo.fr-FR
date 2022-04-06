---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 2ac0ef0b715eb2acd03fe2c5ad4cfee8daeef4f6
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Notes de mise à jour : Mai 2022 {#release-notes-may-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 mai. Vérifiez la disponibilité de votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_**

Les fonctionnalités suivantes commenceront à être publiées sur **6 mai 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes (sauf indication contraire).

## Intégration CRM native {#native-crm-integration}

**Intégration de la gestion de la relation client (disponibilité limitée) native de Veeva**: Améliorer l&#39;engagement avec les professionnels de santé en synchronisant l&#39;activité entre Veeva VRM et Marketo Engage via l&#39;intégration native. Cette intégration permet aux marketeurs de créer des expériences cross-canal plus personnalisées et plus transparentes pour les professionnels de la santé. Contactez votre responsable du succès client si vous souhaitez participer.

## Orchestration cross-canal {#cross-channel-orchestration}

**Événements Chatbot pour les conversations dynamiques**: Tirez parti de données de comportement plus détaillées pour les visiteurs web, telles que le temps passé sur la page, le temps passé sur le site et le pourcentage de défilement de la page, afin de définir à quel moment une boîte de dialogue de conversation doit être affichée.

**Incorporation de PDF pour Dynamic Chat**: Augmentez l’engagement et partagez du contenu significatif en incorporant des PDF dans les boîtes de dialogue de conversation et en mesurant les performances du contenu par le biais du suivi des activités d’engagement.

**Prise en charge linguistique étendue pour Dynamic Chat**: L’interface utilisateur de Dynamic Chat sera désormais disponible en allemand, en français, en japonais, en portugais et en espagnol. Les boîtes de dialogue de conversation peuvent également être configurées dans ces langues.

**Exclure des URL pour la messagerie instantanée dynamique**: Contrôlez les pages de vos pages web avec la possibilité d’exclure des URL spécifiques des critères de ciblage.

**Améliorations du filtrage des activités des robots de messagerie**: Continuez à protéger l’intégrité de votre base de données avec la possibilité d’identifier le comportement des robots en fonction des agents utilisateur ou des adresses IP des liens masqués et des modèles de proximité, en plus de l’identification des correspondances de liste IAB existante. Affichez les statistiques des activités de robots qui vous permettent de comprendre le nombre d’activités de robots identifiées pour chaque type.

**En-tête STS pour les liens de suivi de courrier électronique**: Respectez les bonnes pratiques en matière de sécurité avec la possibilité d’appliquer des en-têtes Secure Transport Security pour garantir que le trafic vers les liens trackés est toujours sécurisé.

## Expérience de nouvelle génération {#next-generation-experience}

**Basculer vers l’expérience de nouvelle génération par défaut**: le bouton bascule sera défini par défaut sur la nouvelle expérience dans tous les écrans où il est disponible, ce qui permettra aux utilisateurs de découvrir plus facilement les conceptions et les améliorations de convivialité mises à jour.

**Écran mis à jour dans l’expérience de génération suivante**:

Nous fournissons la vue Détails du modèle d’email dans Design Studio dans l’expérience de nouvelle génération, qui offre une conception et des améliorations de convivialité mises à jour accessibles par basculement.

## Automatisation de l’expérience {#experience-automation}

**Étapes de flux en libre-service (version bêta continue)**: Développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes dynamiques. Les utilisateurs Marketo Engage et les partenaires peuvent exploiter cette fonctionnalité pour permettre l’utilisation de services web externes dans des campagnes déclencheuses, par lots et exécutables (contrairement aux webhooks qui ne peuvent être utilisés que dans des campagnes déclencheuses).

## Améliorations des API {#api-enhancements}

* **Accès aux API étendu pour les abonnements CRM**: Nous développons l’accès aux API pour les abonnements pour lesquels une synchronisation CRM est activée afin de permettre aux utilisateurs de récupérer les sociétés, opportunités et personnes chargées de la vente auprès de Marketo Engage.
* **Prise en charge des types de données &quot;masqués&quot; dans Forms**: Permet de gérer les champs de formulaire masqués via l’API.
* **Prise en charge de plusieurs valeurs de comparaison pour isNotForm via des règles**: Gérez la visibilité des champs de formulaire selon que la valeur d’un autre champ n’est pas une des valeurs d’une liste donnée.
* **Autoriser la définition des valeurs d’affichage et d’envoi dans certaines listes séparément**: Définissez la valeur d’affichage et la valeur envoyée séparément dans un champ. Par exemple, affichez le nom d’un hôtel, mais envoyez un ID interne au serveur principal.
* **Autoriser la définition de l’option Désactiver le suivi d’ouverture lors de la création ou de la mise à jour d’un email**: Créez un email avec le suivi des ouvertures désactivé.

## Annonces {#announcements}

**Vérification des emails et unicité**: À compter du mois d’avril, le déploiement de la vérification des courriers électroniques commencera. À ce stade, les adresses électroniques des utilisateurs Marketo Engage devront être vérifiées et uniques (cela ne s’applique pas aux utilisateurs d’API uniquement). Les courriers électroniques des utilisateurs authentifiés du service d’annuaire seront automatiquement vérifiés lorsque leur abonnement sera activé avec la vérification des courriers électroniques.

La vérification des e-mails pour les abonnements à l’aide de la fonction &quot;Se connecter dans la boîte de dialogue d’invitation&quot; ou pour lesquels un e-mail unique est associé à plusieurs utilisateurs coïncide avec la version de mai. Les abonnements auxquels un seul message électronique est associé à plusieurs utilisateurs seront activés avec la vérification par courrier électronique et nécessiteront que ces utilisateurs résolvent le conflit et utilisent un message électronique unique par utilisateur. Lorsque la fonction &quot;Connexion à la boîte de dialogue d’invitation d’utilisateur&quot; est activée, les utilisateurs invités via cette fonction doivent disposer d’une adresse électronique unique. Pour les utilisateurs d’API uniquement invités via cette fonctionnalité, l’adresse électronique n’a pas besoin d’être unique.

**_Webinaire sur la version du produit_**

Rejoignez-nous le 11 mai 2022, à 9h00 PT / 12h00 ET pour une [webinaire en direct](https://engage.marketo.com/2022_March_May_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} hébergé par notre équipe produit où vous pouvez apprendre à utiliser toutes les dernières innovations de produit.
