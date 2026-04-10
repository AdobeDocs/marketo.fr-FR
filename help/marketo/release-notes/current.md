---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: af89a1a1fd0246564d0904103f742230a096de04
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 38%

---

# Notes de mise à jour : mars 2026 {#release-notes-mar-26}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version de mars 2026. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 27 mars 2026**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Gérer les marques (version bêta)</strong> : générez le contenu des e-mails en fonction des directives de rédaction de votre organisation/marque.</td>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/manage-brands.md" target="_blank">Créer et gérer des marques</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Actions rapides</strong> : <i>parité avec l’ancien éditeur d’email</i>. Les actions rapides sont désormais disponibles pour toutes les ressources de Designer par e-mail (e-mails, modèles d’e-mail, fragments). Les actions rapides prises en charge sont les suivantes : Dupliquer, Supprimer, Déplacer, Créer/Modifier le brouillon.
   </td>
   <td>Libéré</i></td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Email Designer - Correctif de rendu Outlook</strong> : cette mise à jour corrige les problèmes de rendu, en particulier dans MS Outlook. Le mode HTML avancé vous permet d’effectuer des modifications HTML/CSS mineures ou d’ajouter des balises de script à votre modèle d’e-mail.
   </td>
   <td>Libéré</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/advanced-html-mode.md" target="_blank">Modification de modèles d’e-mail à l’aide de l’éditeur HTML avancé</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Vérificateur de qualité de marque</strong> : évaluez la qualité générale du contenu pour identifier les problèmes potentiels de lisibilité, de cohésion du contenu et d’efficacité, indépendamment des directives de votre marque.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Gestion des listes de sélection</strong> : vous pouvez désormais spécifier les valeurs qui peuvent être utilisées dans les champs de Marketo Engage.
   </td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Notifications push</strong> : les URL de redirection configurées dans les messages de notification push prennent désormais en charge les jetons Marketo Engage (applicable uniquement aux <i>URL de l’application Launch</i>).
   </td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Obsolescence des fonctionnalités d’optimisation du moteur de recherche** : le mardi 31 mars 2026, Marketo Engage abandonnera la fonctionnalité d’optimisation du moteur de recherche (SEO). Si vous n&#39;utilisez pas activement l&#39;optimisation du moteur de recherche, vous n&#39;avez rien à faire. Si vous avez récemment utilisé l’optimisation du moteur de recherche, vous avez la possibilité d’exporter vos données. [En savoir plus](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}.

* **Limite de leads de fusion de l’API REST** : à compter du 31 mars 2026, les appels qui incluent plus de 25 identifiants dans le paramètre leadIds d’un appel de l’API Merge Leads entraîneront un code d’erreur 1080 et l’appel sera ignoré. Les tâches nécessitant la fusion de plus de 25 enregistrements en un seul doivent être divisées en plusieurs tâches pour assurer le succès de ces appels.

* **Obsolescence du paramètre « access_token » de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours de suppression et ne sera plus disponible après le samedi 31 juillet 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API SOAP Marketo prendra fin le samedi 31 juillet 2026. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
