---
unique-page-id: 12983280
description: Notes de mise à jour - Automne 17 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Automne 17
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 5%

---

# Notes de mise à jour : automne 17 {#release-notes-fall}

Les fonctionnalités suivantes sont incluses dans la version de l’automne 17. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Marketo.

Cliquez sur les liens de titre pour afficher des articles détaillés pour chaque fonctionnalité. Remarque : Certaines des fonctionnalités incluses dans cette version n’ont pas d’articles associés. Si une rubrique comporte plusieurs sous-titres, les liens y sont placés.

## Fiabilité du système {#system-reliability}

Nous avons apporté d’autres améliorations à l’infrastructure Marketo de base, notamment un meilleur séquencement, moins de discordances et une meilleure stabilité de Munchkin.

## Performance de la synchronisation Sfdc {#sfdc-sync-performance}

Profitez d’une synchronisation plus riche et plus rapide entre Marketo et Salesforce. Les modifications de données qui nécessitent des mises à jour en masse des comptes ou des pistes peuvent être fractionnées en files d’attente parallèles afin d’éviter les retards. Les événements et les tâches se synchronisent désormais 50 % plus rapidement.

## Améliorations des performances d’analyse {#analytics-performance-improvements}

Les récentes améliorations de l’infrastructure offrent une disponibilité et une stabilité accrues dans les outils de reporting et d’analyse de Marketo, ce qui vous permet de créer plus rapidement des rapports ad hoc.

## [Fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Grâce à cette nouvelle fonctionnalité, vous pouvez désormais conserver et envoyer des emails en fonction des fuseaux horaires locaux. Les programmes de messagerie et d’engagement peuvent être configurés pour être diffusés dans les fuseaux horaires des destinataires, éliminant ainsi la nécessité de créer plusieurs programmes : envoyer une fois et Marketo contiendra automatiquement l’email jusqu’à l’heure locale correcte. Effet élévateur des mesures de courrier électronique, observez les pratiques locales et gagnez du temps en utilisant globalement un seul programme.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Si vous ne pouvez pas encore activer le Fuseau horaire du destinataire dans vos programmes d’email et d’engagement, ne paniquez pas ! Cette fonctionnalité est progressivement activée pour tous les clients.

## [Vérification d’exemples d’emails par segment](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo dispose d’une nouvelle option pour sélectionner un segment lors de l’envoi d’exemples d’emails pour révision. Il n’est plus nécessaire de déterminer manuellement le segment auquel appartient une piste, ce qui facilite l’envoi d’emails contenant du contenu dynamique à différents segments.

## [ Questions personnalisées sur le &quot;Lead Gen LinkedIn&quot;](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Personnalisez vos formulaires de génération de pistes LinkedIn pour collecter des attributs de pistes personnalisés. Vous pouvez désormais poser jusqu’à trois questions personnalisées par formulaire, choisir entre une saisie de texte sur une seule ligne ou des questions à choix multiples et revenir aux champs de piste Marketo.

## Intégration de Slack {#slack-integration}

Nous avons publié deux fonctionnalités dans le cadre de notre nouvelle intégration de Slack :

* Notifications système : Recevez des notifications Slack concernant des événements importants dans votre instance Marketo, tels que des alertes concernant les états de la campagne en cours et tout problème nécessitant une attention immédiate.
* Moments intéressants : lorsqu’un insight Marketo a été déclenché par une personne connue à partir d’un compte de vente, les propriétaires de prospect peuvent être avertis via Slack. Les notifications incluent des informations de piste ainsi que des détails sur le compte de vente.

## Améliorations ABM {#abm-enhancements}

**[Afficher les comptes sans contacts](https://docs.marketo.com/x/fKCt)**

Marketo ABM se synchronise désormais et affiche les comptes CRM sans contacts. Incluez de nouveaux comptes sans historique commercial ou commercial antérieur et effectuez le suivi de l’avancement en faisant correspondre les prospects suivants aux comptes.

## Analyse ContentAI {#contentai-analytics}

**[Nouveau filtre de liste de comptes ABM](https://docs.marketo.com/x/1BPG)**

Affichez et comparez les performances du contenu sur les listes de comptes ABM afin d’optimiser le contenu existant. ContentAI vous présente :

* contenu le plus consulté
* contenu converti supérieur
* Contenu suggéré optimisé par l’IA pour les activités marketing

## Améliorations de la personnalisation Web {#web-personalization-enhancements}

**[Jetons pour campagnes Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Les jetons peuvent désormais être utilisés dans les campagnes web. Utilisez les jetons pour diffuser des messages et du contenu personnalisés afin d’augmenter l’engagement dans vos campagnes web.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Élaborez des images studio dans l’Éditeur de campagnes Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Gagnez du temps en réutilisant les ressources créatives et les images sur plusieurs canaux dans Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Intégration  {#integration}

**[&rbrace;API d’aperçu d’email](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/email-scripting)**

Vous pouvez désormais prévisualiser un email à distance en dehors de Marketo, ce qui simplifie le processus de localisation du contenu d&#39;un email et réduit les erreurs.

**[Remplacer l’API HTML](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/email-scripting)**

Les développeurs peuvent mettre à jour à distance le contenu d’HTML des ressources de courrier électronique, ce qui leur permet de travailler sur un seul système pour gérer les ressources.
