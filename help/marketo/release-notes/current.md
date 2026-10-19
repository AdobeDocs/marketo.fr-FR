---
description: Notes de mise à jour actuelles - Documentation Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: 'https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 29aa413a7346a79906f4021dedc79e8e48170c69
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 15%
---
# Notes De Mise À Jour : Octobre 2026 {#release-notes-oct-26}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 26 octobre. Vérifiez la disponibilité des fonctionnalités dans votre édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques à Adobe Dynamic Chat [peuvent être consultées ici](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes font partie du cycle de publication standard et commenceront à être publiées le **23 octobre 2026**, avec un déploiement échelonné des fonctionnalités restantes au cours des semaines suivantes. Les fonctionnalités et dates de publication sont susceptibles d’être modifiées. Vérifiez le statut en regard de chaque fonctionnalité.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Fonctionnalité</th>
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
  <tr>
   <td><strong>Compétences en matière de planification de campagnes</strong> : CX Enterprise Coworker for Marketo Engage peut désormais transformer un résumé de campagne en un document de configuration de programme Marketo Engage complet. Le document comprend la structure des dossiers, les campagnes intelligentes, les configurations d’e-mail, les jetons et une liste de contrôle d’assurance qualité. Cela permet aux équipes de lancer des campagnes plus rapidement et de normaliser la configuration du programme. La compétence peut être configurée via Markdown.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Agents appelables</strong> : créez des agents d’IA qui s’exécutent en tant qu’étape de flux dans vos campagnes intelligentes et qui agissent sur un enregistrement de prospect en fonction des instructions que vous écrivez en langage clair. Par exemple, un agent peut normaliser les données d’un prospect ou signaler des robots probables, puis réécrire le résultat dans les champs du prospect. Le traitement des prospects est ainsi basé sur le jugement et s’effectue dans vos campagnes sans code personnalisé.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Cloner vers ce programme/dossier</strong> : les opérations de clonage dans Marketo Engage offrent désormais de manière cohérente une option « Ce dossier » ou « Ce programme » comme premier choix lors du choix de la destination de la ressource clonée. La sélection de cette option clone la ressource dans le programme parent ou le dossier de la ressource active.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <tr>
   <td><strong>Alerte instantanée sur la synchronisation CRM </strong> : l’activation ou la désactivation de la synchronisation CRM native pour un environnement déclenche désormais une notification aux utilisateurs et utilisatrices abonnés au canal de notification CRM.</td>
   <td><i>Bientôt disponible</i></td>
   <td><i>Bientôt disponible</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Annonces {#announcements}

* **Obsolescence des images capturées sur le web** : pour se conformer aux bonnes pratiques modernes en matière de sécurité et de confidentialité, la fonctionnalité [Capturer des images sur le web](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"} sera abandonnée à compter de la version d’octobre.

* **Restrictions de nom d’API pour les attributs d’activité personnalisés** : les noms d’API pour les attributs d’activité personnalisés créés via l’API ou l’interface utilisateur peuvent désormais uniquement contenir des caractères alphanumériques et des traits de soulignement et doivent commencer par un caractère alphanumérique.

* **Limites de taille de liste statique pour les activités Get Lead et Get Lead Changes** : depuis le 30 septembre 2026, les appels aux points d’entrée Get Lead Activities ou Get Lead Changes qui incluent le paramètre `listId` ont commencé à échouer avec un code d’erreur 1003 (indiquant que la liste statique cible contient trop d’enregistrements) si les listes cibles contiennent 10 000 leads ou plus. Consultez le [ Guide de migration ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} pour plus d’informations.
