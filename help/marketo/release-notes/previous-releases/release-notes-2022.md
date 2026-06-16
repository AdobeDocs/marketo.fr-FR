---
title: 2022
description: 2022 - Documents Marketo - Documentation Du Produit
feature: Release Information
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
  - id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 992f0ad35d396b1f6ecd30f34ba1d228116fb264
workflow-type: tm+mt
source-wordcount: 4282
ht-degree: 6%

---

# 2022

## Janvier 2022 {#january}

Les fonctionnalités suivantes sont incluses dans la version de janvier 2022. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **21 janvier 2022**, avec un déploiement échelonné de chaque fonctionnalité au cours des semaines suivantes (sauf indication contraire).

## Expérience nouvelle génération

* **Mise à jour de Screens dans l’expérience de nouvelle génération** : nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour et accessibles via le bouton bascule :

   * Détails de la ressource de page de destination dans [!UICONTROL Design Studio]
   * Détails de la ressource de page de destination dans [!UICONTROL Activités marketing]

## Intégration [!DNL Microsoft Dynamics] {#microsoft-dynamics-integration}

* **Synchronisation du type de champ de jeu d’options à sélection multiple généralement disponible** : synchronisez le type de champ de jeu d’options à sélection multiple de [!DNL Microsoft Dynamics] pour l’exploiter dans les listes dynamiques et les campagnes dynamiques pour un ciblage d’audience plus granulaire. Par exemple : sujets/produits d’intérêt, modes de communication préférés, etc. Cette nouvelle synchronisation est disponible pour [!DNL Microsoft Dynamics] version 9.X (y compris Dynamics 365 Online).

* **Authentification de serveur à serveur pour[!DNL Microsoft Dynamics 365 Online]** : pour une sécurité accrue, nous prendrons désormais en charge Serveur à serveur (S2S) en tant que mode d’authentification supplémentaire pour l’utilisateur de la synchronisation Marketo Engage sur Azure Active Directory pour un accès non interactif à [!DNL Microsoft Dynamics 365 Online]. Vous pouvez ainsi utiliser l’authentification à plusieurs facteurs, car toutes les authentifications seront basées sur OAuth (uniquement l’identifiant et le secret client).

>[!NOTE]
>
>Le mode S2S est basé sur l’utilisateur de l’application plutôt que sur l’utilisateur sous licence, ce qui permet d’économiser l’utilisation d’une licence supplémentaire.

## Administration {#administration}

* **[Règles de validation des formulaires](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)** : préservez l’intégrité de votre base de données et bloquez les domaines d’e-mail problématiques ou indésirables pour l’envoi de formulaires Marketo Engage. Le panneau Règle de validation globale des formulaires permet aux administrateurs de définir une liste bloquée ou d’activer une liste prédéfinie de domaines consommateurs libres à bloquer des formulaires.

* **[Sécurité des en-têtes de page de destination](/help/marketo/product-docs/administration/settings/landing-page-headers.md)** : les administrateurs peuvent gérer les en-têtes Strict Transport Security et X-Frame Options sur leurs domaines de page de destination pour appliquer des exigences de sécurité strictes.

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes font l’objet d’un cycle non trimestriel et seront publiées au cours des prochains mois.

## Connecteur de destination AEP Marketo Engage - Créer de nouveaux prospects {#aep-marketo-engage-destination-connector}

