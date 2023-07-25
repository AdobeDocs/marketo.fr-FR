---
unique-page-id: 2949839
description: Archivage des personnes dans votre événement à partir de votre tablette - Documents Marketo - Documentation du produit
title: Archivage des personnes dans votre événement à partir de votre tablette
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Archivage des personnes dans votre événement à partir de votre tablette {#check-people-into-your-event-from-your-tablet}

Lorsque des personnes se présentent à votre événement, vous pouvez trouver leurs informations dans l’application. Après l’archivage, ils sont promus au statut Participant lorsque vous vous synchronisez avec Marketo.

L’application fonctionne de la même manière sur iPad et Android, à l’exception des différences mineures de mise en page et de conception.

>[!PREREQUISITES]
>
>* Créez un événement dans Marketo et renseignez-le avec des personnes invitées et enregistrées.
>* Téléchargez l’application pour tablette [Android](https://play.google.com/store/apps/details?id=com.marketo.eventcheckin&amp;hl=en) ou [iOS](https://itunes.apple.com/us/app/marketo-events/id522766637?mt=8)

## Archivage des invités enregistrés {#check-in-registered-guests}

1. Appuyez sur l’icône de l’application sur votre tablette iPad ou Android.

1. Appuyer **Connexion** pour lancer l’application Marketo Event.

   ![](assets/1.jpg)

1. Saisissez votre nom d’utilisateur et votre mot de passe Marketo, puis cliquez sur **Connexion**.

   >[!NOTE]
   >
   >Vous devez disposer d’un rôle avec accès à la base de données pour voir les personnes dans l’application.

1. Sélectionnez une **Événement**.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >Seuls les programmes d’événement (à l’exception des webinaires) planifiés une semaine avant et une semaine après la date d’aujourd’hui s’affichent.

1. Sur l’écran Accueil , recherchez les invités enregistrés . Pour trouver une personne dans la liste, vous pouvez :

   * Faire défiler pour trouver un nom
   * Saisissez un nom dans le champ de recherche.
   * Accédez à une lettre initiale spécifique du nom en appuyant sur celle-ci sur le côté droit de la liste.

   >[!NOTE]
   >
   >Le processus est le même sur iPad et Android, mais les écrans diffèrent et les éléments peuvent se trouver à des emplacements différents. Cet article présente l’interface d’iPad. Comparez l’écran Android de cette section à titre de référence.

   **iPad**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **Android**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. Appuyez sur le nom sélectionné, puis, sur l’enregistrement de la personne, appuyez sur **Archivage**.

   ![](assets/img-0068-35-hands.png)

L’invité dispose désormais du statut Participant et reçoit une coche. L’enregistrement de personne est mis à jour lors de la synchronisation avec Marketo. Le compteur rouge sur le bouton Synchroniser s’incrémente pour afficher le nombre d’enregistrements depuis la dernière synchronisation avec Marketo. Le bouton Synchroniser a un aspect différent et se trouve à un autre emplacement pour iPad et Android :

**iPad**

![](assets/image2016-4-12-14-3a25-3a13.png)

**Android**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>Si une personne est invitée mais ne s’est pas inscrite, vous pouvez rechercher le nom en cliquant sur **Recherche sur le serveur**, juste en dessous de la zone de recherche. L’état Invité passe à **Attaché** pour l’événement .

## Création d’une personne sur la tablette {#create-a-new-person-on-the-tablet}

Vous pouvez ajouter manuellement des invités qui ne sont pas des personnes existantes dans votre base de données Marketo. Ils seront automatiquement archivés et ajoutés à votre base de données lors de la synchronisation avec Marketo.

1. Cliquez sur **Ajouter**.

   **iPad**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **Android**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. Renseignez autant de champs d’informations de base que possible et appuyez sur **Terminé**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >Vous ne pouvez utiliser que les champs existants. Vous ne pouvez pas en créer des personnalisés.

   >[!CAUTION]
   >
   >Vérifiez deux fois l&#39;adresse email. D&#39;autres champs peuvent être corrigés ultérieurement, mais l&#39;adresse email est la méthode Principale pour contacter l&#39;invité.

La nouvelle personne est enregistrée comme archivée dans votre événement et sera ajoutée à la base de données Marketo avec le statut Participant lors de la synchronisation avec Marketo.

## Reverse d’une archivage {#reverse-a-check-in}

Si vous vous êtes inscrit par erreur dans une personne, _avant la synchronisation avec Marketo_, vous pouvez inverser l’état Participant .

1. Appuyez sur le nom dans la liste, puis, dans l’enregistrement de la personne, appuyez sur . **Annuler**.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   Tout est réparé !

## Modification d’un enregistrement de personne lors de l’archivage {#edit-a-person-record-at-check-in}

Vous pouvez ajouter et modifier des informations sur les invités, directement à l’événement !

1. Appuyez sur le nom dans la liste des personnes, puis appuyez sur **Modifier**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. Modifiez et ajoutez des informations aux champs, puis appuyez sur **Terminé**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >Sous Android, la variable **Terminé** peut être masqué. Faites défiler l’écran vers le bas pour le trouver.

Les informations sont mises à jour lorsque vous synchronisez l’application avec Marketo.

## Synchronisation de l’application avec Marketo {#sync-the-app-with-marketo}

L’application Marketo Events fonctionne indépendamment jusqu’à ce que vous resynchronisiez votre activité sur la base de données Marketo. Il est préférable de se synchroniser dès que possible après la dernière archivage. Votre tablette doit être connectée à Internet.

>[!CAUTION]
>
>Une fois la synchronisation effectuée, vous ne pouvez pas inverser l’archivage à partir de l’application.

1. Sur votre tablette, ouvrez l’application et accédez à votre événement.

1. Appuyer **Synchronisation**.

   Votre événement est mis à jour avec de nouveaux check-ins dans la base de données Marketo. Le compteur rouge sur le bouton Synchroniser s’efface, jusqu’à ce que vous identifiiez quelqu’un d’autre.

   Pour des raisons de sécurité, vous devez quitter l’application Marketo Events une fois la synchronisation terminée.

## Utilisation d’un accès Internet limité {#working-with-limited-internet-access}

Certains lieux ont un accès internet pourri. Vous avez besoin d’une bonne connexion à :

* Télécharger et installer l’application
* Se connecter
* Sélection d’un événement
* Synchronisation de l’application avec Marketo

Si l’accès à Internet vous préoccupe, vous pouvez vous connecter à l’application Marketo Events et sélectionner votre événement à l’avance, à un emplacement disposant d’un accès Internet sécurisé. Ainsi, vous pouvez toujours utiliser l’application hors ligne. Ensuite, lorsque vous récupérez une connexion Internet, synchronisez-la immédiatement vers la base de données Marketo.

>[!TIP]
>
>Si vous ne disposez pas d’une connexion Internet, vous pouvez toujours créer une nouvelle personne pour qu’une personne s’enregistre. Il sera réconcilié avec la personne existante lorsque vous synchroniserez l’application.

>[!NOTE]
>
>L’application vous déconnecte automatiquement après huit heures d’inactivité.
