---
description: Paramètres de l’agent - Documents Marketo - Documentation du produit
title: Paramètres de l’agent
feature: Dynamic Chat
exl-id: a782ef9b-6a89-448a-8bd9-f127ceea3bf5
source-git-commit: 19f7a38a6a87bc66084e7e45f5bf49cd0d29c3cd
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 2%

---

# Paramètres de l’agent {#agent-settings}

Configurez votre calendrier et définissez la disponibilité des réunions/conversations en direct.

>[!PREREQUISITES]
>
>Assurez-vous que vos agents ont reçu les [autorisations](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"} appropriées.

![](assets/agent-settings-1.png)

## Connecter le calendrier {#connect-calendar}

Dans l’onglet de configuration du calendrier, connectez votre calendrier Outlook ou Gmail pour l’utiliser dans la planification des rendez-vous dans le chatbot.

![](assets/agent-settings-2.png)

Une fois que le calendrier d’un utilisateur est connecté à Dynamic Chat, il est ajouté à la file d’attente et les visiteurs du site peuvent prendre rendez-vous sur leur calendrier.

>[!NOTE]
>
>Vous pouvez connecter un calendrier par utilisateur. Si vous souhaitez recevoir des réunions sur plusieurs calendriers, vous devez ajouter plusieurs utilisateurs et leur demander de connecter leurs calendriers.

Les utilisateurs et utilisatrices peuvent également personnaliser le corps de l’invitation envoyée au visiteur ou à la visiteuse lorsqu’ils prennent rendez-vous dans le calendrier de l’utilisateur ou de l’utilisatrice. Il peut également cocher la case en bas pour inclure un lien Google Meeting ou Microsoft Teams (selon le calendrier auquel l&#39;application est connectée).

![](assets/agent-settings-3.png)

>[!TIP]
>
>Utilisez l’icône de jeton (accolades) pour personnaliser les e-mails de confirmation de réservation de réunion à l’aide des attributs de personne ou d’entreprise.

### Autorisations {#permissions}

La configuration d’avec Outlook accorde les autorisations suivantes à Dynamic Chat :

* Accès complet à vos calendriers
* Vous connecter et lire votre profil
* Conserver l’accès aux données auxquelles vous lui avez donné accès
* Lire les paramètres de votre boîte aux lettres

La configuration d’avec Google accorde les autorisations suivantes à Dynamic Chat :

* Créer, modifier ou supprimer des calendriers
* Mettre à jour des événements de calendrier individuels
* Modifier vos paramètres, y compris qui peut voir vos événements
* Modifier la personne avec qui le calendrier est partagé
* Accès à votre nom, adresse e-mail, préférence de langue et image de profil

## Disponibilité pour la réservation de réunion {#meeting-booking-availability}

Définissez votre fuseau horaire et la disponibilité du jour/de la semaine pour recevoir les réservations de réunion.

![](assets/agent-settings-4.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Durée de la réunion</b></td>
   <td>Détermine la durée pendant laquelle les visiteurs verront vos créneaux horaires disponibles.</td>
  </tr> 
  <tr> 
   <td><b>Période tampon entre les réunions</b></td>
   <td>Durée définie comme tampon après la réunion. Si vous la fixez à 30 minutes, personne ne pourra réserver une réunion avec vous jusqu'à 30 minutes après la fin prévue d'une réunion sur votre calendrier.</td>
  </tr>
 </tbody> 
</table>

>[!TIP]
>
>Vous pouvez sélectionner plusieurs blocs de temps le même jour (par exemple, vendredi de 8a à 12p _et_ 1p à 5p) en cliquant sur le signe **+** à droite.

## Disponibilité du chat en direct {#live-chat-availability}

Définissez votre fuseau horaire et la disponibilité du jour/de la semaine pour recevoir des conversations en direct.

![](assets/agent-settings-5.png)

Si vous êtes connecté à l’application, vous recevrez une notification in-app d’une conversation entrante. Si vous n’êtes pas connecté, vous recevrez une notification du navigateur (si vous l’avez [configuré](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}).

>[!IMPORTANT]
>
>Le [bouton de disponibilité](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#availability-toggle){target="_blank"} de la boîte de réception de l’agent **remplacera** ce que vous saisissez dans l’onglet Disponibilité du chat en direct . Ainsi, si vous êtes planifié comme disponible à partir de 1p-5p mais que vous devez faire une pause rapide à 3p, vous n&#39;avez pas besoin de modifier vos paramètres d&#39;agent. Le statut du bouton Disponibilité reste inchangé jusqu’à ce que vous le modifiiez manuellement ou jusqu’à ce que la prochaine période de votre disponibilité soit atteinte.

>[!TIP]
>
>Vous pouvez sélectionner plusieurs blocs de temps le même jour (par exemple, vendredi de 8a à 12p _et_ 1p à 5p) en cliquant sur le signe **+** à droite.

## Photo du profil de l&#39;agent

Un agent peut charger sa propre photo de profil, mais cette action n’est pas effectuée dans Dynamic Chat. Ils devraient accéder à `account.adobe.com/profile`. En savoir plus ici : [Mettre à jour le profil de votre compte](https://helpx.adobe.com/fr/manage-account/using/edit-adobe-account-personal-profile.html).

>[!NOTE]
>
>L’image de profil affichée dans `experience.adobe.com` n’est **pas** prise en charge.
