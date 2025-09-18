---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 9189d45829a23a3b9eb75fc4125db92c3508773d
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 41%

---

# Notes de mise à jour : septembre 2025 {#release-notes-sep-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version de septembre 2025. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant ou représentante Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 19 septembre 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Conservation des activités de webinaire à la demande</strong> : les utilisateurs de webinaires interactifs disposent désormais de données de tableau de bord de webinaires à la demande disponibles depuis plus de 30 jours (auparavant, elles ne pouvaient pas être consultées avant 30 jours).</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Workflow Content Collaboration</strong> : vous pouvez désormais commenter les autres utilisateurs de Marketo et collaborer avec eux dans une ressource d’e-mail. Identifiez les membres de l’équipe (les utilisateurs de Marketo qui disposent des autorisations de ressources appropriées) et ils recevront une notification Push ou par e-mail.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Autorisations de l’assistant AI</strong> : les administrateurs Marketo peuvent fournir à des utilisateurs spécifiques un accès aux fonctionnalités de GenAI.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Mode sombre</strong> : vous pouvez désormais utiliser le mode sombre, qui permet aux clients de messagerie et aux applications de gestion d’afficher les e-mails avec des arrière-plans plus sombres et des couleurs plus claires pour le texte, les boutons et d’autres éléments de l’interface utilisateur.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Correctifs de redirection</strong> : certains utilisateurs rencontraient des problèmes de redirection avec les URL pour les e-mails créés à l’aide du nouveau Designer (par exemple, le collage direct des URL ou le signet de ressources d’e-mail ne fonctionnait pas toujours). Ce problème a été résolu. En outre, les liens vers des ressources d’e-mail provenant de <b>Modèles d’e-mail</b> &gt; <b>Détails</b> &gt; <b>Utilisé par</b> redirigeront vers la ressource d’e-mail correspondante.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Retour aux scripts Velocity dans le nouveau Designer d’e-mail** : Adobe Marketo Engage a lancé en juin dernier une fonctionnalité appelée _Contenu conditionnel_ pour le nouveau Designer d’e-mail. Cette fonctionnalité était optimisée par le script Handlebar au lieu du script Velocity, dans le but de fournir un peu plus de flexibilité dans votre contenu dynamique. Mais lorsque nous avons découvert qu’il provoquait une résolution incorrecte de certains jetons, nous avons décidé de le désactiver temporairement. [En savoir plus](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Marketo Engage Identity End of Life** : en août 2025, Adobe a commencé à supprimer progressivement la prise en charge de Marketo Engage Identity (connexion via `login.marketo.com`). Pour éviter l’interruption de l’accès à Marketo Engage, vous devez passer à [Adobe Identity](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} au plus tard le 30 septembre 2025.

   * _Obsolescence des restrictions IP_ : la prise en charge de [Limitation des connexions Marketo en fonction des adresses IP](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} a pris fin le 30 juillet 2025. La fonctionnalité restera opérationnelle jusqu’à la fin de la transition vers Adobe Identity. Une nouvelle fonctionnalité de contrôle d’accès basé sur l’emplacement pour Adobe Identity dans Adobe Admin Console sera bientôt disponible.

   * _Obsolescence de l’authentification unique (SSO)_ : la prise en charge de [l’authentification unique de Marketo](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} a pris fin le 30 juillet 2025. La fonctionnalité restera opérationnelle jusqu’à la fin de la transition vers Adobe Identity. L’authentification unique pour Adobe Identity dans Adobe Admin Console doit être configurée séparément. Pour connaître les étapes de configuration, consultez [Configurer une identité et l’authentification unique](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

* **Obsolescence de la fonctionnalité _Transférer à un ami_** : le 29 septembre 2025, la fonctionnalité _Transférer à un ami_ des e-mails Marketo Engage 2.0 (l’ancien éditeur d’e-mail) sera complètement obsolète pour tous les abonnements. Cela affecte les liens « Transférer à un ami » et « Transférer à un ami » dans les e-mails qui ont déjà été envoyés ou qui seront envoyés à l’aide du jeton. [En savoir plus](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Obsolescence du paramètre « access_token » de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours de suppression et ne sera plus disponible après le 31 octobre 2025. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API SOAP Marketo prendra fin le 31 octobre 2025. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
