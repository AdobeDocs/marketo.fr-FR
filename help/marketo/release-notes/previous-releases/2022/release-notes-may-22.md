---
description: Notes De Mise À Jour - Mai 2022 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Mai 2022
exl-id: f591ab95-5ad8-45fa-8c4e-8e42b5d1359a
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# Notes De Mise À Jour : Mai 2022 {#release-notes-may-22}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 mai. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Marketo Engage pour en savoir plus.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **6 mai 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes (sauf indication contraire).

## Intégration native de CRM {#native-crm-integration}

**[Intégration native de Veeva CRM](/help/marketo/product-docs/crm-sync/veeva-crm-sync/understanding-the-veeva-crm-sync.md){target="_blank"} (disponibilité limitée)** : Améliorez l&#39;engagement avec les professionnels de santé en synchronisant l&#39;activité entre Veeva CRM et Marketo Engage via l&#39;intégration native. Cette intégration permet aux professionnels du marketing de créer des expériences cross-canal plus personnalisées et transparentes pour les professionnels de la santé. Contactez votre responsable du succès client si vous souhaitez participer.

## Orchestration cross-canal {#cross-channel-orchestration}

**Événements de bot conversationnel pour[!DNL Dynamic Chat]** : utilisez des données de comportement plus détaillées pour les visiteurs et visiteuses web, telles que le temps passé sur la page, le temps passé sur le site et le pourcentage de défilement de la page, pour définir à quel moment une boîte de dialogue de conversation doit s’afficher.

**PDF Embed for[!DNL Dynamic Chat]** : accroît l’engagement et partage du contenu significatif en incorporant des fichiers PDF dans les boîtes de dialogue de conversation et mesure les performances du contenu grâce au suivi des activités d’engagement.

**Prise en charge étendue des langues pour les[!DNL Dynamic Chat]** : l’interface utilisateur [!DNL Dynamic Chat] sera désormais également disponible en français, en allemand, en japonais, en portugais et en espagnol. Les boîtes de dialogue de conversation peuvent également être configurées dans ces langues.

**Exclure des URL pour les[!DNL Dynamic Chat]** : contrôlez [!DNL Dynamic Chat] pages web sur lesquelles apparaît la possibilité d’exclure des URL spécifiques des critères de ciblage.

**[Améliorations du filtrage des activités de robots d’e-mail](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"}** : continuez à protéger l’intégrité de votre base de données en permettant d’identifier le comportement des robots en fonction des liens masqués, des agents utilisateur ou des adresses IP et des modèles de proximité, en plus de l’identification de correspondance de liste IAB existante. Affichez les statistiques des activités de robots qui vous permettent de comprendre le nombre d’activités de robots identifiées pour chaque type.

**[En-tête STS pour les liens de suivi d’e-mail](/help/marketo/product-docs/administration/settings/email-tracking-link-headers.md){target="_blank"}** : appliquez les bonnes pratiques de sécurité en appliquant des en-têtes Secure Transport Security pour vous assurer que le trafic vers les liens suivis est toujours sécurisé.

## Expérience nouvelle génération {#modern-ux}

**Basculer vers l’expérience de nouvelle génération par défaut** : le bouton (bascule) est défini par défaut sur la nouvelle expérience sur tous les écrans où il est disponible, ce qui facilite la découverte des conceptions mises à jour et les améliorations de la convivialité.

**Écran mis à jour dans l’expérience de nouvelle génération** :

Nous fournissons une vue détaillée du modèle d’e-mail dans [!UICONTROL Design Studio] dans l’expérience de nouvelle génération, offrant une conception et des améliorations de convivialité mises à jour accessibles via le bouton bascule.

## Automatisation de l’expérience {#experience-automation}

**Étapes de flux en libre-service (bêta continue)** : développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes intelligentes. Les utilisateurs et partenaires de Marketo Engage peuvent tirer parti de cette fonctionnalité pour permettre l’utilisation de services web externes dans les campagnes de déclenchement, par lots et exécutables (contrairement aux webhooks qui ne peuvent être utilisés que dans les campagnes de déclenchement).

## Améliorations de l’API {#api-enhancements}

* **Accès étendu aux API pour les abonnements compatibles CRM** : nous étendons l’accès aux API pour les abonnements pour lesquels la synchronisation CRM est activée afin de permettre aux utilisateurs de récupérer les entreprises, les opportunités et les commerciaux dans Marketo Engage.
* **Prise en charge des types de données « masqués » dans Forms** : permet de gérer les champs de formulaire masqués via l’API.
* **Prendre en charge des valeurs de comparaison multiples pour isNot Form via des règles** : permet de gérer la visibilité des champs de formulaire selon que la valeur d’un autre champ ne figure pas ou non parmi les valeurs d’une liste donnée.
* **Autoriser le paramétrage distinct des valeurs d’affichage et des valeurs envoyées dans Sélectionner des listes** : définissez séparément la valeur d’affichage et la valeur envoyée dans un champ. Par exemple, affichez le nom d’un hôtel, mais envoyez un ID interne au serveur principal.
* **Autoriser la désactivation du suivi des ouvertures lors de la création ou de la mise à jour d’un e-mail** : créez un e-mail avec le suivi des ouvertures désactivé.

## Annonces {#announcements}

**Vérification des e-mails et singularité** : à partir d’avril, le déploiement de la vérification des e-mails commencera. À ce stade, les adresses e-mail des utilisateurs de Marketo Engage devront être vérifiées et être uniques (cela ne s’applique pas aux utilisateurs utilisant uniquement l’API). Les utilisateurs authentifiés du service d’annuaire verront automatiquement leurs e-mails vérifiés lorsque leur abonnement sera activé avec la vérification par e-mail.

La vérification des e-mails pour les abonnements utilisant la fonctionnalité « [!UICONTROL Se connecter à la boîte de dialogue d’invitation de l’utilisateur] » ou qui ont un seul e-mail associé à plusieurs utilisateurs coïncidera avec la version de mai. La vérification des e-mails sera activée pour les abonnements qui comportent un seul e-mail associé à plusieurs utilisateurs. Ces utilisateurs devront résoudre le conflit et utiliser un e-mail unique par utilisateur. Lorsque la fonction « Connexion à la boîte de dialogue d’invitation d’utilisateur » est activée, les utilisateurs invités via cette fonction doivent avoir une adresse e-mail unique. Pour les utilisateurs et utilisatrices uniquement invités par le biais de cette fonctionnalité, l’adresse e-mail n’a pas besoin d’être unique.

**Modification du comportement du dossier d’archivage** : avec cette version, la possibilité de créer des ressources dans les dossiers d’archivage ne sera plus disponible dans les menus contextuels de l’arborescence. Les options de menu de création de ressources seront masquées pour toutes les ressources. [En savoir plus ici](https://nation.marketo.com/t5/product-discussions/archive-folder-change-in-may-2022-release/m-p/324369#M183235){target="_blank"}.

**_Webinaire de mise à jour du produit_**

[Webinaire de mise à jour de Marketo Engage de mars et mai 2022](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}
