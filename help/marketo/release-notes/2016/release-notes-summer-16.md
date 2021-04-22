---
unique-page-id: 11380218
description: Notes de mise à jour - Été 16 - Marketo Docs - Documentation du produit
title: Notes de mise à jour - Été 16
exl-id: 3843668e-c729-42aa-b05c-55c33ee0d783
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 4%

---

# Notes de mise à jour : Été 16 {#release-notes-summer}

Les fonctionnalités suivantes sont incluses dans la version de Summer &#39;16. Consultez votre édition Marketo pour connaître la disponibilité des fonctionnalités. Veuillez cliquer sur les liens de titre vers les articles détaillés de la vue pour chaque fonction.

## [Account Based Marketing](https://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

Le marketing basé sur les comptes Marketo fournit tous les éléments essentiels dans une seule plate-forme unifiée :

* **Cible**  - Détection de compte, mise en correspondance de pistes vers comptes et Listes de comptes nommés
* **Interagir**  - Personnalisation basée sur le compte, engagement entre canaux et Workflows spécifiques au compte
* **Mesure**  - Statistiques au niveau du compte et de la Liste, note d’engagement du compte, impact sur le pipeline et les recettes

![](assets/abm-5-acme.png)

>[!NOTE]
>
>ABM est disponible en tant que complément à votre abonnement Marketo. Contactez votre représentant commercial pour l&#39;implémenter.

## [Journal d’audit](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md) {#audit-trail}

La piste d’audit fournit un historique complet des modifications apportées à votre abonnement Marketo. Il créera des responsabilités parmi les utilisateurs et les administrateurs, aidera à identifier la cause d&#39;un comportement inattendu, et assurera la sécurité de savoir qui fait quoi et quand. Ces renseignements seront disponibles à tout moment et pourront être utilisés pour répondre à des questions telles que :

* Qu’est-il advenu de cet actif ou paramètre et qui l’a mis à jour en dernier ?
* Qu&#39;est-ce que l&#39;utilisateur X a fait ?
* Qui se connecte à notre compte ?

![](assets/audit-trail.png)

## [Intégration Marketo-Vibes SMS LaunchPoint](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) {#marketo-vibes-sms-launchpoint-integration}

Créez facilement des SMS directement à Marketo. Personnalisez et cible votre message à l&#39;aide de vos données Marketo riches et surveillez facilement ses performances à l&#39;aide du tableau de bord de messages SMS.

>[!NOTE]
>
>Cette fonctionnalité nécessite que vous disposiez d’un compte SMS Vibes existant.

![](assets/vibes-sms2.png)

## [Améliorations des e-mails 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**Variables au niveau du module**

Auparavant, toutes les variables spécifiées dans les modèles Email 2.0 étaient &quot;globales&quot; dans la portée. Lorsque vous utilisez des variables dans des modules, cela n’est pas toujours souhaitable si vous prévoyez d’utiliser plusieurs instances du module. Dans cette version, les variables peuvent désormais être spécifiées au niveau du module, ce qui vous permet d’indiquer que l’utilisateur doit être en mesure de définir des valeurs uniques pour chaque module dans lequel il est utilisé.

![](assets/module-level-variables.png)

**Mises à jour de la syntaxe**

* Vous pouvez désormais utiliser &quot;mktoAddByDefault&quot; sur les modules spécifiés dans les modèles d’e-mail 2.0 afin d’indiquer quels modules doivent être affichés par défaut dans les nouveaux e-mails. Cela est beaucoup plus pratique si vous créez un modèle de courrier électronique avec un grand nombre de modules.
* Sur les éléments d’image, vous pouvez désormais spécifier si les propriétés &quot;hauteur&quot; et &quot;largeur&quot; de l’élément HTML sous-jacent `<img>` doivent être verrouillées ou modifiables pour l’utilisateur final. mktoLockImgSize=&quot;true&quot; entraîne le verrouillage de la hauteur/largeur (même si l’image est modifiée). De même, mktoLockImgStyle=&quot;true&quot; entraînera le verrouillage de la propriété &quot;style&quot;.

**Recherche de code**

Utilisez la nouvelle fonctionnalité de recherche pour rechercher et remplacer efficacement du contenu dans le code de votre courriel. Cette fonctionnalité est également disponible dans l’éditeur Modèle de courriel.

![](assets/2nd-screenshot.png)

**Prise en charge des jetons dans les éléments d’image**

Les jetons peuvent désormais être utilisés dans la zone &quot;URL externe&quot; de l’expérience d’insertion d’image ! Si vous avez spécifié des images avec `{{my.tokens}}`, vous pouvez maintenant référencer ces jetons dans l’éditeur de messagerie 2.0. Notez que l’image apparaîtra toujours rompue dans le canevas de l’éditeur de messagerie 2.0. Mais vous verrez qu’ils sont rendus dans Prévisualisation et Envoyer un exemple avant d’envoyer votre courriel.

## Plusieurs noms de domaine {#multiple-branding-domains}

L&#39;époque où les liens de tracking email ne pouvaient être marqués qu&#39;avec un seul domaine de marque est révolue. Vous pouvez maintenant ajouter plusieurs domaines de marque pour inspirer la confiance des consommateurs, créer une apparence plus rationnelle pour vous concentrer sur la marque, améliorer la délivrabilité des courriels et choisir, par courriel, le domaine de marque à utiliser pour les liens de suivi de chaque courrier électronique.

![](assets/multiple-branding-domains.png)

## [Jetons de programme](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

Nous avons créé un nouveau type de jeton pour les programmes. Vous pouvez désormais afficher le nom, la description et l’identifiant du Programme dans les ressources et les étapes de flux de campagne dynamique.

![](assets/program-tokens.png)

## [Clé d’entreprise](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Demander à chaque membre de votre équipe commerciale d&#39;installer notre module externe Sales Insight for Outlook peut être fastidieux. Nous avons introduit une nouvelle méthode d&#39;installation du module externe pour Outlook à distance à l&#39;aide d&#39;une clé d&#39;entreprise. Envoyez à votre équipe informatique votre clé unique trouvée dans la section Marketo Sales Insight de l&#39;administrateur et laissez-la s&#39;occuper du reste.

![](assets/enterprise-key.png)

## [Campagnes de personnalisation Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

Indiquez une temporisation de réaction des campagnes Web sur votre site Web.

![](assets/dialog-campaign-delay.png)

## [Analyse de contenu et exportation Recommendations](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

Afficher les données des analyses et recommandations de contenu hors ligne.

## [Prise en charge par l’API d’Email Editor 2.0](https://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

Les API d’actifs préexistantes, auparavant uniquement compatibles avec les modèles et courriers électroniques v1.0, sont désormais activées pour les ressources de courrier électronique v2.0.

## [Site des développeurs Marketo](https://developers.marketo.com/) {#marketo-developers-site}

Nouveau et amélioré !

## [Paramètres de confidentialité](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

Les spécialistes du marketing peuvent utiliser les paramètres de confidentialité pour décider s’il convient ou non de suivre les visiteurs à l’aide des fonctions Munchkin et Personnalisation Web. Le niveau de suivi est contrôlé en utilisant le paramètre Ne pas suivre du navigateur, un cookie d’exclusion ou une adresse IP non spécifique. Ces méthodes peuvent affecter la valeur et la fonctionnalité de Marketo dans des zones spécifiques, mais si le spécialiste du marketing ne change rien, la fonctionnalité de Marketo reste la même.

Cette fonctionnalité sera mise à la disposition des clients progressivement sur une période de six semaines. Si vous en avez besoin tout de suite, veuillez contacter l&#39;assistance technique de Marketo.
