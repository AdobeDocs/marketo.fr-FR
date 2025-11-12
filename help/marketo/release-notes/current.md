---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 6c362502c975676a635b1425393bf43e1cf0be12
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 99%

---

# Notes de mise à jour : octobre 2025 {#release-notes-oct-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version d’octobre 2025. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **31 octobre 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Concepteur d’e-mail : importateur de modèles (version bêta)</strong> : importez des modèles d’e-mail à partir de l’éditeur d’e-mail classique pour créer des modèles compatibles avec le nouveau concepteur d’e-mail dans Design Studio.</td>
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/import-template.md" target="_blank">Import de modèle</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Concepteur d’e-mail - Thèmes de marque</strong> : vous pouvez désormais définir des thèmes de marque dans Marketo Engage. Les configurations de style peuvent être réutilisées et appliquées aux modèles d’e-mail et aux autres ressources d’e-mail pour garantir la cohérence de la marque.</td>
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brand-themes.md" target="_blank">Thèmes de marque</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Concepteur d’e-mail - Contenu conditionnel</strong> : fonction de parité du nouveau concepteur d’e-mail, qui vous permet de personnaliser les e-mails au-delà de l’utilisation des jetons.</td>
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/conditional-content.md" target="_blank">Contenu conditionnel</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <td><strong>Concepteur d’e-mail - Convertisseur d’images en HTML</strong> : chargez un fichier image PNG/JPEG conforme d’un e-mail et il sera automatiquement converti en HTML pour être utilisé dans le nouveau concepteur d’e-mail.</td>
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/image-to-html.md" target="_blank">Convertir des images en modèles HTML</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Concepteur d’e-mail - Cloner l’action d’e-mail</strong> : vous pouvez désormais cloner un e-mail dans un autre dossier de programme des activités marketing et réutiliser rapidement les e-mails existants.</td>
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Concepteur d’e-mail - Tests A/B</strong> : fonctionnalité de parité du nouveau concepteur d’e-mail, qui vous permet d’effectuer des tests A/B pour déterminer les types de contenu qui reçoivent la meilleure réponse.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Mise à niveau de l’intégration CRM Salesforce** : une nouvelle version de l’intégration CRM native sera déployée sur les sandbox actifs pour lesquels le connecteur natif sera activé au cours des sept prochains jours, à compter du 13 novembre 2025. Retrouvez tous les détails dans [cette publication Nation](https://nation.marketo.com/t5/product-blogs/salesforce-crm-integration-upgrade/ba-p/358702){target="_blank"}.

* **Obsolescence de la double barre oblique de l’API REST** : le 16 septembre 2025, Adobe a effectué une transition vers une infrastructure d’hébergement plus moderne pour les URL d’API REST qui tire parti d’une technologie plus récente et améliore la sécurité et l’évolutivité. Si votre abonnement utilise des API avec une double barre oblique (//) dans l’URL, lisez [cette publication de Nation](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} pour connaître les prochaines étapes.

* **Retour aux scripts Velocity dans le nouveau Concepteur d’e-mail** : Adobe Marketo Engage a lancé en juin dernier une fonctionnalité appelée _Contenu conditionnel_ pour le nouveau concepteur d’e-mail. Cette fonctionnalité a été optimisée par les scripts Handlebar au lieu des scripts Velocity, dans le but d’apporter un peu plus de flexibilité à votre contenu dynamique. Mais lorsque nous avons découvert qu’elle provoquait une résolution incorrecte de certains jetons, nous avons décidé de la désactiver temporairement. [En savoir plus](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179?lang=fr){target="_blank"}

* **Fin de vie de Marketo Engage Identity** : en août 2025, Adobe a commencé à supprimer progressivement la prise en charge de Marketo Engage Identity (connexion via `login.marketo.com`). Pour éviter l’interruption de l’accès à Marketo Engage, vous devez passer à [Adobe Identity](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} au plus tard le 30 septembre 2025.

   * _Obsolescence des restrictions d’adresse IP_ : la prise en charge de la [restriction des connexions Marketo en fonction des adresses IP](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} a pris fin le 30 juillet 2025. La fonctionnalité restera opérationnelle jusqu’à la fin de la transition vers Adobe Identity. Une nouvelle fonctionnalité de contrôle d’accès basé sur l’emplacement pour Adobe Identity dans Adobe Admin Console est prévue pour bientôt.

   * _Obsolescence de l’authentification unique (SSO)_ : la prise en charge de [l’authentification unique de Marketo Identity](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} prendra fin le 30 juillet 2025. La fonctionnalité restera opérationnelle jusqu’à la fin de la transition vers Adobe Identity. L’authentification unique pour Adobe Identity dans Adobe Admin Console doit être configurée séparément. Pour connaître les étapes de configuration, consultez [Configurer une identité et l’authentification unique](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

* **Obsolescence de la fonctionnalité _Transférer à un ami ou une amie_** : le 29 septembre 2025, la fonctionnalité _Transférer à un ami ou une amie_ des e-mails dans Marketo Engage 2.0 (l’ancien éditeur d’e-mails) sera complètement obsolète pour tous les abonnements. Cela affecte le jeton « Transférer à un ami ou une amie » et les liens « Transférer à un ami ou une amie » dans les e-mails qui ont déjà été envoyés ou qui seront envoyés à l’aide du jeton. [En savoir plus](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Obsolescence du paramètre « access_token » de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours de suppression et ne sera plus disponible après le 31 janvier 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API SOAP Marketo prendra fin le 31 janvier 2026. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
