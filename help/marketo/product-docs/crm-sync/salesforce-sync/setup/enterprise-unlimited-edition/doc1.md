---
description: Étape 1 sur 3 - Ajout de champs Marketo à Salesforce (Entreprise/Illimité) - Documents Marketo - Documentation du produit
title: Étape 1 sur 3 - Ajouter des champs Marketo à Salesforce (Entreprise/Illimité)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 1%

---

# Étape 1 sur 3 : ajouter des champs Marketo à Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>Vous devez avoir accès aux API Salesforce pour effectuer la synchronisation entre Marketo Engage et Salesforce.

Marketo utilise un ensemble de champs pour capturer certains types d’informations liées au marketing. Si vous souhaitez obtenir ces données dans Salesforce, suivez les instructions ci-dessous.

1. Créez trois champs personnalisés dans Salesforce sur les objets de prospect et de contact : Score, Programme d’acquisition et Date d’acquisition.
1. Mappez ces champs personnalisés entre les prospects et les contacts afin que les valeurs soient transférées lors de la conversion dans Salesforce.
1. Vous pouvez créer d’autres champs supplémentaires, si nécessaire (voir le tableau ci-dessous).

Tous ces champs personnalisés sont facultatifs et ne sont pas obligatoires pour synchroniser Marketo et Salesforce. Il est recommandé de créer des champs pour le score, le programme d’acquisition et la date d’acquisition.

## Ajout de champs Marketo à Salesforce {#add-marketo-fields-to-salesforce}

Ajoutez trois champs personnalisés sur les objets de lead et de contact dans Salesforce répertoriés ci-dessus. Si vous souhaitez en ajouter d&#39;autres, consultez le tableau des champs disponibles à la fin de cette section.

Effectuez les étapes suivantes pour chacun des trois champs personnalisés pour les ajouter. Commencez par le score.

1. Connectez-vous à Salesforce et cliquez sur Configuration.

   CAPTURE D’ÉCRAN

1. Dans la recherche rapide, recherchez le mot « Objet »

   CAPTURE D’ÉCRAN

1. Cliquez sur Gestionnaire d’objets et recherchez « Prospects ».

   CAPTURE D’ÉCRAN

1. Cliquez sur Lead sous LIBELLÉ, puis cliquez sur Champs et relations sur la gauche.

   CAPTURE D’ÉCRAN

1. Cliquez sur le bouton Nouveau de la page Champs et relations

   CAPTURE D’ÉCRAN

1. Sélectionnez le type de champ approprié (pour Score - Nombre ; Programme d&#39;acquisition - Texte ; Date d&#39;acquisition - Date/Heure).

   CAPTURE D’ÉCRAN

1. Cliquez sur Suivant.

   CAPTURE D’ÉCRAN

1. Saisissez le Libellé, la Longueur et le Nom du champ, comme illustré dans le tableau ci-dessous.

   TABLEAU

   >[!NOTE]
   >
   >Salesforce ajoute __c aux noms de champ lorsqu’il les utilise pour créer des noms d’API.

   CAPTURE D’ÉCRAN

   >[!NOTE]
   >
   >Les champs de texte et de nombre nécessitent une longueur, mais pas les champs Date/Heure. Une description est facultative.

1. Cliquez sur Suivant.

   CAPTURE D’ÉCRAN

1. Spécifiez les paramètres d’accès et cliquez sur Suivant :

   Définir tous les rôles sur Visible et Lecture seule

   Désélectionnez la case Lecture seule pour le profil de votre utilisateur de synchronisation :

   Si vous avez un utilisateur avec le profil d’un administrateur système en tant qu’utilisateur de synchronisation, désélectionnez la case Lecture seule pour le profil d’administrateur système (comme illustré ci-dessous)
Si vous avez créé un profil personnalisé pour l’utilisateur de synchronisation, décochez la case Lecture seule pour ce profil personnalisé

   CAPTURE D’ÉCRAN

1. Choisissez les mises en page qui doivent afficher le champ.

   CAPTURE D’ÉCRAN

1. Cliquez sur Enregistrer et Nouveau pour revenir en arrière et créer chacun des deux autres champs personnalisés. Cliquez sur Enregistrer avec vous. Vous avez terminé avec les trois.

   CAPTURE D’ÉCRAN

* Dans le Gestionnaire d&#39;objets, recherchez « Contacts ». Cliquez sur Champs et relations.
* Exécutez les étapes 5 à 12 pour les champs Score, Date d&#39;acquisition et Programme d&#39;acquisition sur l&#39;objet de contact, comme vous l&#39;avez fait pour l&#39;objet de prospect.
* Vous pouvez éventuellement utiliser la procédure ci-dessus pour tout champ personnalisé supplémentaire de ce tableau.

  TABLEAU

  >[!NOTE]
  >
  >Les valeurs des champs affectés automatiquement par Marketo ne seront pas immédiatement disponibles dans Salesforce une fois le nouveau champ créé. Marketo synchronise les données avec Salesforce lors de la prochaine mise à jour de l’enregistrement sur l’un des systèmes (c’est-à-dire une mise à jour de l’un des champs synchronisés entre Marketo et Salesforce).

## Mapper des champs personnalisés pour les conversions {#map-custom-fields-for-conversions}

Un champ personnalisé sur l’objet de prospect dans Salesforce doit être mappé à un champ de contact sur l’objet de contact afin que les données soient transférées lorsqu’une conversion se produit.

1. Dans le coin supérieur droit, cliquez sur Configurer.

   CAPTURE D’ÉCRAN

1. Dans la recherche rapide, recherchez le mot « Objet »

   CAPTURE D’ÉCRAN

1. Accédez à la section Champs personnalisés et relations du lead et cliquez sur Mapper les champs de lead

   CAPTURE D’ÉCRAN

1. Cliquez sur la liste déroulante en regard du champ à mapper, sous l’onglet correspondant - compte, contact ou opportunité .

   CAPTURE D’ÉCRAN

1. Sélectionnez le champ personnalisé de contact correspondant.

   CAPTURE D’ÉCRAN

1. Répétez les étapes ci-dessus pour tout autre champ que vous avez créé.

1. Cliquez sur Enregistrer lorsque vous avez terminé.
