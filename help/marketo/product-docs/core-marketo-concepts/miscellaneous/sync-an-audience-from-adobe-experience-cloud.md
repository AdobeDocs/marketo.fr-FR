---
description: Synchronisation d’une audience à partir de Adobe Experience Cloud - Documents Marketo - Documentation du produit
title: Synchronisation d’une audience à partir de Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
source-git-commit: 86451f1027e74479a415a4c6654a2625275d4112
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Synchronisation d’une audience à partir de Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Un déploiement prêt pour la HIPAA d’une instance Marketo ne peut pas utiliser cette intégration.

>[!PREREQUISITES]
>
>[Configuration du mappage de l’organisation Adobe](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-organization-mapping.md)

## Synchronisation d’une audience {#how-to-sync-an-audience}

1. Dans Mon Marketo, cliquez sur le bouton **Base** mosaïque.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Cliquez sur le bouton **Nouveau** et sélectionnez **Synchronisation à partir de l’audience Experience Cloud**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Cliquez sur le bouton **Dossier de bibliothèque d’audiences** et sélectionnez le dossier d’origine souhaité.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Sélectionnez une **Nom de l’audience**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Pour la destination, vous pouvez sélectionner une liste existante ou en saisir un nouveau. Dans cet exemple, nous en créons un nouveau. Cliquez sur **Synchronisation** une fois terminé.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Cliquez sur **OK**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## FAQ {#faq}

**Comment fonctionne la synchronisation des cookies ?**

Lorsque la synchronisation des cookies est activée pour votre abonnement Marketo, le fichier munchkin.js de Marketo tente de capturer et de stocker les ECID d’Adobe de l’organisation IMS Adobe que vous avez spécifiée lors de la configuration de l’intégration et de faire correspondre ces ECID à l’identifiant de cookie Marketo correspondant. Cela permet aux profils utilisateur anonymes de Marketo d’être enrichis avec des ECID d’Adobe.

Une autre étape est nécessaire pour associer le profil utilisateur anonyme à un profil de piste, qui est identifié à l’aide d’un email en texte brut. Fonctionnement exact [est décrit ici](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md).

**Pourquoi la taille de la liste dans Marketo est-elle différente de celle de l’Adobe ?**

Une personne ne se synchronise pas non plus si nous ne parvenons pas à lier un identifiant de cookie ECID à une personne connue dans Marketo.

**S’agit-il d’une synchronisation unique ?**

Vous ne devez lancer la synchronisation qu’une seule fois. Ensuite, les enregistrements seront synchronisés automatiquement. La synchronisation initiale peut prendre jusqu’à 24 heures ; à partir de maintenant, les nouveaux enregistrements seront synchronisés dans 2 à 3 heures.
