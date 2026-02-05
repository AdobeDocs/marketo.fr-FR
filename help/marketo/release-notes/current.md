---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: d46ce01ca654ce17c1909d9e458cab1a8cb520f9
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 38%

---

# Notes de mise à jour : janvier 2026 {#release-notes-jan-26}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 26 janvier. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Fonctionnalités du cycle de publication de la version standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication de la version standard et commenceront à être publiées le **samedi 30 janvier 2026**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Gérer les marques (version bêta)</strong> : générez le contenu des e-mails en fonction des directives de rédaction de votre organisation/marque.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Amélioration de l’assistant AI</strong> : vous pouvez désormais ajouter directement des ressources de marque dans votre invite et demander au modèle de se référer à cette source pour générer du contenu, plutôt que d’ajouter manuellement une ressource de marque sous forme de fichier.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer d’e-mail - Aperçus visuels des fragments</strong> : tous les fragments publiés s’affichent désormais sous forme de miniatures, ce qui permet d’identifier beaucoup plus rapidement celui dont vous avez besoin.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer d’e-mail - Puces</strong> : vous pouvez désormais créer des puces à plusieurs niveaux lors de la création d’un e-mail dans le Designer d’e-mail.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Améliorations du contenu conditionnel</strong> : parité avec la fonctionnalité <i>Contenu dynamique</i> de l’ancien éditeur d’e-mail.
   <ul>
   <li>Le contenu conditionnel s’applique désormais à la segmentation dans les dossiers partagés.</li>
   <li>Les segmentations sont désormais triées par ordre alphabétique.</li>
   </ul>
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
   <td><strong>Email Designer - Dossiers</strong> : vous pouvez désormais organiser vos ressources créées à l’aide du Designer d’e-mail (e-mails, modèles d’e-mail, fragments) avec des dossiers.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Fonctionnalités de cycle de publication non standard {#non-standard-release-cycle-features}

Les fonctionnalités suivantes ont été publiées en dehors du cycle de publication standard de Marketo Engage.

### Webinaires interactifs {#interactive-webinars}

* **Survey Pod** : une nouvelle capsule Survey permet aux hôtes de concevoir et de diffuser des formulaires de commentaires structurés directement au cours d’une session en direct.

* **capsule Ressources** : la nouvelle capsule Ressources remplace les capsules Fichiers et Liens web précédentes, offrant ainsi un moyen unique et unifié de partager des ressources lors des sessions en direct.

* **Amélioration de l’expérience de l’interface de la salle** : profitez d’une interface de salle actualisée et plus moderne, reposant sur le dernier framework de conception Spectrum 2 d’Adobe, s’alignant sur le langage visuel utilisé dans d’autres produits Adobe tels que Creative Cloud et Experience Cloud.

Consultez [cette page](https://helpx.adobe.com/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"} pour plus de détails.

## Annonces {#announcements}

* **Migration de la communauté Marketo terminée** : la nouvelle communauté Adobe Experience League est maintenant en ligne ! [Plusieurs améliorations](https://experienceleaguecommunities.adobe.com/community-pulse-blog-34/community-update-streamlined-ways-to-engage-and-a-redesigned-homepage-247673){target="_blank"} ont été apportées pour améliorer davantage votre expérience dans la communauté Marketo. [Regarde ça](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-26){target="_blank"}.

* **Obsolescence du paramètre « access_token » de l’API Rest** : le paramètre de requête `access_token` utilisé pour authentifier les appels de l’API REST Marketo est en cours de suppression et ne sera plus disponible après le mercredi 31 mars 2026. Toutes les intégrations nouvelles et existantes doivent authentifier les appels de l’API REST à l’aide de l’en-tête « Autorisation », [comme décrit ici](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Obsolescence de l’API SOAP** : la prise en charge de l’API SOAP Marketo prendra fin le 31 mars 2026. Les services qui utilisent les fonctionnalités de l’API SOAP doivent être migrés vers l’[API REST](https://experienceleague.adobe.com/fr/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
