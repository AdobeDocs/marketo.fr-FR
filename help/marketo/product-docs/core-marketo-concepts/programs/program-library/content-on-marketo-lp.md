---
description: Contenu sur Marketo LP - Documents Marketo - Documentation du produit
title: Contenu sur Marketo LP
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 661a41eb0c5c43541a63a36c31837b35f516d827
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 12%

---

# Contenu sur Marketo LP {#content-on-marketo-lp}

Nom du programme : CT-AAAA-MM-Contenu sur Marketo LP

Cet exemple de référence est conçu pour être un programme de contenu qui exploite une page d’entrée Marketo avec un formulaire Marketo utilisant un programme Marketo par défaut. Le formulaire doit accéder au contenu/à l’offre. Le lien vers l’offre peut être affiché sur la page de remerciement, envoyé dans un email de remerciement, ou les deux. Pour obtenir de l’aide sur la stratégie ou personnaliser un programme, contactez l’équipe Compte d’Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) page.

**Résumé du canal**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Canal</th> 
   <th>État d’appartenance</th>
   <th>Comportement d’analyse</th>
   <th>Type de programme</th>
  </tr> 
  <tr> 
   <td>Contenu Web</td> 
   <td>01-Member 
<br/>02-Engaged-Success</td>
   <td>Inclusif</td>
   <td>Par défaut</td>
  </tr>
 </tbody> 
</table>

**Le programme contient les ressources suivantes :**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Type</th> 
   <th>Nom du modèle</th>
   <th>Nom de la ressource</th>
  </tr> 
  <tr> 
   <td>E-mail</td> 
   <td>Modèle de courrier électronique de démarrage rapide</td>
   <td>01-Email-Thank You</td>
  </tr>
  <tr> 
   <td>Page de destination</td> 
   <td>Modèle LP de démarrage rapide</td>
   <td>01 - LP - Enregistrement</td>
  </tr>
  <tr> 
   <td>Page de destination</td> 
   <td>Modèle LP de démarrage rapide</td>
   <td>02 - LP - Merci</td>
  </tr>
  <tr> 
   <td>Formulaire</td> 
   <td> </td>
   <td>Formulaire d’enregistrement de contenu</td>
  </tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Envoyer la performance par e-mail</td>
  </tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Performance page de destination </td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>01 - Formulaire rempli</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>02 - Engagé (succès du programme)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Ressources : héberge toutes les ressources créatives 
<br/>(sous-dossiers pour les emails et les landing pages)  </td>
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

CAPTURE D’ÉCRAN - Image du programme

**Mes jetons incluaient :**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Type de jeton</th> 
   <th>Nom du jeton</th>
   <th>Valeur</th>
  </tr> 
  <tr> 
   <td>Texte complet</td> 
   <td><code>{{my.Content-Description}}</code></td>
   <td>Double-cliquez pour plus de détails  
<br/><code><--My Content Description Here--></code> 
<br/>Modifiez cette description du contenu au niveau du programme, sous l’onglet Mes jetons . 
<br/>Vous allez apprendre : 
<li>Puce 1</li>
<li>Puce 2</li>
<li>Puce 3</li></td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Content-Title}}</code></td>
   <td><code><--My Content Title Here--></code></td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Content-Type}}</code></td>
   <td><code><--My Content Type Here--></code></td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Content-URL}}</code></td>
   <td>my.ContentURL?without=http://</td>
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
   <td><code>{{my. Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL?sans le http://</td>
  </tr>
 </tbody> 
</table>

>[!CAUTION]
>
>Voir Instructions d’importation de programme pour les règles de conflit par défaut.

**Règles de conflit par défaut recommandées pour l’importation :**

* Étiquettes du programme
   * Créer des étiquettes dans cet abonnement (Par défaut) - Recommandé
   * Ignorer

* Modèle de page d’entrée du même nom
   * Copier le modèle original (par défaut)
   * Utiliser le modèle de destination : recommandé

* Des images portant le même nom existent déjà
   * Conserver les deux fichiers (par défaut)
   * Remplacer un élément dans cet abonnement - Recommandé

* Modèles d&#39;email portant le même nom
   * Conserver les deux modèles (par défaut)
   * Remplacer le modèle existant - Recommandé

CAPTURE D’ÉCRAN - Image des règles de conflit par défaut

**Bonnes pratiques recommandées :**

* Les bonnes pratiques de Marketo Consulting recommandent de déplacer le formulaire d’une ressource locale vers une ressource globale située dans Design Studio de Marketo Engage après l’importation du programme de contenu.
   * La réduction du nombre de formulaires et l’utilisation de ressources plus globales à partir de Design Studio vous permettent d’accroître l’évolutivité de la conception de votre programme et de la gouvernance administrative. Il offre également une certaine flexibilité quant aux mises à jour régulières de conformité pour les champs, la langue d’inscription, etc.

* Envisagez de mettre à jour les modèles de votre programme importé afin d’utiliser des modèles de marque actuels ou de mettre à jour le modèle nouvellement importé pour refléter votre marque en ajoutant un fragment de code ou votre logo et vos informations de pied de page appropriés.

* Envisagez de mettre à jour la convention d’affectation des noms de ce modèle de programme pour vous aligner sur votre convention d’affectation des noms, si nécessaire.

* N’oubliez pas de mettre à jour les valeurs Mon jeton sur le modèle de programme et chaque fois que vous utilisez le programme, selon les besoins.

* Pour obtenir de l’aide sur la stratégie ou personnaliser un programme, contactez votre équipe de compte d’Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) page.

>[!TIP]
>
>N’oubliez pas d’activer la campagne &quot;2002-Engaged&quot; pour suivre le succès de la campagne. Procédez comme suit AVANT que votre formulaire ne soit actif et que les courriers électroniques soient envoyés.

>[!NOTE]
>
>Les jetons qui font référence à une URL ne peuvent pas contenir les caractères http:// ou https:// ; dans le cas contraire, le lien ne fonctionnera pas correctement dans la ressource.