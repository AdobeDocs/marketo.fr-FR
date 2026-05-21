---
description: Notes De Mise À Jour - Août 2025 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Août 2025
feature: Release Information
exl-id: f4f71a77-d0c0-41c3-9362-afbfb467cc7a
TQID: https://experienceleague.adobe.com/Tt3KgAUlQd8oBN2KV-dFUQdEPmlZ-3tOzQ8T-EaCTfI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 680
ht-degree: 98%

---

# Notes de mise à jour : août 2025 {#release-notes-aug-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version d’août 2025. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **22 août 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Concepteur d’e-mail - Reporting</strong> : les rapports Performances des e-mails et Performances des liens d’e-mail affichent désormais les données des e-mails créés à l’aide du nouveau Concepteur d’e-mail.</td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Concepteur d’e-mail - Suppression de la saisie semi-automatique</strong> : l’option de saisie semi-automatique de l’éditeur de personnalisation de jeton pointait vers des objets erronés et a été supprimée. Il n’est pas prévu de la mettre à nouveau en œuvre pour le moment.</td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Concepteur d’e-mail - Optimisation de l’aperçu des e-mails</strong> : certains utilisateurs et certaines utilisatrices affichaient des temps de chargement plus lents lors de la tentative d’aperçu de leur e-mail dans la page e-mail/modèle d’e-mail/détails du fragment. Cette expérience a été optimisée pour des temps de chargement jusqu’à 60 % plus rapides.</td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Concepteur d’e-mail - Correctifs de modèles</strong> : certains modèles prêts à l’emploi rencontraient des problèmes de rendu (par exemple, le rendu n’était pas correct sur certains navigateurs/modes sombres, les images n’étaient pas alignées correctement, les boutons CTA étaient déplacés, etc.). Tous ces problèmes ont été corrigés dans cette version.</td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Concepteur d’e-mail - Correctif de verrouillage de contenu</strong> : auparavant, si un modèle d’e-mail était créé avec le verrouillage de contenu et que le modèle était utilisé pour créer un e-mail, le verrouillage de contenu persistait même lorsque l’e-mail était réinitialisé ou que l’option « modifier la conception » était sélectionnée. Ce problème est résolu dans cette version.</td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Fin de vie de Marketo Engage Identity** : en août 2025, Adobe a commencé à supprimer progressivement la prise en charge de Marketo Engage Identity (connexion via `login.marketo.com`). Pour éviter l’interruption de l’accès à Marketo Engage, vous devez passer à [Adobe Identity](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} au plus tard le 30 septembre 2025.

   * _Obsolescence des restrictions d’adresse IP_ : la prise en charge de la [restriction des connexions Marketo en fonction des adresses IP](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} a pris fin le 30 juillet 2025. La fonctionnalité restera opérationnelle jusqu’à la fin de la transition vers Adobe Identity. Une nouvelle fonctionnalité de contrôle d’accès basé sur l’emplacement pour Adobe Identity dans Adobe Admin Console est prévue pour bientôt.

   * _Obsolescence de l’authentification unique (SSO)_ : la prise en charge de [l’authentification unique de Marketo Identity](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} prendra fin le 30 juillet 2025. La fonctionnalité restera opérationnelle jusqu’à la fin de la transition vers Adobe Identity. L’authentification unique pour Adobe Identity dans Adobe Admin Console doit être configurée séparément. Pour connaître les étapes de configuration, consultez [Configurer une identité et l’authentification unique](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

* **Obsolescence de la fonctionnalité _Transférer à un ami_** : le 29 septembre 2025, la fonctionnalité _Transférer à un ami_ des e-mails dans Marketo Engage 2.0 (l’ancien éditeur d’e-mail) sera complètement obsolète pour tous les abonnements. Cela affecte le jeton « Transférer à un ami » et les liens « Transférer à un ami » dans les e-mails qui ont déjà été envoyés ou qui seront envoyés à l’aide du jeton. [En savoir plus](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Obsolescence du paramètre « access_token » de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours de suppression et ne sera plus disponible après le 31 mars 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API SOAP Marketo prendra fin le 31 mars 2026. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
