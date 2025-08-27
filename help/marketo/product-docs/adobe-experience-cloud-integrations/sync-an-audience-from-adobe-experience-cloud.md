---
description: Synchroniser une audience à partir de Adobe Experience Cloud - Documents Marketo - Documentation du produit
title: Synchroniser une audience à partir de Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%

---

# Synchroniser une audience à partir de Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Un déploiement conforme à la norme HIPAA d’une instance Marketo ne peut pas utiliser cette intégration.

>[!PREREQUISITES]
>
>[Configurer le mappage d’organisation Adobe](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Comment synchroniser une audience {#how-to-sync-an-audience}

1. Dans Mon Marketo, cliquez sur la mosaïque **[!UICONTROL Base de données]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Nouveau]** et sélectionnez **[!UICONTROL Synchronisation depuis l’audience Experience Cloud]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Dossier de la bibliothèque d’audiences]** et sélectionnez le dossier d’origine de votre choix.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Sélectionnez un **[!UICONTROL Nom de l’audience]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Pour la destination , vous pouvez sélectionner une liste existante ou saisir le nom d’une nouvelle liste. Dans cet exemple, nous en créons un nouveau. Cliquez sur **[!UICONTROL Synchroniser]** lorsque vous avez terminé.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Cliquez sur **[!UICONTROL OK]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Questions fréquentes {#faq}

**Comment fonctionne la synchronisation des cookies ?**

Lorsque la synchronisation des cookies est activée pour votre abonnement Marketo, Marketo munchkin.js tente de capturer et de stocker les ECID Adobe pour l’organisation Adobe IMS que vous avez spécifiée lors de la configuration de l’intégration, puis de faire correspondre ces ECID à l’identifiant de cookie Marketo correspondant. Cela permet aux profils d’utilisateurs anonymes Marketo d’être enrichis avec les ECID Adobe.

Une étape supplémentaire est nécessaire pour associer le profil utilisateur anonyme à un profil de prospect, qui est identifié à l’aide d’un e-mail en texte brut. Le fonctionnement exact de cette procédure [est décrit ici](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Pourquoi la taille de la liste dans Marketo est-elle différente de celle dans Adobe ?**

Une personne ne se synchronise pas non plus si nous ne parvenons pas à lier un ID de cookie ECID à une personne connue dans Marketo.

**S’agit-il d’une synchronisation unique ?**

Il vous suffit de lancer la synchronisation une seule fois. Ensuite, les enregistrements seront automatiquement synchronisés. La synchronisation initiale peut prendre jusqu’à 24 heures. À l’avenir, les nouveaux enregistrements seront synchronisés dans 2 à 3 heures.
