---
description: Synchronisation d’une audience à partir de Adobe Experience Cloud - Documents Marketo - Documentation du produit
title: Synchronisation d’une audience à partir de Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Synchronisation d’une audience à partir de Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Un déploiement prêt pour la HIPAA d’une instance Marketo ne peut pas utiliser cette intégration.

>[!PREREQUISITES]
>
>[Configuration du mappage de l’organisation Adobe](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Synchronisation d’une audience {#how-to-sync-an-audience}

1. Dans My Marketo, cliquez sur la mosaïque **[!UICONTROL Base de données]** .

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Cliquez sur la liste déroulante **[!UICONTROL New]** et sélectionnez **[!UICONTROL Synchroniser avec l’audience Experience Cloud]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Dossier de bibliothèque d’audiences]** et sélectionnez le dossier d’origine de votre choix.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Sélectionnez un **[!UICONTROL nom d’audience]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Pour la destination, vous pouvez sélectionner une liste existante ou en saisir un nouveau. Dans cet exemple, nous en créons un nouveau. Cliquez sur **[!UICONTROL Synchroniser]** une fois terminé.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Cliquez sur **[!UICONTROL OK]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Questions fréquentes {#faq}

**Comment fonctionne la synchronisation des cookies ?**

Lorsque la synchronisation des cookies est activée pour votre abonnement Marketo, Marketo qui  munchkin.js tente de capturer et de stocker les ECID d’Adobe pour l’organisation IMS Adobe que vous avez spécifiée lors de la configuration de l’intégration et de faire correspondre ces ECID à l’identifiant de cookie Marketo correspondant. Cela permet à Marketo de  des profils utilisateur anonymes afin de les enrichir avec des ECID Adobes.

Une autre étape est nécessaire pour associer le profil utilisateur anonyme à un profil de piste, qui est identifié à l’aide d’un email en texte brut. La façon exacte dont cela fonctionne [est décrite ici](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Pourquoi la taille de liste dans Marketo est-elle différente de celle de l’Adobe ?**

Une personne ne se synchronise pas non plus si nous ne parvenons pas à lier un identifiant de cookie ECID à une personne connue dans Marketo.

**S’agit-il d’une synchronisation unique ?**

Vous ne devez lancer la synchronisation qu’une seule fois. Ensuite, les enregistrements seront synchronisés automatiquement. La synchronisation initiale peut prendre jusqu’à 24 heures ; à l’avenir, de nouveaux enregistrements seront synchronisés dans 2 à 3 heures.
