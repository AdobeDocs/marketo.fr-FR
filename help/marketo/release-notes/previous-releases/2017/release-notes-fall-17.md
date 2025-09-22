---
unique-page-id: 12983280
description: Notes De Mise À Jour - Automne 17 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Automne 17
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 5%

---

# Notes de mise à jour : automne 2017 {#release-notes-fall}

Les fonctionnalités suivantes sont incluses dans la version de l’automne 17. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo.

Cliquez sur les liens de titre pour afficher les articles détaillés de chaque fonctionnalité. Remarque : certaines fonctionnalités incluses dans cette version ne sont pas associées à des articles. Si une rubrique comporte plusieurs sous-titres, les liens y sont placés.

## Fiabilité du système {#system-reliability}

Nous avons apporté d’autres améliorations à l’infrastructure de base de Marketo, notamment un meilleur séquencement, moins d’incohérences et une meilleure stabilité de la [!DNL Munchkin].

## Performance de la synchronisation Sfdc {#sfdc-sync-performance}

Tirez parti d’une synchronisation plus riche et plus rapide sur Marketo et [!DNL Salesforce]. Les modifications de données qui nécessitent des mises à jour en bloc sur les comptes ou les prospects peuvent être divisées en files d’attente parallèles pour éviter les retards. Les événements et les tâches se synchronisent désormais jusqu’à 50 % plus rapidement.

## Améliorations des performances d’analyse {#analytics-performance-improvements}

Les récentes améliorations de l’infrastructure offrent une disponibilité et une stabilité accrues au sein des outils d’analyse et de création de rapports de Marketo, ce qui vous permet de créer des rapports ad hoc plus rapidement.

## [Fuseau horaire du destinataire](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Grâce à cette nouvelle fonctionnalité, vous pouvez désormais conserver et diffuser des e-mails en fonction des fuseaux horaires locaux. Les programmes d’e-mail et d’engagement peuvent être configurés pour être diffusés dans les fuseaux horaires des destinataires, ce qui élimine la nécessité de créer plusieurs programmes ; envoyez une seule fois et Marketo conservera automatiquement l’e-mail jusqu’à l’heure locale appropriée. Élevez les mesures par e-mail, observez les pratiques locales et gagnez du temps en utilisant un seul programme à l’échelle mondiale.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Si vous ne pouvez pas encore activer le fuseau horaire du destinataire sur vos programmes d’e-mail et d’engagement, ne paniquez pas ! Nous activons progressivement cette fonctionnalité pour tous les clients.

## [Consultez les exemples d’e-mails par segment](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo dispose d’une nouvelle option permettant de sélectionner un segment lors de l’envoi d’exemples d’e-mails pour révision. Vous n’avez plus besoin de déterminer manuellement à quel segment appartient un prospect, ce qui facilite l’envoi d’e-mails contenant du contenu dynamique à différents segments.

## [Questions personnalisées de génération de leads LinkedIn](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Personnalisez vos formulaires [!UICONTROL LinkedIn Lead Gen] pour collecter des attributs de prospect personnalisés. Vous pouvez désormais poser jusqu’à trois questions personnalisées par formulaire, choisir entre une saisie de texte sur une seule ligne ou des questions à choix multiples, et faire correspondre aux champs de prospect Marketo.

## Intégration de Slack {#slack-integration}

Nous avons publié deux fonctionnalités dans le cadre de notre nouvelle intégration Slack :

* Notifications système : recevez des notifications Slack concernant les événements importants se produisant dans votre instance Marketo, tels que les alertes sur le statut actuel des campagnes et tout problème nécessitant une attention immédiate.
* Moments intéressants : lorsqu’une Insight Marketo a été déclenchée par un individu connu à partir d’un compte commercial, les propriétaires de leads peuvent être avertis via Slack. Les notifications incluent des informations sur le prospect ainsi que des détails sur le compte de vente.

## Améliorations ABM {#abm-enhancements}

**[Afficher les comptes sans contacts](https://docs.marketo.com/x/fKCt)**

Marketo ABM se synchronise et affiche désormais les comptes CRM sans contact. Incluez de nouveaux comptes sans historique de ventes ou de marketing précédent et suivez la progression en faisant correspondre les prospects suivants aux comptes.

## Analyse ContentAI {#contentai-analytics}

**[Nouveau filtre de liste de comptes ABM](https://docs.marketo.com/x/1BPG)**

Affichez et comparez les performances du contenu dans les listes de comptes AEM pour optimiser le contenu existant. ContentAI vous montre :

* contenu le plus consulté
* contenu le plus converti
* Contenu suggéré optimisé par l’IA pour les activités marketing

## Améliorations de la personnalisation Web {#web-personalization-enhancements}

**[Jetons pour campagnes Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Les jetons peuvent désormais être utilisés dans les campagnes web. Utilisez des jetons pour diffuser des messages et du contenu personnalisés afin d’augmenter l’engagement dans vos campagnes web.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Élaborez des images studio dans l’Éditeur de campagnes Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Gagnez du temps en réutilisant des ressources créatives et des images sur plusieurs canaux dans Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Intégration  {#integration}

**[API de prévisualisation d’e-mail](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)**

Vous pouvez désormais prévisualiser à distance les e-mails en dehors de Marketo, ce qui simplifie le processus de localisation du contenu des e-mails et réduit les erreurs.

**[Remplacer l’API HTML](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)**

Les développeurs peuvent mettre à jour à distance le contenu des ressources d’e-mail d’HTML, ce qui leur permet de travailler dans un seul système pour gérer les ressources.
