---
unique-page-id: 11380218
description: Notes De Mise À Jour -Été '16 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Été 2016
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '774'
ht-degree: 4%

---

# Notes de mise à jour : été 2016 {#release-notes-summer}

Les fonctionnalités suivantes sont incluses dans la version d’été 16. Vérifiez la disponibilité des fonctionnalités dans votre édition Marketo. Cliquez sur les liens de titre pour afficher les articles détaillés de chaque fonctionnalité.

## [Account Based Marketing](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Le marketing basé sur les comptes Marketo fournit tous les éléments essentiels dans une seule plateforme unifiée :

* **Target** - Découverte de compte, correspondance entre les prospects et les comptes et listes de comptes nommés
* **Engage** - Personalization basé sur les comptes, engagement cross-canal et workflows spécifiques aux comptes
* **Mesure** - Informations au niveau du compte et de la liste, score de l’engagement du compte et impact sur le pipeline et le chiffre d’affaires

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM est disponible sous la forme d’un module complémentaire pour votre abonnement Marketo. Vous devez donc contacter votre représentant commercial pour qu’il l’implémente.

## [Journal d’audit](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

Le journal d&#39;audit fournit un historique complet des modifications apportées à votre abonnement Marketo. Il créera une responsabilisation parmi les utilisateurs et les administrateurs, aidera à identifier la cause du comportement inattendu et fournira la sécurité de savoir qui fait quoi et quand. Ces informations seront disponibles à tout moment et pourront être utilisées pour répondre à des questions telles que :

* Qu’est-il advenu de cette ressource ou de ce paramètre et qui l’a mis à jour pour la dernière fois ?
* Qu&#39;a fait l&#39;utilisateur X ?
* Qui se connecte à notre compte ?

![](assets/audit-trail.png)

## Intégration Marketo-Vibes SMS LaunchPoint

Créez facilement des SMS directement dans Marketo. Personnalisez et ciblez votre message à l’aide de vos données Marketo enrichies et surveillez facilement ses performances à l’aide du tableau de bord des messages SMS.

>[!NOTE]
>
>Cette fonctionnalité nécessite que vous disposiez d’un compte [!DNL Vibes SMS] existant.

![](assets/vibes-sms2.png)

## [Améliorations des e-mails 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**Variables au niveau du module**

Auparavant, toutes les variables spécifiées dans les modèles d’e-mail 2.0 avaient une portée « globale ». Lorsque vous utilisez des variables dans des modules, cela n’est pas toujours souhaitable si vous prévoyez d’utiliser plusieurs instances du module. Avec cette version, les variables peuvent désormais être spécifiées comme « niveau du module », ce qui vous permet d’indiquer que l’utilisateur doit être en mesure de définir des valeurs uniques pour chaque module dans lequel elles sont utilisées.

![](assets/module-level-variables.png)

**Mises à jour de la syntaxe**

* Vous pouvez désormais utiliser « mktoAddByDefault » sur les modules spécifiés dans les modèles d’e-mail 2.0 afin d’indiquer quels modules doivent être affichés par défaut dans les nouveaux e-mails. Cela s’avère beaucoup plus pratique si vous créez un modèle d’e-mail avec un grand nombre de modules.
* Sur les éléments d’image, vous pouvez maintenant spécifier si les propriétés « height » et « width » de l’élément d’HTML `<img>` sous-jacent doivent être verrouillées ou modifiables par l’utilisateur final. mktoLockImgSize=« true » entraîne le verrouillage de la hauteur/largeur (même si l’image est modifiée). De même, mktoLockImgStyle=« true » entraîne le verrouillage de la propriété « style ».

**Recherche de code**

Utilisez la nouvelle fonctionnalité de recherche pour rechercher et remplacer efficacement le contenu dans le code de votre e-mail. Cette fonctionnalité est également disponible dans l’éditeur de modèles d’e-mail.

![](assets/2nd-screenshot.png)

**Prise en charge des jetons dans les éléments d’image**

Les jetons peuvent désormais être utilisés dans la zone « URL externe » de l’expérience d’insertion d’images. Si vous avez spécifié des images avec `{{my.tokens}}`, vous pouvez désormais référencer ces jetons dans l’éditeur d’e-mail 2.0. Notez que l’image apparaîtra toujours endommagée dans la zone de travail de l’éditeur d’e-mail 2.0. Cependant, vous les verrez rendues dans Aperçu et Envoyer un exemple avant d’envoyer votre e-mail.

## Plusieurs noms de domaine {#multiple-branding-domains}

Nous sommes loin de l&#39;époque où les liens de tracking e-mail ne pouvaient être marqués qu&#39;avec un seul domaine de marque. Vous pouvez désormais ajouter plusieurs domaines de marque pour inspirer confiance aux consommateurs, créer une apparence plus rationalisée pour vous concentrer sur la marque, améliorer la délivrabilité des e-mails et choisir, par e-mail, le domaine de marque à utiliser pour les liens de suivi de chaque e-mail.

![](assets/multiple-branding-domains.png)

## [Jetons de programme](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

Nous avons créé un nouveau type de jeton pour les programmes. Vous pouvez désormais effectuer le rendu du nom, de la description et de l’identifiant du programme dans les étapes de ressources et de flux de campagne intelligent.

![](assets/program-tokens.png)

## [Clé d’entreprise](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Exiger que chaque personne de votre équipe de vente installe notre plug-in [!DNL Sales Insight] pour [!DNL Outlook] peut être fastidieux. Nous avons introduit une nouvelle méthode pour installer le plug-in pour [!DNL Outlook] à distance à l’aide d’une clé d’entreprise. Envoyez à votre équipe informatique la clé unique qui se trouve dans la section [!DNL Sales Insight] de Marketo de [!UICONTROL Admin] et laissez-la faire le reste.

![](assets/enterprise-key.png)

## [Campagnes de personnalisation Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

Spécifiez un délai pour que les campagnes web réagissent sur votre site web.

![](assets/dialog-campaign-delay.png)

## [Exportation de Content Analytics et Recommendations](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

Affichez les données d’analyse de contenu et de recommandations hors ligne.

## [Prise en charge par l’API d’Email Editor 2.0](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

Les API de ressources préexistantes, auparavant uniquement compatibles avec les e-mails et les modèles v1.0, sont désormais activées pour les ressources de messagerie v2.0.

## [Site des développeurs Marketo](https://developers.marketo.com/) {#marketo-developers-site}

Nouveau et amélioré !

## [Paramètres de confidentialité](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

Les marketeurs peuvent utiliser les paramètres de confidentialité pour décider d’effectuer ou non le suivi des visiteurs à l’aide des fonctionnalités de [!DNL Munchkin] et de Web Personalization. Le niveau de suivi est contrôlé à l’aide du paramètre Ne pas suivre du navigateur, d’un cookie d’exclusion ou d’une adresse IP non spécifique. Ces méthodes peuvent avoir une incidence sur la valeur et la fonctionnalité de Marketo dans des zones spécifiques, mais si le marketeur ne modifie rien, la fonctionnalité de Marketo reste la même.

Cette fonctionnalité sera progressivement disponible pour les clients sur une période de six semaines. Si vous en avez besoin immédiatement, contactez l’assistance Marketo.
