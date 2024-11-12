---
description: Notes de mise à jour actuelles - Documents Marketo - Documentation du produit
title: Notes de mise à jour actuelles
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 236c99d8939f076d93dfcd7988fc89e4c617c113
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 5%

---

# Notes de mise à jour : octobre 2024 {#release-notes-oct-24}

Vous trouverez ci-dessous toutes les fonctionnalités incluses dans la version du 24 octobre. Vérifiez la disponibilité de vos fonctionnalités dans l’édition Adobe Marketo Engage.

Les notes de mise à jour spécifiques au Adobe Dynamic Chat [ se trouvent ici ](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Les fonctionnalités signalées par une étoile (![star](assets/yellow-star.png)) sont des modules complémentaires payants. Pour en savoir plus, contactez votre représentant Marketo Engage.

## Fonctionnalités du cycle de publication standard {#standard-release-cycle-features}

Les fonctionnalités suivantes entrent dans le cycle de publication standard et commenceront à être publiées le **4 octobre 2024**, avec un déploiement progressif des fonctionnalités restantes au cours des semaines suivantes. Les fonctions et dates de publication peuvent faire l’objet de modifications. Vérifiez l’état de chaque fonction en regard de celle-ci.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Fonctionnalité</th> 
   <th style="width:10%">Statut</th>
   <th style="width:25%">Documentation</th>
  </tr>
    <tr> 
   <td><strong>Tableau de bord des données d’enregistrement améliorées dans l’engagement pour les webinaires interactifs</strong> : Vous pouvez désormais voir quelles entreprises ont eu le plus de fréquentation et obtenir que l’entreprise, le titre et le secteur soient mis à jour au niveau de l’avance dans les rapports disponibles dans le tableau de bord de l’engagement.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
    <tr> 
   <td><strong>Tokenization for Interactive Webinars</strong> : vous pouvez désormais utiliser des jetons pour promouvoir des webinaires interactifs dans des emails et des landing pages sans avoir à ajouter manuellement les détails du webinaire.</td> 
   <td><i>Disponible bientôt</i></td>
   <td><i>Disponible bientôt</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>Liste dynamique "Définir pour affecter" : nombre</strong> : voir le nombre de personnes qui seront affectées lors de la modification des règles de qualification d’une campagne dynamique.</td> 
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>Bouton Mon compte dans le rail de navigation</strong> : pour ceux qui ont migré vers Adobe Identity Management System, un nouveau bouton "Mon compte" dans le rail de navigation de gauche permet de configurer votre fuseau horaire et d’accéder aux détails de l’abonnement.</td> 
   <td>Expédié</td>
   <td>s/o</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   <tr> 
   <td><strong>Améliorations des rapports de performances des emails</strong> : plusieurs améliorations ont été apportées aux mesures de création de rapports par email et au suivi des activités, offrant des informations supplémentaires et améliorant la précision.
   <ul>
   <li>Filtrage des personnes supprimées et fusionnées à partir des mesures de performances des emails</li>
   <li>Les emails sont désormais classés comme <i>avorté</i> après trois jours d’attente d’activité de réponse.</li>
   <li>Les ouvertures d’email sont comptabilisées comme ouvertes uniques séparément pour chaque campagne dynamique</li>
   </td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">Rapport des performances des e-mails</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   <tr> 
   <td><strong>Mesures de journal de synchronisation de Salesforce</strong> : surveillez les tendances de débit de synchronisation et de journal de la synchronisation afin de planifier et de planifier des mises à jour CRM pour une expérience de synchronisation optimale.
   </td> 
   <td>Expédié</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Mesures de journal de synchronisation Salesforce</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annonces {#announcements}

* **Dépréciation du paramètre access_token de l’API Rest** : le paramètre de requête &#39;access_token&#39; utilisé pour authentifier les appels de l’API REST Marketo est en cours d’abandon et ne sera plus disponible après le 30 juin 2025. Toutes les intégrations nouvelles et existantes doivent authentifier les appels API REST à l’aide de l’en-tête &#39;Authorization&#39; [, comme décrit ici](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication#using-an-access-token).


* **Dépréciation du code QR** : le 4 octobre 2024, la fonctionnalité de code QR utilisée dans les notifications push et les ressources de messagerie in-app sera obsolète. Cela inclut l’utilisation de codes QR pour un nouvel appareil de test, ainsi que la création de nouvelles ressources avec des codes QR. Les fonctionnalités obsolètes avec une utilisation plus faible nous permettent de réaffecter leurs ressources à la maintenance globale de Marketo Engage.

* **Modifications Munchkin**

   * **Nouvelle version** : le 17 septembre 2024, [Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 commencera à se déployer vers les instances de Marketo Engage pour lesquelles le paramètre &quot;Munchkin Beta&quot; est activé dans **Admin** > **Treasure Chest**. Il est prévu qu’il démarre le déploiement sur toutes les autres instances le 29 octobre. Cette version met à jour la création des cookies Munchkin. Les fonctionnalités ne sont pas modifiées.

   * **Caractères de l’URL supprimés** : les activités &quot;Page web des visites&quot; et &quot;Lien des clics&quot; créées par Munchkin JS vont désormais supprimer les caractères de contrôle non encodés par URL de tous les champs d’URL. Cette modification est conçue pour empêcher les erreurs liées à la propagation de ces types de caractères dans des systèmes qui ne les prennent pas en charge et qui n’ont pas d’utilisation valide dans Marketo Engage.
