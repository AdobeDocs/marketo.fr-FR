---
description: Notes De Mise À Jour - Février 2026 - Documents Marketo - Documentation Du Produit
title: Notes De Mise À Jour - Février 2026
feature: Release Information
exl-id: 679d2fca-99ba-4321-ad0d-a297b7f193fc
source-git-commit: 713ab854749cb88a35b24f4355368092cdb35e64
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 22%

---

# Notes De Mise À Jour : Février 2026 {#release-notes-feb-26}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 26 février. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **20 février 2026**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Actions de dossier</strong> : parité avec l’ancien éditeur d’e-mail.
   <ul>
   <li>Partagez et archivez des actions de dossier pour les ressources Designer par e-mail.</li>
   <li>Partagez des dossiers sur des espaces de travail, cliquez avec le bouton droit de la souris sur un dossier pour créer une ressource, puis déplacez des ressources par glisser-déposer.</li>
   </ul>
   </td>
   <td>Libéré</td>
   <td>s/o</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - API</strong> : vous pouvez désormais utiliser des appels d’API pour le Designer d’e-mail.</td>
   <td>Libéré</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/asset#">API Marketo Asset</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - génération d’images de l’assistant AI</strong> : désormais, en plus de Firefly, vous pouvez utiliser des modèles Nano Banana pour générer des images avec l’assistant AI pour le contenu des e-mails.</td>
   <td>Libéré</td>
   <td><a href="https://experienceleague.adobe.com/fr/docs/marketo/using/product-docs/email-marketing/email-designer/ai-assistant#create-content-for-a-specific-section">Créer du contenu pour une section spécifique de votre e-mail</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Obsolescence des fonctionnalités d’optimisation du moteur de recherche** : le mardi 31 mars 2026, Marketo Engage abandonnera la fonctionnalité d’optimisation du moteur de recherche (SEO). Si vous n&#39;utilisez pas activement l&#39;optimisation du moteur de recherche, vous n&#39;avez rien à faire. Si vous avez récemment utilisé l’optimisation du moteur de recherche, vous avez la possibilité d’exporter vos données. [En savoir plus](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617?profile.language=fr){target="_blank"}.

* **Limite de leads de fusion de l’API REST** : à compter du 31 juillet 2026, les appels qui incluent plus de 25 identifiants dans le paramètre leadIds d’un appel de l’API Merge Leads entraîneront un code d’erreur 1080 et l’appel sera ignoré. Les tâches nécessitant la fusion de plus de 25 enregistrements en un seul doivent être divisées en plusieurs tâches pour assurer le succès de ces appels.

* **Obsolescence du paramètre &#39;access_token&#39; de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours d’obsolescence et ne sera plus disponible après le 31 juillet 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API Marketo SOAP prendra fin le 31 juillet 2026. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
