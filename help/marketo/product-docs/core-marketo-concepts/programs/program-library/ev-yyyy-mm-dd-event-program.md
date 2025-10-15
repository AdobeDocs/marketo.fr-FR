---
description: Programme d’événement EV-YYYY-MM-DD - Documents Marketo - Documentation du produit
title: EV-AAAA-MM-JJ-Programme d’événement
feature: Programs
exl-id: 999a82ae-6637-40bf-96c0-62183cb0a197
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 22%

---

# EV-AAAA-MM-JJ-Programme d’événement {#ev-yyyy-mm-dd-event-program}

Voici un exemple de programme d’événement avec une page d’inscription, trois e-mails d’invitation et des e-mails de relance utilisant un programme d’événement Marketo Engage. Convient à tous les événements où vous avez besoin d&#39;inscriptions, y compris les tournées, les déjeuners, les dîners ou les présentations lors d&#39;événements de salon.

Pour obtenir de l’aide sur la stratégie ou la personnalisation d’un programme, contactez l’équipe du compte Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/fr/customers/consulting-services/main.html){target="_blank"}.

## Résumé du canal {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Canal</th>
   <th>Statut d’abonnement</th>
   <th>Comportement d'analyse</th>
   <th>Type de programme</th>
  </tr>
  <tr>
   <td>Événement</td>
   <td>01-Invité
<br/>02-Waitlisted
<br/>03-Registered
<br/>04-Pas d'affichage
<br/>05-Attended-Success</td>
   <td>Inclusif</td>
   <td>Événement</td>
  </tr>
 </tbody>
</table>

## Le programme contient les Assets suivantes {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Type</th>
   <th>Nom du modèle</th>
   <th>Nom de la ressource</th>
  </tr>
  <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle d’e-mail pour un démarrage rapide</a></td>
   <td>01-E-Mail-Merci</td>
  </tr>
   <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle d’e-mail pour un démarrage rapide</a></td>
   <td>02a- Email - Invitation</td>
  </tr>
  <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle d’e-mail pour un démarrage rapide</a></td>
   <td>02b - E-mail - Rappel d’invitation</td>
  </tr>
  <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle d’e-mail pour un démarrage rapide</a></td>
   <td>02c- Email - Rappel d'invitation Dernière chance</td>
  </tr>
  <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle d’e-mail pour un démarrage rapide</a></td>
   <td>03 - E-mail - Rappel de participation</td>
  </tr>
  <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle d’e-mail pour un démarrage rapide</a></td>
   <td>04a - E-mail - Suivi - Terminé</td>
  </tr>
  <tr>
   <td>E-mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modèle d’e-mail pour un démarrage rapide</a></td>
   <td>04b - Email - Suivi - NoShow</td>
  </tr>
  <tr>
   <td>Page de destination</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Modèle de programme de démarrage rapide</a></td>
   <td>01a - LP - Inscription</td>
  </tr>
  <tr>
   <td>Page de destination</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Modèle de programme de démarrage rapide</a></td>
   <td>01b - LP - Merci</td>
  </tr>
  <tr>
   <td>Form</td>
   <td> </td>
   <td>Enregistrement des événements FM</td>
  </tr>
  <tr>
   <td>Rapport local</td>
   <td> </td>
   <td>Performance des e-mails</td>
  </tr>
  <tr>
   <td>Rapport local</td>
   <td> </td>
   <td>Performance de la page de destination</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>00 - Programme d'acquisition des captures</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>01 - Procéder à l'enregistrement</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>02a - Envoyer l'invitation</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>02b - Envoyer un rappel d'invitation</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>02c - Envoyer l'invitation de la dernière chance</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>03 - Envoyer un rappel pour participer</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>04 - Participant (Succès du programme)</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>05 - Envoyer des e-mails de relance</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Assets - Contient toutes les ressources créatives
<br/>(sous-dossiers pour les e-mails et les landing pages)</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Campagnes - Abrite toutes les campagnes intelligentes</td>
  </tr>
  <tr>
   <td>Dossier</td>
   <td> </td>
   <td>Rapports</td>
  </tr>
 </tbody>
</table>

![](assets/ev-yyyy-mm-dd-event-program-1.png)

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
   <td>Double-Clic pour plus de détails</td>
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
   <td><code>{{my.Content-Description}}</code></td>
   <td>Double-cliquer pour plus de détails
