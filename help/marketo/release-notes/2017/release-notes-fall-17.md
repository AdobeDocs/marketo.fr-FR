---
unique-page-id: 12983280
description: Notes de mise à jour - Automne 17 - Marketo Docs - Documentation du produit
title: Notes de mise à jour - Automne 17
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 11%

---

# Notes de mise à jour : Automne 17 {#release-notes-fall}

Les fonctionnalités suivantes sont incluses dans la version de l’automne 17. Consultez votre édition Marketo pour connaître la disponibilité des fonctionnalités.

Veuillez cliquer sur les liens de titre vers les articles détaillés de la vue pour chaque fonction. Remarque : Certaines des fonctionnalités incluses dans cette version n’ont pas d’articles associés. Si une rubrique comporte plusieurs sous-titres, les liens y sont placés.

## Fiabilité du système {#system-reliability}

Nous avons apporté d&#39;autres améliorations à l&#39;infrastructure de base de Marketo, y compris un meilleur séquençage, moins d&#39;asymétries et une meilleure stabilité de Munchkin.

## Performance de la synchronisation Sfdc {#sfdc-sync-performance}

Profitez d&#39;une synchronisation plus riche et plus rapide entre Marketo et Salesforce. Les modifications de données qui nécessitent des mises à jour en masse sur les comptes ou les pistes peuvent être fractionnées en files d&#39;attente parallèles pour éviter les retards. Les événements et les tâches se synchronisent désormais également jusqu’à 50 % plus rapidement.

## Améliorations des performances d’analyse {#analytics-performance-improvements}

Améliorations récentes de l’infrastructure L’offre a augmenté le temps de fonctionnement et la stabilité dans le rapports Marketo et les outils d’analyse, ce qui vous permet de créer des rapports ad hoc plus rapidement.

## [Fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Grâce à cette nouvelle fonctionnalité, vous pouvez désormais conserver et diffuser des messages électroniques en fonction des fuseaux horaires locaux. Les programmes de messagerie et d’engagement peuvent être configurés pour être distribués dans les fuseaux horaires des destinataires, ce qui évite la nécessité de créer plusieurs programmes : envoyer une fois et Marketo tiendra automatiquement le courriel jusqu’à l’heure locale appropriée. Effacez les mesures de courriel, observez les pratiques locales et gagnez du temps en utilisant un seul programme globalement.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Si vous ne parvenez pas encore à activer le fuseau horaire Destinataire sur vos programmes de messagerie et d’engagement, ne paniquez pas ! Nous activons progressivement cette fonctionnalité pour tous les clients.

## [Revoyez les exemples d’e-mails par segment](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo dispose d’une nouvelle option pour sélectionner un segment lors de l’envoi d’exemples de messages électroniques à réviser. Il n&#39;est plus nécessaire de déterminer manuellement le segment auquel appartient une piste, ce qui facilite l&#39;envoi de courriers électroniques contenant du contenu dynamique vers différents segments.

## [Questions personnalisées pour la génération de leads LinkedIn](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Personnalisez vos formulaires de génération de leads LinkedIn pour collecter les attributs des leads personnalisés. Vous pouvez désormais poser jusqu’à trois questions personnalisées par formulaire, choisir entre une saisie de texte sur une ligne ou des questions à choix multiples, puis effectuer une mise en correspondance avec les champs de piste Marketo.

## [Intégration Slack](/help/marketo/product-docs/administration/additional-integrations/add-slack-as-a-launchpoint-service.md) {#slack-integration}

Nous avons publié deux fonctionnalités dans le cadre de notre nouvelle intégration Slack :

* Notifications système : Recevez des notifications de Slack concernant les événements importants de votre instance Marketo, tels que des alertes sur les états de la campagne en cours et tout problème nécessitant une attention immédiate.
* Moments intéressants : Lorsqu&#39;un utilisateur connu a déclenché une notification Marketo Insight à partir d&#39;un compte client, les propriétaires de pistes peuvent être avertis par l&#39;intermédiaire d&#39;un Slack. Les notifications incluent des informations de piste ainsi que des détails sur le compte client.

## Améliorations ABM {#abm-enhancements}

**[Afficher les comptes sans contacts](https://docs.marketo.com/x/fKCt)**

Marketo ABM synchronise et affiche désormais les comptes CRM sans contacts. Inclure de nouveaux comptes sans vente ou historique marketing antérieurs et suivre l&#39;avancement en faisant correspondre les prospects suivants aux comptes.

## Analyse ContentAI {#contentai-analytics}

**[Nouveau filtre de liste de compte ABM](https://docs.marketo.com/x/1BPG)**

Vue et comparaison des performances du contenu entre les Listes de compte ABM pour optimiser le contenu existant. ContentAI vous montre :

* contenu le plus consulté
* contenu converti en haut
* Contenu suggéré optimisé par IA pour les activités marketing

## Améliorations de la personnalisation Web {#web-personalization-enhancements}

**[Jetons pour campagnes Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Les jetons peuvent désormais être utilisés dans des campagnes Web. Tirez parti des jetons pour diffuser des messages et du contenu personnalisés afin d’accroître l’engagement dans vos campagnes Web.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Élaborez des images studio dans l’Éditeur de campagnes Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Gagnez du temps en réutilisant les ressources créatives et les images sur plusieurs canaux dans Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Intégration  {#integration}

**[Aperçu d’e-mail API](https://developers.marketo.com/rest-api/assets/emails/)**

Vous pouvez désormais prévisualisation à distance des messages électroniques en dehors de Marketo, ce qui simplifie le processus de localisation du contenu des messages électroniques et réduit les erreurs.

**[Remplacer l’HTML API](https://developers.marketo.com/rest-api/assets/emails/)**

Les développeurs peuvent mettre à jour le contenu HTML des ressources de courrier électronique à distance, ce qui leur permet de travailler dans un système unique pour gérer les ressources.
