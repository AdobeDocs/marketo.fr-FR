---
unique-page-id: 2949839
description: Envoyez des personnes à votre événement depuis votre tablette - Documents Marketo - Documentation du produit
title: Intégrer des personnes à votre événement à partir de votre tablette
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
feature: Mobile Marketing
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Intégrer des personnes à votre événement à partir de votre tablette {#check-people-into-your-event-from-your-tablet}

Lorsque les gens se présentent à votre événement, vous pouvez trouver leurs informations sur l&#39;application. Après l’enregistrement, ils sont promus au statut Participants lorsque vous effectuez une synchronisation avec Marketo.

>[!IMPORTANT]
>
>Le 2 octobre 2023, Adobe a supprimé l’application d’événements Marketo de tous les magasins d’applications. Si l’application est déjà installée sur votre tablette ou votre appareil mobile, vous pouvez continuer à l’utiliser pour le moment. Une fois votre instance Marketo Engage migrée vers Adobe Identity pour l’authentification de Marketo, vous ne pourrez plus accéder à l’application. [En savoir plus](https://nation.marketo.com/t5/product-discussions/marketo-events-app-and-marketo-moments-app-end-of-life/m-p/340712/highlight/true#M193869){target="_blank"}.

L’application fonctionne de la même manière sur [!DNL iPad] et [!DNL Android], à l’exception de légères différences de mise en page et de conception.

>[!PREREQUISITES]
>
>* Créez un événement dans Marketo et renseignez-le avec des personnes invitées et enregistrées.

## Enregistrer les invités enregistrés {#check-in-registered-guests}

1. Appuyez sur l’icône de l’application sur votre tablette [!DNL iPad] ou [!DNL Android].

1. Appuyez sur **[!UICONTROL Connexion]** pour lancer l’application Événement Marketo.

   ![](assets/1.jpg)

1. Saisissez votre nom d’utilisateur et votre mot de passe Marketo, puis cliquez sur **[!UICONTROL Connexion]**.

   >[!NOTE]
   >
   >Vous devez disposer d&#39;un rôle avec un accès à la base de données pour voir les personnes dans l&#39;application.

1. Sélectionnez un **[!UICONTROL Événement]**.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >Seuls les programmes d’événement (à l’exception des webinaires) planifiés une semaine avant et une semaine après la date d’aujourd’hui s’affichent.

1. Sur l’écran d’accueil, recherchez Invités enregistrés . Pour trouver une personne dans la liste, vous pouvez :

   * Défilement pour trouver un nom
   * Saisir un nom dans le champ de recherche
   * Accédez à une lettre initiale spécifique du nom en appuyant dessus sur le côté droit de la liste

   >[!NOTE]
   >
   >Le processus est le même sur [!DNL iPad] et [!DNL Android], mais les écrans diffèrent et les éléments peuvent se trouver à des emplacements différents. Cet article présente l’interface [!DNL iPad]. Comparez l’écran [!DNL Android] de cette section à titre de référence.

   **[!DNL iPad]**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **[!DNL Android]**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. Appuyez sur le nom sélectionné, puis sur l’enregistrement de la personne, appuyez sur **[!UICONTROL Archiver]**.

   ![](assets/img-0068-35-hands.png)

L’invité possède désormais le statut Terminé et reçoit une coche. L’enregistrement de personne est mis à jour lorsque vous effectuez une synchronisation avec Marketo. Le compteur rouge sur le bouton Synchroniser s’incrémente pour afficher le nombre d’archivages depuis la dernière synchronisation avec Marketo. Le bouton Synchroniser a un aspect différent et se trouve à un emplacement différent pour [!DNL iPad] et [!DNL Android] :

**[!DNL iPad]**

![](assets/image2016-4-12-14-3a25-3a13.png)

**[!DNL Android]**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>Si une personne est invitée mais ne s’est pas enregistrée, vous pouvez rechercher le nom en cliquant sur **[!UICONTROL Rechercher sur le serveur]**, juste en dessous de la zone de recherche. Le statut Invité passe à **[!UICONTROL Participé]** pour l’événement.

## Créer une nouvelle personne sur la tablette {#create-a-new-person-on-the-tablet}

Vous pouvez ajouter manuellement des invités qui ne sont pas des personnes existantes dans votre base de données Marketo. Ils seront automatiquement archivés et ajoutés à votre base de données lors de la synchronisation avec Marketo.

1. Cliquez sur **[!UICONTROL Ajouter]**.

   **[!DNL iPad]**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **[!DNL Android]**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. Renseignez autant de champs d’informations de base que possible et appuyez sur **[!UICONTROL Terminé]**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >Vous ne pouvez utiliser que les champs existants. Vous ne pouvez pas en créer de personnalisés.

   >[!CAUTION]
   >
   >Vérifiez à nouveau l’adresse e-mail. D’autres champs peuvent être corrigés ultérieurement, mais l’adresse e-mail est la méthode principale pour contacter l’invité.

La nouvelle personne est enregistrée comme étant connectée à votre événement et sera ajoutée à la base de données Marketo avec le statut Terminé lorsque vous effectuez une synchronisation avec Marketo.

## Inverser un enregistrement {#reverse-a-check-in}

Si vous avez archivé une personne par erreur, _avant la synchronisation avec Marketo_, vous pouvez annuler le statut [!UICONTROL Terminé].

1. Appuyez sur le nom dans la liste, puis sur **[!UICONTROL Annuler]** dans l’enregistrement de personne.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   Tout est arrangé !

## Modifier un enregistrement de personne lors de l’enregistrement {#edit-a-person-record-at-check-in}

Vous pouvez ajouter et modifier des informations sur les invités, dès l&#39;événement !

1. Appuyez sur le nom dans la liste des personnes, puis sur **[!UICONTROL Modifier]**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. Modifiez et ajoutez des informations aux champs, puis appuyez sur **[!UICONTROL Terminé]**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >Dans [!DNL Android], le bouton **[!UICONTROL Terminé]** peut être masqué. Faites défiler la page vers le bas pour le trouver.

Les informations sont mises à jour lorsque vous synchronisez l’application avec Marketo.

## Synchroniser l’application avec Marketo {#sync-the-app-with-marketo}

L’application Marketo Events fonctionne indépendamment jusqu’à ce que vous resynchronisiez votre activité avec la base de données Marketo. Il est préférable de synchroniser le plus tôt possible après le dernier enregistrement. Votre tablette doit être connectée à Internet.

>[!CAUTION]
>
>Une fois la synchronisation effectuée, vous ne pouvez pas annuler un enregistrement à partir de l’application.

1. Sur votre tablette, ouvrez l’application et accédez à votre événement.

1. Appuyez sur **[!UICONTROL Synchroniser]**.

   Votre événement est mis à jour avec de nouveaux enregistrements dans la base de données Marketo. Le compteur rouge sur le bouton Synchroniser se décoche jusqu&#39;à ce que vous consigniez quelqu&#39;un d&#39;autre.

   Pour des raisons de sécurité, vous devez quitter l’application Marketo Events une fois la synchronisation terminée.

## Utilisation d’un accès Internet limité {#working-with-limited-internet-access}

Certains établissements ont un accès internet de mauvaise qualité. Vous avez besoin d’une bonne connexion vers :

* Télécharger et installer l’application
* Se connecter
* Sélectionner un événement
* Synchroniser l’application avec Marketo

Si vous êtes préoccupé par l&#39;accès à Internet sur le site, vous pouvez vous connecter à l&#39;application Marketo Events et sélectionner votre événement à l&#39;avance, à un emplacement disposant d&#39;un accès Internet fort. De cette manière, vous pouvez toujours utiliser l’application hors ligne. Ensuite, lorsque vous retrouvez une connexion Internet, synchronisez immédiatement avec la base de données Marketo.

>[!TIP]
>
>Si vous ne disposez pas d&#39;une connexion Internet, vous pouvez toujours créer une nouvelle personne pour une personne qui s&#39;enregistre. Il se réconciliera avec la personne existante lorsque vous synchroniserez l&#39;application.

>[!NOTE]
>
>L’application vous déconnecte automatiquement après huit heures d’inactivité.
