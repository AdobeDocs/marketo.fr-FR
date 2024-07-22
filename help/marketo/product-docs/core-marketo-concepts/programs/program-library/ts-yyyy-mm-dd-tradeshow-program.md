---
description: TS-YYYY-MM-DD-Tradeshow Program - Marketo Docs - Documentation du produit
title: Programme TS-YYYY-MM-DD-Tradeshow
feature: Programs
exl-id: 39ef8d6e-392b-456e-a925-b1f6c2cb81d8
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 15%

---

# Programme TS-YYYY-MM-DD-Tradeshow {#ts-yyyy-mm-dd-tradeshow-program}

Il s’agit d’un exemple de programme de commerce avec des emails d’invitation et de suivi utilisant un programme d’événement de Marketo Engage.

Pour obtenir de l’aide sur la stratégie ou personnaliser un programme, contactez l’équipe chargée du compte Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} .

## Résumé du canal {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Canal</th> 
   <th>État d’appartenance</th>
   <th>Comportement d'analyse</th>
   <th>Type de programme</th>
  </tr> 
  <tr> 
   <td>Événement</td> 
   <td>01-Invité 
   <br/>02-Waitlisted
   <br/>03-Registered
   <br/>04-Visited Booth
   <br/>05-Engagés à l’émission - Succès
   <br/>06-Engagé à la publication - Réussite</td>
   <td>Inclusif</td>
   <td>Événement</td>
  </tr>
 </tbody> 
</table>

## Le programme contient l’Assets suivante {#program-contains-the-following-assets}

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
   <td>01-Email-Thank You</td>
  </tr>
   <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle de courrier électronique de démarrage rapide</a></td>
   <td>02a- Email - Invitation</td>
  </tr>
  <tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Performance des e-mails</td>
  </tr>
  <tr> 
   <td>Rapport local</td> 
   <td> </td>
   <td>Performance du programme</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>00 - Programme d’acquisition de capture</td>
  </tr>
  <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>01 - Envoyer une invitation</td>
  </tr>
   <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>02 - Envoi d’emails de relance</td>
  </tr>
   <tr> 
   <td>Campagne intelligente</td> 
   <td> </td>
   <td>03 - Engagé par un message de relance (succès)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Assets : héberge toutes les ressources créatives 
<br/> (sous-dossiers pour les pages d’entrée et de messagerie)</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Campagnes : héberge toutes les campagnes dynamiques.</td>
  </tr>
  <tr> 
   <td>Dossier</td> 
   <td> </td>
   <td>Rapports</td>
  </tr>
 </tbody> 
</table>

![](assets/ts-yyyy-mm-dd-tradeshow-program-1.png)

## Mes jetons inclus {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Type de jeton</th> 
   <th>Nom du jeton</th>
   <th>Valeur</th>
  </tr>
  <tr> 
   <td>Fichier du calendrier</td> 
   <td><code>{{my.AddToCalendar}}</code></td>
   <td>Double-cliquer pour plus de détails</td>
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
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
   <tr> 
   <td>Texte complet</td> 
   <td><code>{{my.Event-Booth#}}</code></td>
   <td><code><--My Booth Number--></code></td>
  </tr>
   <tr> 
   <td>Texte</td> 
   <td><code>{{my.Event-City}}</code></td>
   <td><code><--My Event City Here--></code></td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Event-Time}}</code></td>
   <td><code><--My Event Time + TimeZone--></code></td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Event-Title}}</code></td>
   <td><code><--My Event Title Here--></code></td>
  </tr>
  <tr> 
   <td>Texte</td> 
   <td><code>{{my.Event-Type}}</code></td>
   <td>Salon professionnel</td>
  </tr>
 </tbody> 
</table>

## Règles de conflit {#conflict-rules}

* **Balises de programme**
   * Créer des balises dans cet abonnement - _Recommandé_
   * Ignorer

* **Modèle de page d’entrée avec le même nom**
   * Copier le modèle d&#39;origine
   * Utiliser le modèle de destination - _Recommandé_

* **Images du même nom**
   * Conserver les deux fichiers
   * Remplacer un élément de cet abonnement - _Recommandé_

* **Modèles d&#39;email portant le même nom**
   * Conserver les deux modèles
   * Remplacer le modèle existant - _Recommandé_

## Meilleures pratiques {#best-practices}

* Après l’importation du programme de webinaire, déplacez le formulaire d’une ressource locale vers une ressource globale située dans Design Studio.
   * La réduction du nombre de formulaires et l’utilisation de ressources plus globales à partir de Design Studio vous permettent d’accroître l’évolutivité de la conception de votre programme et de la gouvernance administrative. Il offre également une certaine flexibilité quant aux mises à jour régulières de conformité pour les champs, la langue d’inscription, etc.

* Envisagez de mettre à jour les modèles de votre programme importé afin d’utiliser les modèles de marque actuels ou de mettre à jour le modèle nouvellement importé pour refléter votre marque en ajoutant un fragment de code ou vos informations de logo/pied de page appropriées.

* Envisagez de mettre à jour la convention d’affectation des noms de cet exemple de programme pour vous aligner sur votre convention d’affectation des noms.

>[!NOTE]
>
>Pensez à mettre à jour les valeurs de mon jeton dans le modèle de programme et chaque fois que vous utilisez le programme, selon les besoins.

>[!TIP]
>
>N’oubliez pas d’activer la campagne &quot;03 - Engagé par un message électronique de relance (succès du programme)&quot; pour le suivi de la réussite. Effectuez cette _avant_ l&#39;envoi de vos emails.

>[!IMPORTANT]
>
>Les jetons qui font référence à une URL ne peuvent pas contenir les caractères http:// ou https:// ; dans le cas contraire, le lien ne fonctionnera pas correctement dans la ressource.
