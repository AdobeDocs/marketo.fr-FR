---
description: Synchroniser une Audience à partir de Adobe Experience Cloud - Marketo Docs - Documentation du produit
title: Synchroniser une Audience à partir de Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Synchroniser une Audience à partir de Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Un déploiement prêt pour la HIPAA d’une instance Marketo ne peut pas utiliser cette intégration.

>[!PREREQUISITES]
>
>[Configuration du partage des Audiences Adobe Experience Cloud](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## Synchronisation d’une Audience {#how-to-sync-an-audience}

1. Dans Mon Marketo, cliquez sur la mosaïque **Base de données**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Cliquez sur la liste déroulante **New** et sélectionnez **Synchroniser à partir de l’Audience Experience Cloud**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Cliquez sur la liste déroulante **Dossier de bibliothèque d’Audiences** et sélectionnez le dossier d’origine de votre choix.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Sélectionnez un **nom de l&#39;Audience**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Pour la destination, vous pouvez sélectionner une liste existante ou en saisir le nom. Dans cet exemple, nous en créons un nouveau. Cliquez sur **Synchroniser** lorsque vous avez terminé.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Cliquez sur **OK**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## FAQ {#faq}

**Comment fonctionne la synchronisation des cookies ?**

Lorsque la synchronisation des cookies est activée pour votre Abonnement Marketo, le fichier munchkin.js de Marketo tente de capturer et de stocker les ECID d’Adobe pour l’organisation IMS d’Adobe que vous avez spécifiée lors de la configuration de l’intégration et de faire correspondre ces ECID à l’identifiant de cookie Marketo correspondant. Cela permet aux profils utilisateurs anonymes de Marketo de s’enrichir avec des ECID d’Adobe.

Une autre étape est nécessaire pour associer le profil d’utilisateur anonyme à un Profil de piste, qui est identifié à l’aide d’un courrier électronique en texte brut. [est décrit ici](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md).

**Pourquoi la taille de la liste dans Marketo est-elle différente de celle de l&#39;Adobe ?**

Une personne ne sera pas synchronisée si nous ne pouvons pas lier un identifiant de cookie ECID à une personne connue à Marketo.

**Est-ce une synchronisation unique ?**

Il vous suffit de lancer la synchronisation une seule fois. Ensuite, les enregistrements seront synchronisés automatiquement. La synchronisation initiale peut prendre jusqu&#39;à 24 heures ; à partir de maintenant, les nouveaux enregistrements seront synchronisés dans 2 à 3 heures.