<br/><code><--My Content Description Here--></code>
<br/>Modifiez cette description de contenu au niveau du programme, sous l’onglet Mes jetons .
<br/>Vous apprendrez :
<li>Puce 1</li>
<li>Puce 2</li>
<li>Puce 3</li></td>
  </tr>
  <tr>
   <td>Texte</td>
   <td><code>{{my.Event-Location-Line1}}</code></td>
   <td><code><--XYZ Hotel--></code></td>
  </tr>
   <tr>
   <td>Texte</td>
   <td><code>{{my.Event-Location-Line2}}</code></td>
   <td><code><--ABC Room--></code></td>
  </tr>
   <tr>
   <td>Texte</td>
   <td><code>{{my.Event-Location-Line3}}</code></td>
   <td><code><--1234 Anystreet--></code></td>
  </tr>
  <tr>
   <td>Texte</td>
   <td><code>{{my.Event-Location-Line4}}</code></td>
   <td><code><--Anytown, ZZ 99999--></code></td>
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
   <td>Évènement en direct</td>
  </tr>
  <tr>
   <td>Texte</td>
   <td><code>{{my.PageURL-Download}}</code></td>
   <td>my.DownloadURL?without=http://</td>
  </tr>
  <tr>
   <td>Texte</td>
   <td><code>{{my.PageURL-Registration}}</code></td>
   <td>my.RegistrationPageURL?without=http://</td>
  </tr>
  <tr>
   <td>Texte</td>
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>my.ThankYouPageURL?without=http://</td>
  </tr>
  <tr>
   <td>Texte</td>
   <td><code>{{my.Speaker1-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
  <tr>
   <td>Texte</td>
   <td><code>{{my.Speaker1-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
  </tr>
  <tr>
   <td>Texte</td>
   <td><code>{{my.Speaker2-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
  <tr>
   <td>Texte</td>
   <td><code>{{my.Speaker2-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
  </tr>
  <tr>
   <td>Texte</td>
   <td><code>{{my.Speaker3-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
 <tr>
   <td>Texte</td>
   <td><code>{{my.Speaker3-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
  </tr>
 </tbody>
</table>

## Règles de conflit {#conflict-rules}

* **Balises de programme**
   * Créer des balises dans cet abonnement - _Recommandé_
   * Ignorer

* **Modèle de page de destination portant le même nom**
   * Copier le modèle d&#39;origine
   * Utiliser le modèle de destination - _Recommandé_

* **Images du même nom**
   * Conserver les deux fichiers
   * Remplacer l&#39;élément dans cet abonnement - _Recommandé_

* **Modèles d’e-mail portant le même nom**
   * Conserver les deux modèles
   * Remplacer le modèle existant - _Recommandé_

## Meilleures pratiques {#best-practices}

* Après l’importation du programme de webinaire, déplacez le formulaire d’une ressource locale vers une ressource globale située dans Design Studio.
   * Réduire le nombre de formulaires et utiliser davantage de ressources globales à partir de Design Studio permet une plus grande évolutivité dans la conception de vos programmes et la gouvernance administrative. Il offre également une certaine flexibilité dans les mises à jour de conformité régulières pour les champs, la langue d’accord préalable, etc.

* Envisagez de mettre à jour les modèles de votre programme importé afin d’utiliser les modèles de la marque actuelle, ou mettez à jour le nouveau modèle importé pour refléter votre marque en ajoutant un fragment de code ou les informations de logo/pied de page appropriées.

* Envisagez de mettre à jour la convention de nommage de cet exemple de programme pour l’aligner sur votre convention de nommage.

>[!NOTE]
>
>N’oubliez pas de mettre à jour mes valeurs de jeton dans le modèle de programme et chaque fois que vous utilisez le programme, si nécessaire.

>[!TIP]
>
>N’oubliez pas d’activer la campagne « 06-Attended (Program Success) » pour assurer le suivi du succès ! Effectuez cette opération _avant_ votre formulaire est en ligne et des e-mails sont envoyés.

>[!IMPORTANT]
>
>Mes jetons qui font référence à une URL ne peuvent pas contenir les adresses http:// ou https://. Autrement, le lien ne fonctionnera pas correctement dans la ressource.
