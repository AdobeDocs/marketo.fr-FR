---
description: Notes de mise à jour - Mai 2022 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Mai 2022
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Notes de mise à jour : mai 2022 {#release-notes-may-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 mai. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

**_Versions trimestrielles_**

Les fonctionnalités suivantes commenceront à être publiées le **6 mai 2022**, avec un déploiement progressif des fonctionnalités restantes au cours des semaines suivantes (sauf indication contraire).

## Intégration CRM native {#native-crm-integration}

**[Intégration CRM native de Veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilité limitée)** : améliorez l&#39;engagement avec les professionnels de santé en synchronisant l&#39;activité entre la CRM de Veeva et le Marketo Engage via l&#39;intégration native. Cette intégration permet aux marketeurs de créer des expériences cross-canal plus personnalisées et plus transparentes pour les professionnels de la santé. Contactez l’équipe du compte d’Adobe (votre gestionnaire de compte) si vous souhaitez participer.

## Orchestration cross-canal {#cross-channel-orchestration}

**Événements Chatbot pour le Dynamic Chat** : tirez parti de données de comportement plus détaillées pour les visiteurs web, telles que le temps passé sur la page, le temps passé sur le site et le pourcentage de défilement de la page, afin de définir à quel moment une boîte de dialogue de conversation doit être affichée.

**Incorporation de PDF pour Dynamic Chat** : augmentez l’engagement et partagez du contenu significatif en incorporant des PDF dans les boîtes de dialogue de conversation et mesurez les performances du contenu grâce au suivi des activités d’engagement.

**Prise en charge étendue de la langue pour le Dynamic Chat** : l’interface utilisateur du Dynamic Chat sera désormais disponible en français, allemand, japonais, portugais et espagnol. Les boîtes de dialogue de conversation peuvent également être configurées dans ces langues.

**Exclure les URL pour le Dynamic Chat** : contrôlez le Dynamic Chat de vos pages web qui apparaît avec la possibilité d’exclure des URL spécifiques des critères de ciblage.

**[Améliorations du filtrage de l’activité des robots d’email](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}** : continuez à protéger l’intégrité de votre base de données avec la possibilité d’identifier le comportement des robots en fonction des agents utilisateur ou des adresses IP de lien masqué et des modèles de proximité, en plus de l’identification des correspondances de liste IAB existante. Affichez les statistiques de l’activité des robots qui vous permettent de comprendre le nombre d’activités de robots identifiées pour chaque type.

**[En-tête STS pour les liens de suivi d’email](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}** : respectez les bonnes pratiques de sécurité en appliquant des en-têtes Secure Transport Security pour vous assurer que le trafic vers les liens trackés est toujours sécurisé.

## Expérience de nouvelle génération {#modern-ux}

**Basculer vers l’expérience de nouvelle génération par défaut** : le bouton bascule sera défini par défaut sur la nouvelle expérience dans tous les écrans où il est disponible, ce qui permettra aux utilisateurs de découvrir plus facilement les conceptions mises à jour et les améliorations de la convivialité.

**Écran mis à jour dans l’expérience de nouvelle génération** :

Nous fournissons la vue Détails du modèle d’email dans Design Studio dans l’expérience de nouvelle génération, qui offre une conception et des améliorations de convivialité mises à jour accessibles par basculement.

## Automatisation de l’expérience {#experience-automation}

**Étapes de flux en libre-service (version bêta continue)** : développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes dynamiques. Les utilisateurs Marketo Engage et les partenaires peuvent exploiter cette fonctionnalité pour permettre l’utilisation de services web externes dans des campagnes déclencheuses, par lots et exécutables (contrairement aux webhooks qui ne peuvent être utilisés que dans des campagnes déclencheuses).

## Améliorations des API {#api-enhancements}

* **Accès à l’API étendu pour les abonnements CRM** : nous développons l’accès à l’API pour les abonnements pour lesquels une synchronisation CRM est activée afin de permettre aux utilisateurs de récupérer les entreprises, opportunités et commerciaux du Marketo Engage.
* **Prise en charge des types de données &quot;masqués&quot; dans Forms** : permet de gérer les champs de formulaire masqués via l’API.
* **Prise en charge de plusieurs valeurs de comparaison pour isNot Form via Rules** : gérez la visibilité des champs de formulaire selon que la valeur d’un autre champ n’est pas l’une des valeurs d’une liste donnée.
* **Paramètre Autoriser l’affichage et les valeurs envoyées dans Sélectionner les listes séparément** : définissez séparément la valeur d’affichage et la valeur envoyée dans un champ. Par exemple, affichez le nom d’un hôtel, mais envoyez un ID interne au serveur principal.
* **Autoriser la définition de l’option Désactiver le suivi d’ouverture lors de la création ou de la mise à jour d’un email** : créez un email avec le suivi d’ouverture désactivé.

## Annonces {#announcements}

**Vérification des emails et unicité** : à compter du mois d’avril, le déploiement de la vérification des emails commencera. À ce stade, les adresses électroniques des utilisateurs Marketo Engage devront être vérifiées et uniques (cela ne s’applique pas aux utilisateurs d’API uniquement). Les courriers électroniques des utilisateurs authentifiés du service d’annuaire seront automatiquement vérifiés lorsque leur abonnement sera activé avec la vérification des courriers électroniques.

La vérification des e-mails pour les abonnements à l’aide de la fonction &quot;Se connecter dans la boîte de dialogue d’invitation&quot; ou pour lesquels un e-mail unique est associé à plusieurs utilisateurs coïncide avec la version de mai. Les abonnements auxquels un seul message électronique est associé à plusieurs utilisateurs seront activés avec la vérification par courrier électronique et nécessiteront que ces utilisateurs résolvent le conflit et utilisent un message électronique unique par utilisateur. Lorsque la fonction &quot;Connexion à la boîte de dialogue d’invitation d’utilisateur&quot; est activée, les utilisateurs invités via cette fonction doivent disposer d’une adresse électronique unique. Pour les utilisateurs d’API uniquement invités via cette fonctionnalité, l’adresse électronique n’a pas besoin d’être unique.

**Modification du comportement des dossiers d’archives** : avec cette version, la possibilité de créer de nouvelles ressources dans les dossiers d’archives ne sera plus disponible à partir des menus contextuels de l’arborescence. Les options de menu permettant de créer des ressources sont masquées pour toutes les ressources. [En savoir plus ici](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinaire sur la version du produit_**

[Webinaire de mise à jour des Marketo Engage de mars et mai 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
