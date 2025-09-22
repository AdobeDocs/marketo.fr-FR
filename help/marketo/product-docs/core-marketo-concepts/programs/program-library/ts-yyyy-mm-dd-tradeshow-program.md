---
description: Programme de salon TS-YYYY-MM-DD - Documentation Marketo - Documentation du produit
title: TS-AAAA-MM-JJ-Programme de salon professionnel
feature: Programs
exl-id: 39ef8d6e-392b-456e-a925-b1f6c2cb81d8
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 18%

---

# TS-AAAA-MM-JJ-Programme de salon professionnel {#ts-yyyy-mm-dd-tradeshow-program}

Voici un exemple de programme de salon professionnel avec des invitations et des e-mails de suivi utilisant un programme d’événement Marketo Engage.

Pour obtenir de l’aide sur la stratégie ou la personnalisation d’un programme, contactez l’équipe du compte Adobe ou rendez-vous sur la page [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}.

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
   Stand <br/>04-Visité
   <br/>05-Engaged at Show - Success
   <br/>06-Engaged at Post Show - Success</td>
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
   <td>00 - Programme d'acquisition des captures</td>
  </tr>
  <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>01 - Envoyer l'invitation</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>02 - Envoyer des e-mails de relance</td>
  </tr>
   <tr>
   <td>Campagne intelligente</td>
   <td> </td>
   <td>03 - Engagement par e-mail de suivi (succès)</td>
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
>N’oubliez pas d’activer la campagne « 03 - Engagement par e-mail de suivi (succès du programme) » pour le suivi du succès ! Effectuez cette opération _avant_ l’envoi de vos e-mails.

>[!IMPORTANT]
>
>Mes jetons qui font référence à une URL ne peuvent pas contenir les adresses http:// ou https://. Autrement, le lien ne fonctionnera pas correctement dans la ressource.
