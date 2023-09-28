---
description: NUR-YYYY-MM-Advanced Nurture - Marketo Docs - Documentation produit
title: NUR-YYYY-MM-Advanced Nurture
feature: Programs
exl-id: cd266cad-843b-4329-ad40-2f3d0acd4948
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 15%

---

# NUR-YYYY-MM-Advanced Nurture {#nur-yyyy-mm-advanced-nurture}

Il s’agit d’un exemple de programme de formation continue avancé qui utilise le Programme d’engagement des Marketo Engage. Les programmes de messagerie imbriqués empêchent les personnes de recevoir du contenu qu’elles ont déjà consommé ou de contrôler le type de contenu qu’elles doivent consommer dans chaque flux. Les rapports d’attribution peuvent être exécutés pour chaque programme de messagerie imbriqué. Canaux : &quot;Nourrir&quot; et un canal dédié &quot;Nourrir un courriel&quot; pour les programmes de messagerie imbriqués envoie un courriel de newsletter à l’aide d’un programme de messagerie du Marketo Engage. Le courrier électronique peut inclure ou non un test A/B.

Pour obtenir de l’aide sur la stratégie ou personnaliser un programme, contactez l’équipe Compte d’Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} page.

## Résumé du canal {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Canal</th> 
   <th>État d’appartenance</th>
   <th>Comportement d’analyse</th>
   <th>Type de programme</th>
  </tr> 
  <tr> 
   <td>Nurture</td> 
   <td>01 - Membre 
<br/>02 - Engagé - Succès</td>
   <td>Inclusif</td>
   <td>Engagement</td>
  </tr>
  <tr> 
   <td>E-mail de fidélisation</td> 
   <td>01 - Ignorer 
<br/>02 - Envoyé
<br/>03 - Engagé - Succès</td>
   <td>Inclusif</td>
   <td>Par défaut</td>
  </tr>
 </tbody> 
</table>

## Le programme contient les ressources suivantes {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Type</th> 
   <th>Nom du modèle</th>
   <th>Nom de la ressource</th>
  </tr> 
   <tr> 
   <td>Programme imbriqué</td> 
   <td> </td>
   <td>01 - Rubrique X</td>
  </tr>
  <tr> 
   <td>Programme imbriqué</td> 
   <td> </td>
   <td>02 - Rubrique Y</td>
  </tr>
  <tr> 
   <td>Programme imbriqué</td> 
   <td> </td>
   <td>03 - Rubrique Z</td>
  </tr>
  <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle de courrier électronique de démarrage rapide</a></td>
   <td>01 - Courrier électronique (en direct dans les programmes imbriqués)</td>
  </tr>
   <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle de courrier électronique de démarrage rapide</a></td>
   <td>02 - Courrier électronique (en direct dans les programmes imbriqués)</td>
  </tr>
   <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle de courrier électronique de démarrage rapide</a></td>
   <td>03 - Courrier électronique (en direct dans les programmes imbriqués)</td>
  </tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Envoyer la performance par e-mail</td>
  </tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Envoyer la performance lien par e-mail</td>
  </tr>
  <tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>01 - Ajouter à l’éducation</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>02 - Infirmière en pause</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>03 - Reprise de la formation</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>04 - Engagé (succès du programme)</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>00 - Ignorer le courrier électronique (situé dans chaque programme imbriqué)</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>01 - Envoyer un courrier électronique (situé dans chaque programme imbriqué)</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>02 - Réussite engagée (située dans chaque programme imbriqué)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Ressources (contiennent les dossiers de ressources et de programmes imbriqués et résident également dans les programmes imbriqués pour contenir les courriers électroniques)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Programmes imbriqués (vies sous le dossier Assets)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Campagnes : toutes les maisons des campagnes intelligentes du programme de prise en charge parent et les dossiers des campagnes se trouvent également dans chaque programme imbriqué.</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Rapports  </td>
  </tr>
 </tbody> 
</table>

![](assets/nur-yyyy-mm-advanced-nurture-1.png)

## Mes jetons inclus {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Type de jeton</th> 
   <th>Nom du jeton</th>
   <th>Valeur</th>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Email-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Email-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
 </tbody> 
</table>

## Règles de conflit {#conflict-rules}

* **Étiquettes du programme**
   * Créer des balises dans cet abonnement - _Recommandé_
   * Ignorer

* **Modèle de page d’entrée du même nom**
   * Copier le modèle d’origine
   * Utiliser le modèle de destination - _Recommandé_

* **Images du même nom**
   * Conserver les deux fichiers
   * Remplacer l’élément de cet abonnement - _Recommandé_

* **Modèles d&#39;email portant le même nom**
   * Conserver les deux modèles
   * Remplacer le modèle existant - _Recommandé_

## Meilleures pratiques {#best-practices}

* Envisagez de mettre à jour les modèles de votre programme importé afin d’utiliser les modèles de marque actuels ou de mettre à jour le modèle nouvellement importé pour refléter votre marque en ajoutant un fragment de code ou vos informations de logo/pied de page appropriées.

* Envisagez de mettre à jour la convention d’affectation des noms de cet exemple de programme pour vous aligner sur votre convention d’affectation des noms.

* Assurez-vous que des règles sont en place pour mettre en pause et reprendre votre cadence de formation. Ces campagnes dynamiques doivent être activées ou planifiées avant l’activation du programme d’engagement.

>[!NOTE]
>
>Pensez à mettre à jour les valeurs de mon jeton dans le modèle de programme et chaque fois que vous utilisez le programme, selon les besoins.

>[!TIP]
>
>N’oubliez pas d’activer la campagne &quot;04 - Engaged (Program Success)&quot; pour le suivi du succès. Procédez comme suit : _before_ vos emails sont envoyés.
