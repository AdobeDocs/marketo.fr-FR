---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 8101d9c73571948847d00dfc21f21c39bcd1d975
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 6%

---

# Notes De Mise À Jour : Août 2025 {#release-notes-aug-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 25 août. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [sont disponibles ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **22 août 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication peuvent faire l’objet de modifications. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Reporting</strong> : les rapports Performances des emails et Performances des liens d'email affichent désormais les données des emails créés à l'aide du nouveau Designer d'email.</td>
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Optimisation de l’aperçu des e-mails</strong> : certains utilisateurs affichaient des temps de chargement plus lents lors de la tentative de prévisualisation de leur e-mail dans la page e-mail/modèle d’e-mail/détails du fragment. Cette expérience a été optimisée pour des temps de chargement jusqu’à 60 % plus rapides.</td>
   <td><i>Disponible bientôt</i></td>
   <td>S.O.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer d’e-mail - Correctifs de modèles</strong> : certains modèles prêts à l’emploi rencontraient des problèmes de rendu (par exemple, le rendu n’était pas correct sur certains navigateurs/modes sombres, les images n’étaient pas alignées correctement, les boutons CTA étaient déplacés, etc.). Tous ces problèmes ont été corrigés dans cette version.</td>
   <td><i>Disponible bientôt</i></td>
   <td>S.O.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Correctif de verrouillage de contenu</strong> : auparavant, si un modèle d’e-mail était créé avec le verrouillage de contenu et que le modèle était utilisé pour créer un e-mail, le verrouillage de contenu persistait même lorsque l’e-mail était réinitialisé ou que l’option « modifier la conception » était sélectionnée. Ce problème est résolu dans cette version.</td>
   <td><i>Disponible bientôt</i></td>
   <td>S.O.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Suppression de la saisie semi-automatique</strong> : l’option de saisie semi-automatique de l’éditeur de personnalisation de jeton pointait vers des objets erronés et a été supprimée. Il n’est pas prévu de le mettre à nouveau en œuvre pour le moment.</td>
   <td>Expédié</td>
   <td>S.O.</td>
  </tr>
 </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Marketo Engage Identity End of Life** : en août 2025, Adobe a commencé à supprimer progressivement la prise en charge de Marketo Engage Identity (connexion via `login.marketo.com`). Pour éviter l’interruption de l’accès à Marketo Engage, vous devez passer à [Adobe Identity](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} au plus tard le 30 septembre 2025.

   * _Obsolescence des restrictions IP_ : la prise en charge de [Limitation des connexions Marketo en fonction des adresses IP](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} a pris fin le 30 juillet 2025. La fonctionnalité restera opérationnelle jusqu’à la fin de la transition vers Adobe Identity. Une nouvelle fonctionnalité de contrôle d’accès basé sur l’emplacement pour Adobe Identity dans Adobe Admin Console sera bientôt disponible.

   * _Obsolescence de l’authentification unique (SSO)_ : la prise en charge de [l’authentification unique de Marketo](https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} a pris fin le 30 juillet 2025. La fonctionnalité restera opérationnelle jusqu’à la fin de la transition vers Adobe Identity. L’authentification unique pour l’identité Adobe dans Adobe Admin Console doit être configurée séparément. Pour connaître les étapes de configuration, voir [Configurer une identité et l&#39;authentification SSO](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 31 octobre 2025. Toutes les intégrations nouvelles et existantes doivent authentifier les appels API REST à l’aide de l’en-tête « Authorization », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API Marketo SOAP prendra fin le 31 octobre 2025. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
