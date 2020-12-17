---
unique-page-id: 12983280
description: Notes de mise à jour - Automne 17 - Documents marketing - Documentation du produit
title: Notes de mise à jour - Automne 17
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Notes de mise à jour : Automne 17 {#release-notes-fall}

Les fonctionnalités suivantes sont incluses dans la version de l’automne 17. Vérifiez la disponibilité des fonctionnalités de votre édition Marketing.

Veuillez cliquer sur les liens de titre vers les articles détaillés de la vue pour chaque fonction. Remarque : Certaines des fonctionnalités incluses dans cette version n’ont pas d’articles associés. Si une rubrique comporte plusieurs sous-titres, les liens y sont placés.

## Fiabilité du système {#system-reliability}

Nous avons apporté d&#39;autres améliorations à l&#39;infrastructure de base du marché, notamment un meilleur séquençage, moins d&#39;incohérences et une meilleure stabilité de Munchkin.

## Performances de synchronisation SFDC {#sfdc-sync-performance}

Profitez d&#39;une synchronisation plus riche et plus rapide entre Marketo et Salesforce. Les modifications de données qui nécessitent des mises à jour en masse sur les comptes ou les pistes peuvent être fractionnées en files d&#39;attente parallèles pour éviter les retards. Les événements et les tâches se synchronisent désormais également jusqu’à 50 % plus rapidement.

## Amélioration des performances d’Analytics {#analytics-performance-improvements}

Améliorations récentes de l’infrastructure L’offre a augmenté le temps de fonctionnement et la stabilité dans les outils d’analyse et de rapports de marketing, ce qui vous permet de créer des rapports ad hoc plus rapidement.

## [Fuseau horaire destinataire](https://docs.marketo.com/x/_xvG) {#recipient-time-zone}

Grâce à cette nouvelle fonctionnalité, vous pouvez désormais conserver et diffuser des messages électroniques en fonction des fuseaux horaires locaux. Les programmes de messagerie et d’engagement peuvent être configurés pour être distribués dans les fuseaux horaires des destinataires, ce qui évite de créer plusieurs programmes. Envoyez-les une seule fois et Marketo conservera automatiquement le courriel jusqu’à l’heure locale appropriée. Effacez les mesures de courriel, observez les pratiques locales et gagnez du temps en utilisant un seul programme globalement.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Si vous ne parvenez pas encore à activer le fuseau horaire Destinataire sur vos programmes de messagerie et d’engagement, ne paniquez pas ! Nous activons progressivement cette fonctionnalité pour tous les clients.

## [Examiner les exemples de courrier électronique par segment](https://docs.marketo.com/x/2IER) {#review-sample-emails-by-segment}

Marketo propose une nouvelle option pour sélectionner un segment lors de l’envoi d’exemples de messages électroniques à réviser. Il n&#39;est plus nécessaire de déterminer manuellement le segment auquel appartient une piste, ce qui facilite l&#39;envoi de courriers électroniques contenant du contenu dynamique vers différents segments.

## [Questions personnalisées LinkedIn Lead Gen](https://docs.marketo.com/x/ngLG) {#linkedin-lead-gen-custom-questions}

Personnalisez vos formulaires LinkedIn Lead Gen pour collecter des attributs de piste personnalisés. Vous pouvez désormais poser jusqu’à trois questions personnalisées par formulaire, choisir entre une saisie de texte sur une ligne ou des questions à choix multiples, puis revenir aux champs de piste Marketo.

## [Intégration Slack](../../product-docs/administration/additional-integrations/add-slack-as-a-launchpoint-service.md) {#slack-integration}

Nous avons publié deux fonctionnalités dans le cadre de notre nouvelle intégration Slack :

* Notifications système : Recevez des notifications de Slack concernant les événements importants de votre instance de marketing, tels que des alertes sur les états de la campagne en cours et tout problème nécessitant une attention immédiate.
* Moments intéressants : Lorsqu&#39;une personne connue d&#39;un compte client a déclenché un Insight Marketo, les propriétaires de pistes peuvent être avertis via un Slack. Les notifications incluent des informations de piste ainsi que des détails sur le compte client.

## Améliorations d&#39;ABM {#abm-enhancements}

** [Afficher les comptes sans contacts](https://docs.marketo.com/x/fKCt)**

Marketo ABM se synchronise et affiche désormais des comptes CRM sans contacts. Inclure de nouveaux comptes sans vente ou historique marketing antérieurs et suivre l&#39;avancement en faisant correspondre les prospects suivants aux comptes.

## Contenu`<sup>AI </sup>`Analyses {#contentai-analytics}

** [Nouveau filtre de Liste de compte ABM](https://docs.marketo.com/x/1BPG) **

Vue et comparaison des performances du contenu entre les Listes de compte ABM pour optimiser le contenu existant. Le contenu `<sup>AI</sup>` vous montre :

* contenu le plus consulté
* contenu converti en haut
* Contenu suggéré optimisé par IA pour les activités marketing

## Améliorations de la personnalisation Web {#web-personalization-enhancements}

** [Jetons pour les campagnes Web](https://docs.marketo.com/x/SwJI)**

Les jetons peuvent désormais être utilisés dans des campagnes Web. Tirez parti des jetons pour diffuser des messages et du contenu personnalisés afin d’accroître l’engagement dans vos campagnes Web.

![](assets/image2017-11-16-11-3a25-3a7.png)

** [Création d’images Studio dans Web Campaign Editor](https://docs.marketo.com/x/SwJI)**

Gagnez du temps en réutilisant les fichiers créatifs et les images sur plusieurs canaux dans Marketing.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Intégration {#integration}

** [API de Prévisualisation de courriel](https://developers.marketo.com/rest-api/assets/emails/)**

Vous pouvez désormais prévisualisation à distance des e-mails en dehors de Marketing Cloud, ce qui simplifie le processus de localisation du contenu des e-mails et réduit les erreurs.

** [Remplacer l’API HTML](https://developers.marketo.com/rest-api/assets/emails/)**

Les développeurs peuvent mettre à jour le contenu HTML des ressources de courrier électronique à distance, ce qui leur permet de travailler dans un système unique pour gérer les ressources.
