---
description: NL-AAAA-MM-Newsletter - Documents Marketo - Documentation du produit
title: NL-AAAA-MM-Newsletter
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 9c9046d6ac889bef4ec8ab7add82fda8e72d73b4
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 19%

---

# NL-AAAA-MM-Newsletter {#nl-yyyy-mm-newsletter}

Cet exemple envoie un email de newsletter à l’aide d’un programme de messagerie de Marketo Engage. Le courrier électronique peut inclure ou non un test A/B.

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
   <td>Bulletin d’information</td> 
   <td>01-Member 
<br/>02-Engaged-Success</td>
   <td>Inclusif</td>
   <td>E-mail</td>
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
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle de courrier électronique de démarrage rapide</a></td>
   <td>01 - Email</td>
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
   <td>01 - Engagé (succès du programme)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Ressources : héberge toutes les ressources créatives 
<br/>(sous-dossiers pour les emails)  </td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Campagnes : héberge toutes les campagnes dynamiques.</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Rapports  </td>
  </tr>
 </tbody> 
</table>

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

CAPTURE D’ÉCRAN DU PROGRAMME

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

CAPTURE D&#39;ÉCRAN DES RÈGLES DE CONFLIT

## Meilleures pratiques {#best-practices}

* Envisagez de mettre à jour les modèles de votre programme importé afin d’utiliser les modèles de marque actuels ou de mettre à jour le modèle nouvellement importé pour refléter votre marque en ajoutant un fragment de code ou vos informations de logo/pied de page appropriées.

* Envisagez de mettre à jour la convention d’affectation des noms de cet exemple de programme pour vous aligner sur votre convention d’affectation des noms.

>[!NOTE]
>
>Pensez à mettre à jour les valeurs de mon jeton dans le modèle de programme et chaque fois que vous utilisez le programme, selon les besoins.

>[!TIP]
>
>N’oubliez pas d’activer la campagne &quot;01-Engaged&quot; (engagement 01) pour suivre le succès de la campagne. Procédez comme suit : _before_ votre formulaire est actif et des courriers électroniques sont envoyés.