Les clients Marketo Engage qui utilisent également Adobe Experience Platform (AEP) peuvent optimiser leur base de données grâce à la possibilité d’envoyer des enregistrements de nouvelles personnes dans Marketo Engage depuis AEP via le connecteur de destination AEP. Lors de l’envoi de segments d’audience d’AEP vers Marketo Engage, les personnes du segment qui n’existent pas encore dans votre base de données Marketo Engage [peuvent y être automatiquement ajoutées](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## [!DNL Sales Insight] {#sales-insight}

![(étoile)](assets/yellow-star.png)

**[!DNL Sales Insight]pour [!DNL Salesforce] CRM**

* **Nouvelle colonne de type pour les [!UICONTROL Meilleurs résultats]** : les vendeurs obtiendront des informations plus rapides grâce à une nouvelle colonne intitulée « Type » pour différencier les prospects et les contacts sur la page [!UICONTROL Meilleurs résultats].

* **[!DNL Salesforce]mise à jour de l’API Platform** : en réponse au retrait [!DNL Salesforce] des versions 21.0 à 30.0 de l’API [!DNL Salesforce] Platform, le package [!DNL Sales Insight] a été mis à jour avec les dernières API.

* **Image de marque mise à jour** : toutes les pages [!DNL Sales Insight] sont mises à jour pour s’aligner sur l’image de marque Adobe.

**[!DNL Sales Insight]for[!DNL Microsoft Dynamics]**

* **Mise à jour de la disposition du compte** : les vendeurs peuvent obtenir une vue collective des principales activités, telles que : les activités de messagerie électronique, les activités web, les moments intéressants et les changements de score pour tous les contacts d’un compte.

## [!DNL Sales Connect] {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Résultats et motifs de l’appel** : comprenez et suivez plus en détail les efforts sortants de vos équipes commerciales grâce à de nouvelles options entièrement personnalisables de résultat d’appel et de motif d’appel. Outre ces nouveaux champs, nous introduisons une nouvelle gouvernance pour appliquer la sélection du motif de l’appel et du résultat pendant que les vendeurs effectuent des appels, une nouvelle gouvernance pour activer ou désactiver les motifs et les résultats des appels, ainsi qu’un nouveau champ personnalisé Motif de l’appel et Activité de [!DNL Salesforce] du résultat de l’appel pour la journalisation des données dans les [!DNL Salesforce]. [Cliquez ici](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) pour en savoir plus.

* Personnalisation des détails de l’activité **[!DNL Salesforce]** : capturez d’autres données d’activité de vente et de tâche dans [!DNL Salesforce] en personnalisant les informations qui sont ajoutées au champ d’objet de la tâche [!DNL Salesforce] lorsqu’une activité de vente est consignée dans un [!DNL Salesforce] à partir de [!DNL Sales Connect]. [Cliquez ici](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) pour en savoir plus.

## Annonces {#announcements}

* **Obsolescence de Marketo Sky** : en mars, Marketo Sky ne sera plus disponible, car nous concentrons nos ressources sur la diffusion de l’expérience utilisateur de nouvelle génération. Dans un effort de conserver l’accès à une fonctionnalité exclusive à Marketo Sky aujourd’hui, nous intégrons l’expiration des ressources et le remplacement de priorité de campagne intelligent dans l’expérience grand public de mars. [Cliquez ici](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) pour en savoir plus.

* **Obsolescence des points d’entrée de formulaire** : les publications de formulaire programmatiques non prises en charge sur le point d’entrée leadCapture/save2 seront rejetées par les formulaires Marketo Engage. [Cliquez ici](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) pour en savoir plus.

* **Connexion à la boîte de dialogue d’invitation d’utilisateur** : en mars, la fonctionnalité facultative existante « Connexion à la boîte de dialogue d’invitation d’utilisateur » sera abandonnée. La fonctionnalité « [!UICONTROL Se connecter dans la boîte de dialogue d’invitation d’utilisateur] » est remplacée par la fonctionnalité d’ID universel, requise pour la prochaine intégration du système Adobe Identity Management et activée en août 2021 sur tous les abonnements. Suite à l’obsolescence, Marketo Engage n’obligera qu’un seul utilisateur à être associé par adresse e-mail dans un abonnement.

**Domaines Marketo Engage - Configuration [!DNL Sales Insight]** : pour les domaines Marketo Engage pour lesquels le certificat SSL n&#39;est pas configuré et pour https://, les appels échouent avec une erreur de négociation SSL. Par conséquent, ces domaines vont disparaître. Par conséquent, les utilisateurs [!DNL Sales Insight] disposant d’une configuration plus ancienne pointant vers l’un de ces domaines peuvent rencontrer des erreurs de légende système sur leur page Lead, Contact, Compte, Panneaux d’opportunité ou Page globale Marketo. Nous vous recommandons de mettre à jour votre configuration [&#128279;](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) dans [!DNL Salesforce] si vous rencontrez cette erreur. Il vous suffit de mettre à jour les informations d’identification Marketo Engage mises en surbrillance dans la section « Configuration [!DNL Marketo Sales Insight] » du document.

**_Webinaire de mise à jour du produit_**

[Webinaire De Mise À Jour De Janvier 2022 Pour Marketo Engage](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)

## Mars 2022 {#march}

Les fonctionnalités suivantes sont incluses dans la version de mars 2022. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

**_Versions trimestrielles_**

Les fonctionnalités suivantes seront publiées le **11 mars 2022**, avec un déploiement échelonné de chaque fonctionnalité au cours des semaines suivantes (sauf indication contraire).

## Orchestration cross-canal {#cross-channel-orchestration}

* **[!DNL Dynamic Chat]** : maximisez chaque opportunité sur votre site web en ciblant les prospects et les comptes avec des conversations proactives, attrayantes et 1:1 personnalisées. [&#128279;](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md){target="_blank"} permet aux utilisateurs de Marketo Engage de commencer à utiliser le chat comme élément clé des expériences cross-canal intégrées pour les cas d’utilisation de marketing et de ventes B2B. Les fonctionnalités incluent : la possibilité de réserver des réunions directement dans le chat, le routage des prospects, les modèles de démarrage, la création de conversations par glisser-déposer, et bien plus encore. Dynamic Chat est inclus dans tous les packages Marketo Engage et sera déployé auprès de tous les utilisateurs Marketo Engage cette année.

* **Amélioration du filtrage des activités de robots d’e-mail** : en complément de la fonctionnalité [Filtrage des activités de robots d’e-mail](/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md){target="_blank"} publiée précédemment, vous pouvez désormais vous inscrire aux activités de journalisation identifiées comme des robots. Vous pouvez ensuite filtrer et déclencher des actions en fonction des activités identifiées comme étant exécutées par des robots.

## Expérience nouvelle génération

* **Mise à jour de Screens dans l’expérience de nouvelle génération** : nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour et accessibles via le bouton bascule :

   * Vue Liste des formulaires dans [!UICONTROL Design Studio] (y compris les nouvelles actions en masse)

* **Mise à jour du workflow d’importation du programme** : le workflow d’importation du programme est fourni dans l’expérience de nouvelle génération avec une conception et des améliorations de convivialité mises à jour. Il s’agira d’une modification automatique sans commutateur.

* **Contrôle d’administration pour le commutateur de basculement d’expérience de nouvelle génération** : gérez le déploiement de l’expérience de nouvelle génération d’une manière qui fonctionne pour vos utilisateurs et qui permet aux administrateurs de sélectionner les types d’utilisateurs pouvant accéder au commutateur de basculement.

## Automatisation de l’expérience {#experience-automation}

* **Étapes de flux en libre-service (Beta)** : développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes intelligentes. Les utilisateurs et partenaires de Marketo peuvent tirer parti de cette fonctionnalité pour permettre l’utilisation de services web externes dans les campagnes par lots et exécutables, contrairement aux webhooks, qui ne peuvent être utilisés que dans les campagnes de déclenchement.

* **Expiration des ressources** : contrôlez vos ressources et campagnes sensibles au facteur temps et planifiez leur désactivation automatique à une date et une heure spécifiées dans l’expérience utilisateur classique.

* **Remplacement de priorité de campagne intelligente** : assurez-vous que les campagnes intelligentes de déclenchement de priorité élevée s’exécutent dès que possible avec la possibilité de remplacer le classement de priorité de campagne standard. Les campagnes intelligentes à déclenchement de priorité inférieure peuvent également être réduites en priorité afin de libérer des ressources de traitement pour d’autres tâches de priorité élevée.

## Améliorations de l’API {#api-enhancements}

* **Renvoyer Désactiver le statut du suivi des ouvertures des e-mails** : permet la lecture du statut de suivi des ouvertures des e-mails via l’API
* **Récupérer les lignes d’objet de contenu dynamique de l’e-mail** : permet aux spécialistes marketing d’analyser les lignes d’objet dynamiques dans les outils de BI
* **CRUD des champs personnalisés des membres de programme** : permet aux spécialistes marketing de créer par programmation des champs personnalisés des membres de programme
* **Exportation d’objets personnalisés en bloc mise à jourAu filtre** : permet aux spécialistes marketing de synchroniser les objets personnalisés par programmation
* **Exposer le paramètre Head Start pour les programmes de messagerie électronique** : permet aux spécialistes du marketing de configurer des programmes de messagerie avec une avance via l’API
* **Mise à jour sélective des balises de programme** : permet aux marketeurs de pousser les mises à jour sélectives des balises sans pousser toutes les balises en même temps
* **Champ ActionResult de l’extraction d’activité en masse** : permet aux spécialistes marketing d’identifier les activités qui ont été ignorées ou ayant échoué

**_Publication tout au long du trimestre_**

Les fonctionnalités suivantes font l’objet d’un cycle non trimestriel et seront publiées au cours des prochains mois.

## [!DNL Bizible] {#bizible}

![(étoile)](assets/yellow-star.png)

* **Modèles BI** : [!DNL Bizible] fournira désormais des artefacts de rapports de base téléchargeables et des exemples de rapports pour Tableau et Power BI afin de permettre le développement rapide de rapports personnalisés adaptés aux besoins spécifiques de votre entreprise.

## [!DNL Sales Connect] {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **Ralentissement de la connexion aux e-mails (GA, Email Connection Throttling)** : le ralentissement de la connexion aux e-mails permet aux administrateurs [!DNL Sales Connect] de configurer le taux d’envoi des e-mails lors de l’utilisation de Gmail ou [!DNL Exchange] comme canal de diffusion, de sorte que le taux de transmission des e-mails au fournisseur de canal de diffusion ne dépasse pas les limites appliquées.

## Annonces {#announcements}

* **Obsolescence de Marketo Sky** : en mars, Marketo Sky ne sera plus disponible, car nous concentrons nos ressources sur la diffusion de l’expérience utilisateur de nouvelle génération. Dans un effort de conserver l’accès à une fonctionnalité exclusive à Marketo Sky aujourd’hui, nous ajoutons l’expiration des ressources et le remplacement de priorité de campagne intelligente à l’expérience classique. [Cliquez ici](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) pour en savoir plus.

**_Webinaire de mise à jour du produit_**

[Webinaire de mise à jour de mars et mai 2022 pour Marketo Engage](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## Mai 2022 {#may}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 mai. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

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

## Expérience nouvelle génération

**Basculer vers l’expérience de nouvelle génération par défaut** : le bouton (bascule) est défini par défaut sur la nouvelle expérience sur tous les écrans où il est disponible, ce qui facilite la découverte des conceptions mises à jour et les améliorations de la convivialité.

**Écran mis à jour dans l’expérience de nouvelle génération** :

Nous fournissons une vue détaillée du modèle d’e-mail dans [!UICONTROL Design Studio] dans l’expérience de nouvelle génération, offrant une conception et des améliorations de convivialité mises à jour accessibles via le bouton bascule.

## Automatisation de l’expérience {#experience-automation}

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

[Webinaire de mise à jour de mars et mai 2022 pour Marketo Engage](https://engage.marketo.com/2022_March_May_Release_Webinar_DemandPage.html){target="_blank"}

## Juin 2022 {#june}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 juin. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

Les fonctionnalités suivantes seront publiées le **24 juin 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes (sauf indication contraire).

## Environnement de données marketing {#marketing-data-environment}

* **Exposer les champs CreatedAt/UpdatedAt pour les objets personnalisés** : permet d’inspecter ces champs dans l’écran Détails de la personne pour obtenir des insight supplémentaires.

## Orchestration cross-canal {#cross-channel-orchestration}

* **Utilisation améliorée de Stream Designer pour les[!DNL Dynamic Chat]** : ajoutez des cartes directement à partir de la zone de travail de Stream Designer sans avoir à effectuer un glisser-déposer. L’interface [!DNL Dynamic Chat] a également été améliorée afin d’offrir une meilleure visibilité du contenu dans les cartes individuelles.

* **Règles avancées de routage des rendez-vous pour les[!DNL Dynamic Chat]** : [!DNL Dynamic Chat] offre davantage d’options de routage des rendez-vous ciblé. Spécifiez les rendez-vous d’agent qui doivent être acheminés en fonction des attributs de Marketo Engage, en vous assurant que les prospects sont acheminés vers les agents appropriés.

* **Rapports de boîte de dialogue avancés pour[!DNL Dynamic Chat]** : affichez plus en détail les performances de vos campagnes [!DNL Dynamic Chat] à l’aide de toutes nouvelles visualisations de données pour les mesures d’engagement et de conversion.

* **Désynchroniser les attributs Marketo Engage inutilisés pour les[!DNL Dynamic Chat]** : désynchronisez les attributs Marketo Engage de votre abonnement [!DNL Dynamic Chat] qui ne sont pas utilisés, ce qui vous permet de faciliter la propreté des données et de synchroniser d’autres attributs si nécessaire.

## Expérience nouvelle génération

**Nouveau bouton (bascule) des vues** : les vues ci-dessous sont désormais disponibles dans l’expérience de nouvelle génération :

* [Vue Détails de l’e-mail](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [Vue Liste d’e-mails](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Automatisation de l’expérience {#experience-automation}

* **Exclusions des règles de validation de champ de formulaire global** : excluez des formulaires spécifiques des règles de validation de formulaire global afin que les centres d’abonnements et d’autres workflows critiques pour l’entreprise puissent accepter toutes les valeurs.

* **Étapes de flux en libre-service** : développez la connectivité entre Marketo Engage et le reste de votre pile avec la possibilité de créer des étapes de flux personnalisées à utiliser dans les campagnes intelligentes. Les utilisateurs et partenaires de Marketo Engage peuvent tirer parti de cette fonctionnalité pour permettre l’utilisation de services web externes dans les campagnes déclencheuses, par lots et exécutables, contrairement aux Webhooks, qui ne peuvent être utilisés que dans les campagnes déclencheuses.

* **Suivi des liens incompatibles avec le protocole Munchkin** : étendez la prise en charge du suivi des liens `tel` et `mailto` avec Munchkin pour suivre l’ensemble étendu des comportements web.

* **Méthodes HTTP supplémentaires pour les Webhooks** : spécifiez PUT, PATCH et DELETE en tant que types de requête pour interagir avec les services web.

## [!DNL Sales Insight] {#sales-insight}

![(étoile)](assets/yellow-star.png)

* Jeu d’autorisations **[!DNL Sales Insight]dans[!DNL Salesforce]** : les administrateurs peuvent fournir un accès [!DNL Sales Insight] à un ensemble limité de personnes au niveau de l’utilisateur plutôt qu’au niveau du profil via le jeu d’autorisations de l’application Marketo, qui fait partie du package d’[!DNL Salesforce] [!DNL Sales Insight].

* **My Marketo Tile Update - [!DNL Sales Insight] Actions** : les administrateurs Marketo (et les utilisateurs qu’ils désignent) peuvent désormais accéder rapidement à leur instance [!DNL Sales Insight] Actions via une nouvelle mosaïque [!DNL Sales Insight] Actions située sur la page My Marketo.

## [!DNL Sales Connect] {#sales-connect}

![(étoile)](assets/yellow-star.png)

* **[!DNL Salesforce]mise à jour de l’API** : avec la version [!DNL Salesforce] de l’été 2022, les anciennes versions 21 à 30 de l’API ne seront plus prises en charge par [!DNL Salesforce]. Avec cette version de Marketo Engage, toutes les requêtes [!DNL Sales Connect] utilisant des versions d’API héritées ont été mises à jour afin de rester dans une version prise en charge. Pour plus d&#39;informations sur les plans de retraite des API [!DNL Salesforce], cliquez [ici](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}.

## Améliorations de l’API {#api-enhancements}

* **Nouvelles fonctionnalités de filtrage pour l’API d’extraction de membre de programme en bloc** : filtrez par statut d’appartenance au programme, updatedAt, cadence ou contenu épuisé pour affiner le jeu de données extrait.

* **Amélioration de l’API d’extraction des membres de programme en bloc** : spécifiez jusqu’à 10 programmes lors de la création de tâche pour améliorer le débit.

## Annonces {#announcements}

* **Obsolescence de Forms : Forms 1.0, point d’entrée de capture/enregistrement de prospect et versions de formulaires sans script** : la prise en charge des ressources Forms 1.0 sera complètement supprimée de Marketo Engage d’ici octobre 2022. Toutes les ressources Forms 1.0 existantes cesseront de fonctionner. Les formulaires Marketo Engage devront être chargés sur des pages de destination et des sites web sous JavaScript.

**_Webinaire de mise à jour du produit_**

[Webinaire de mise à jour de Marketo Engage juin et août 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## Août 2022 {#august}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 août. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

Le déploiement échelonné des fonctionnalités suivantes a commencé le **26 août 2022**.

## Orchestration cross-canal {#cross-channel-orchestration}

* Activer/désactiver toutes les boîtes de dialogue publiées en une seule fois pour [!DNL Dynamic Chat] ** : activez/désactivez globalement toutes les boîtes de dialogue publiées en une seule fois à partir de la page Configuration en appuyant sur un bouton.

* **Avatars personnalisés pour[!DNL Dynamic Chat]** : téléchargez un avatar de bot conversationnel personnalisé afin qu’il puisse être personnalisé pour votre marque.

* **Transcriptions de conversation pour les[!DNL Dynamic Chat]** : affichez les transcriptions de conversation pour chaque conversation afin d’obtenir une insight plus approfondie sur ce qui intéresse chaque visiteur web.

## Expérience nouvelle génération

* **Image de marque** : mise à jour de la page aspect pour les éditeurs et les détails de la personne avec la nouvelle image de marque Adobe Experience Cloud.

* **Afficher la hiérarchie des dossiers du dossier de destination dans la boîte de dialogue Déplacer** : l’affichage de la hiérarchie des dossiers pour chaque dossier facilite le déplacement des ressources et réduit la probabilité de les placer dans un mauvais dossier.

* **[Mise à jour de Screens dans l’expérience de nouvelle génération](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"}** : nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour et accessibles via le bouton bascule :

   * Détails du fragment de code
   * Détails « Images et fichiers »

>[!NOTE]
>
>Exception : déplacement d’une ressource vers un dossier au sein d’un programme dans les activités marketing. Cette action de déplacement n’affiche pas la hiérarchie de dossiers, car les dossiers d’un programme ne peuvent pas avoir de noms en double.

## Automatisation de l’expérience {#experience-automation}

* **[Étapes de flux en libre-service - Améliorations de l’importation de programmes](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/flow-step-service.md){target="_blank"}** : prise en charge améliorée de l’importation de programmes avec des étapes de flux personnalisées où vous pouvez désormais utiliser plusieurs instances du même fournisseur de services et importer des programmes dont les étapes de flux sont compatibles avec ces fournisseurs de services.

* **[!DNL Munchkin]- Suivi des liens étendu** : étendez la prise en charge du suivi des liens `tel` et `mailto` avec Munchkin pour suivre un ensemble étendu de comportements web.

* **Visibilité des en-têtes personnalisés Webhook** : les en-têtes personnalisés Webhook sont désormais affichés dans l’onglet [!UICONTROL Admin] > [!UICONTROL Webhooks] pour une meilleure visibilité.

* **CAPTCHA** : évaluez la validité des envois de formulaire [à l’aide de reCAPTCHA v3](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"} pour noter le trafic de formulaire entrant. Créez des workflows marketing pour exclure, mettre en quarantaine ou supprimer automatiquement le trafic de robots suspect.

* **Autorisation d’approuver le formulaire** : nouvelle autorisation permettant de contrôler quels concepteurs et conceptrices peuvent approuver les modifications apportées à un formulaire conformément aux autres ressources [!UICONTROL Design Studio]. Cela empêche d&#39;autres concepteurs d&#39;apporter des modifications aux formulaires sans que quelqu&#39;un d&#39;autre disposant d&#39;une autorisation l&#39;examine.

* **Toujours effectuer la relecture de la campagne après une fusion anonyme** : la fusion de leads anonymes se produit avant la relecture de la campagne, de sorte que les filtres de champ personnalisés se comportent de manière fiable lorsque la relecture de la campagne anonyme est effectuée.

## Environnement de données marketing {#marketing-data-environment}

* **Corriger la troncature de l’interface utilisateur des champs Objet personnalisé « [!UICONTROL Utilisé par] »** : il est désormais plus facile d’identifier les champs d’objet personnalisés « en cours d’utilisation » afin que vous puissiez supprimer des champs d’un objet personnalisé si nécessaire.

## Améliorations de l’API {#api-enhancements}

* **Nouvelles fonctionnalités de filtrage pour l’API d’extraction de membre de programme en bloc** : filtrez par statut d’appartenance au programme, mise à jour d’at, cadence ou contenu épuisé pour affiner le jeu de données extrait.

## [!DNL Sales Insight] {#sales-insight}

![(étoile)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Intégration à [!DNL Dynamic Chat]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}** : affichez les activités des [!DNL Dynamic Chat] dans le panneau [!DNL Sales Insight] et exploitez ce nouveau point de données dans votre effort de prospection.

## Annonces {#announcements}

**_Webinaire de mise à jour du produit_**

[Webinaire de mise à jour de Marketo Engage juin et août 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}

## Octobre 2022 {#october}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 22 octobre. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 14 octobre 2022**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Veuillez vérifier ci-dessous chaque fonctionnalité pour connaître son statut.

### Environnement de données marketing {#marketing-data-environment}

</br>

* **Synchronisation des champs personnalisés du membre de programme** : possibilité de synchroniser de manière bidirectionnelle les champs extensibles capturés pour un membre de programme (par exemple, les préférences du participant lors de l’enregistrement à l’événement, telles que la nourriture, les sessions, les suivis, etc.) avec les champs de membre de campagne dans Salesforce.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Synchronisation des champs personnalisés des personnes membres du programme</a></td>
  </tr>
  </tbody>
</table>

* **Intégration d’Adobe Privacy Service** : harmonisez-le avec Privacy Service pour automatiser la conformité aux réglementations de confidentialité des données sur les produits Experience Cloud. Actuellement, ce service n’est disponible que pour les clients Marketo Engage qui ont intégré le système Adobe Identity Management.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### Expérience nouvelle génération

</br>

* **Mise à jour de Screens dans l’expérience de nouvelle génération** : nous proposons d’autres écrans actualisés dans l’expérience de nouvelle génération qui offrent une conception et des améliorations de convivialité mises à jour et accessibles via le bouton bascule :

   * Détails du modèle de page de destination
   * Liste de modèles d’e-mail

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">Bouton (bascule)</a></td>
  </tr>
  </tbody>
</table>

* **Amélioration de l’onglet Utilisé par dans les Détails du modèle d’e-mail** : dans la nouvelle expérience, vous verrez des informations supplémentaires relatives aux ressources utilisant le modèle d’e-mail, y compris le statut de la ressource, Dernière modification et Dernière modification par. Vous pouvez également rechercher, trier et filtrer la liste des utilisés par les ressources.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  </tbody>
</table>

* **Modales de filtre des ressources de rapport** : nouvelle conception pour les modèles de configuration de rapport affichant une nouvelle arborescence de ressource dans le menu de configuration et un filtre pour les dates de création et de modification.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  </tbody>
</table>

### Améliorations de l’API {#api-enhancements}

</br>

* **Importation de leads en bloc : association des vendeurs** : parité avec l’API REST de lead pour pouvoir associer des leads aux vendeurs pendant le processus d’importation de leads en bloc, ce qui réduit la complexité et le nombre d’appels d’API requis.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">Importation de leads en bloc</a></td>
  </tr>
  </tbody>
</table>

### Sales Insight {#sales-insight}

</br>

![(étoile)](assets/yellow-star.png)

* **Intégration de Sales Insight à Dynamic Chat** : le tableau de bord Insights comprend désormais les activités Dynamic Chat dans la grille dynamique, ainsi qu’un résumé hebdomadaire et des cartes détaillées.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Intégration de Dynamic Chat</a></td>
  </tr>
  </tbody>
</table>

## Fonctionnalités de mise à jour d’Agile

Les fonctionnalités suivantes suivent un format Agile et sont publiées à différentes dates avant ou après la date de publication standard. Veuillez vérifier ci-dessous chaque fonctionnalité pour connaître son statut.

* **Réorganiser automatiquement les flux de dialogue pour Dynamic Chat** : améliorez votre zone de travail de boîte de dialogue encombrée en organisant tous les éléments de la zone de travail dans un format propre et facile à lire en appuyant sur un bouton via Réorganiser automatiquement.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">Icônes de diffusion Designer</a></td>
  </tr>
  </tbody>
</table>

* **Liens de réunion pour Dynamic Chat** : option permettant d’inclure automatiquement un lien Équipes ou Réunion pour Google et Outlook dans chaque invitation de calendrier envoyée aux visiteurs.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">Calendrier</a></td>
  </tr>
  </tbody>
</table>

* **Prise en charge de types de données supplémentaires pour Dynamic Chat** : trois nouveaux types de données (booléen, entier, flottant) vous permettent d’exploiter davantage de champs Marketo Engage existants dans Dynamic Chat pour des choses telles que le ciblage basé sur les scores ou le fait de poser des questions oui/non aux visiteurs.

<table>
  <tr>
   <td><b>Statut</b></td>
   <td><b>Mises à jour de la documentation</b></td>
  </tr>
  <tr>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  </tbody>
</table>

## Annonces {#announcements}

* **Forms 1.0** : l’obsolescence de Forms 1.0 sera terminée avec la version d’octobre. Les ressources de Forms 1.0 ne pourront plus envoyer de données à Marketo Engage et renverront des erreurs si elles sont tentées.

* **No-Script Forms** : Forms ne fonctionnera plus lorsque JavaScript sera désactivé dans le navigateur. L’envoi du formulaire nécessite l’activation de JavaScript.

