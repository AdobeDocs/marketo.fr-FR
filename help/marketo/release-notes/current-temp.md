---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: dd8604c1eeca1c56441d537b40e08571e96198a7
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 9%

---

# Notes De Mise À Jour : Septembre 2025 {#release-notes-sep-25}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version de septembre 2025. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [sont disponibles ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![étoile](assets/yellow-star.png)) sont des modules complémentaires payants. Contactez votre représentant Marketo Engage pour en savoir plus.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **19 septembre 2025**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication peuvent faire l’objet de modifications. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>TITRE</strong> : Description.</td>
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITRE</strong> : Description.</td>
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITRE</strong> : Description.</td>
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITRE</strong> : Description.</td>
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITRE</strong> : Description.</td>
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITRE</strong> : Description.</td>
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Marketo Engage Identity End of Life** : en août 2025, Adobe a commencé à supprimer progressivement la prise en charge de Marketo Engage Identity (connexion via `login.marketo.com`). Pour éviter l’interruption de l’accès à Marketo Engage, vous devez passer à [Adobe Identity](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} au plus tard le 30 septembre 2025.

   * _Obsolescence des restrictions IP_ : la prise en charge de [Limitation des connexions Marketo en fonction des adresses IP](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} a pris fin le 30 juillet 2025. La fonctionnalité restera opérationnelle jusqu’à la fin de la transition vers Adobe Identity. Une nouvelle fonctionnalité de contrôle d’accès basé sur l’emplacement pour Adobe Identity dans Adobe Admin Console sera bientôt disponible.

   * _Obsolescence de l’authentification unique (SSO)_ : la prise en charge de [l’authentification unique de Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} a pris fin le 30 juillet 2025. La fonctionnalité restera opérationnelle jusqu’à la fin de la transition vers Adobe Identity. L’authentification unique pour l’identité Adobe dans Adobe Admin Console doit être configurée séparément. Pour connaître les étapes de configuration, voir [Configurer une identité et l&#39;authentification SSO](https://helpx.adobe.com/fr/enterprise/using/set-up-identity.html){target="_blank"}.

* **Obsolescence de la fonctionnalité _Transférer à un ami_** : le 29 septembre 2025, la fonctionnalité _Transférer à un ami_ des e-mails Marketo Engage 2.0 (l’ancien éditeur d’e-mail) sera complètement obsolète pour tous les abonnements. Cela affecte les liens « Transférer à un ami » et « Transférer à un ami » dans les e-mails qui ont déjà été envoyés ou qui seront envoyés à l’aide du jeton. [En savoir plus](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 31 octobre 2025. Toutes les intégrations nouvelles et existantes doivent authentifier les appels API REST à l’aide de l’en-tête « Authorization », [comme décrit ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API Marketo SOAP prendra fin le 31 octobre 2025. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
