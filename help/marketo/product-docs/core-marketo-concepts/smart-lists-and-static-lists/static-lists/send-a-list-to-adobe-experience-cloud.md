---
unique-page-id: 37356194
description: Envoyer une liste à Adobe Experience Cloud - Documents Marketo - Documentation du produit
title: Envoi d’une liste à Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
feature: Static Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 1%

---

# Envoi d’une liste à Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Un déploiement prêt pour la mise en PAA d’une instance de Marketo Engage ne peut pas utiliser cette fonctionnalité.

>[!PREREQUISITES]
>
>[Configuration du mappage de l’organisation Adobe](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Applications de destination prises en charge {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (_uniquement_ si vous possédez une licence Adobe Audience Manager)
* Adobe Audience Manager
* Gestionnaire d’expérience Adobe
* Adobe Real-Time Customer Data Platform
* Adobe Target

## Comment envoyer une liste statique {#how-to-send-a-static-list}

Une liste statique est juste statique. Aucune modification ne sera apportée à la liste dans Adobe Experience Cloud, sauf si vous les apportez manuellement.

1. Dans Marketo, recherchez la liste à exporter. Cliquez dessus avec le bouton droit de la souris et sélectionnez **[!UICONTROL Envoyer à l&#39;Experience Cloud]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Dossier d’Audience Manager]** et sélectionnez le dossier de destination de votre choix dans l’Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. Choisissez de créer une audience ou d&#39;en remplacer une existante (dans cet exemple, nous en créons une). Saisissez le nouveau nom de l&#39;audience et cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. Cliquez sur **[!UICONTROL OK]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >Il peut s’écouler entre 6 et 8 heures avant que l’appartenance à l’audience ne soit pleinement renseignée dans l’Adobe.

## Comment envoyer une liste synchronisée {#how-to-send-a-synced-list}

La synchronisation d’une liste signifie que chaque fois que vous mettez à jour une liste dans Marketo, la modification se synchronise automatiquement avec son audience dans Adobe Experience Cloud.

1. Dans Marketo, recherchez la liste à exporter. Cliquez dessus avec le bouton droit de la souris et sélectionnez **[!UICONTROL Envoyer à l&#39;Experience Cloud]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Dossier de bibliothèque d’audiences]** et sélectionnez le dossier de destination souhaité dans l’Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. Choisissez de créer une audience ou d&#39;en remplacer une existante (dans cet exemple, nous en créons une). Saisissez le nouveau nom de l’audience, cochez la case **[!UICONTROL Conserver l’appartenance à l’audience dans la synchronisation]**, puis cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. Cliquez sur **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## Comment arrêter une synchronisation de liste {#how-to-stop-a-list-sync}

Vous pouvez empêcher la synchronisation de votre liste à tout moment.

1. Dans Marketo, recherchez et cliquez avec le bouton droit sur la liste dont vous souhaitez arrêter la synchronisation. Cliquez sur **[!UICONTROL Arrêter la synchronisation de liste]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. Sélectionnez la ou les audiences dont vous souhaitez arrêter la synchronisation et cliquez sur **[!UICONTROL Arrêter]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. Cliquez sur **[!UICONTROL Arrêter]** pour confirmer.

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## Informations à noter {#things-to-note}

**Partage vers Adobe Analytics**

Pour les clients qui possèdent à la fois Adobe Audience Manager et Adobe Analytics, cette intégration permettra le partage des audiences de Marketo vers vos suites de rapports Adobe Analytics. Toutefois, d’autres étapes de configuration doivent être effectuées dans Adobe Audience Manager pour activer cette fonctionnalité. Pour plus d’informations sur la configuration de ce service, consultez la [documentation Adobe Audience Manager](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html){target="_blank"} .

**Utilisation des caractéristiques pour les clients Adobe Audience Manager**

Lorsque vous lancez l’exportation d’une liste dans Marketo, les modifications suivantes sont répercutées dans votre instance Adobe Audience Manager :

* Pour tous les Leads de la liste exportée, Marketo crée une caractéristique à l’aide des courriers électroniques hachés des Leads comme identifiant multi-appareils. Le nom de la caractéristique correspond au nom de l’audience de destination que vous avez spécifié lors de l’exportation.
* Pour tous les ECID que Marketo a réussi à faire correspondre aux Leads de la liste exportée, Marketo crée une caractéristique à l’aide de l’identifiant de périphérique ECID. Le nom de la caractéristique correspond au nom de l’audience de destination que vous avez spécifié lors de l’exportation.
* Marketo crée également un segment dans votre instance d’Audience Manager en utilisant la caractéristique ECID comme seul critère de segmentation. Le nom du segment correspond au nom de l’audience de destination que vous avez spécifié lors de l’exportation.

## Questions fréquentes {#faq}

**Pourquoi la taille de liste dans Marketo est-elle différente de celle de l’Adobe ?**

Sous le capot, l’intégration de l’audience fonctionne en synchronisant les cookies Marketo Munchkin avec le cookie ECID d’Adobe correspondant. Marketo peut uniquement partager des données d’adhésion pour les prospects pour lesquels Marketo a synchronisé un ECID. Pour obtenir de meilleurs résultats, il est recommandé de charger le script de suivi de Marketo munchkin.js en parallèle avec le code de suivi visitor.js d’Adobe sur toutes les pages que vous souhaitez suivre à des fins marketing.

**Comment fonctionne la synchronisation des cookies ?**

Lorsque la synchronisation des cookies est activée pour votre abonnement Marketo, Marketo qui  munchkin.js tente de capturer et de stocker les ECID d’Adobe pour l’organisation IMS Adobe que vous avez spécifiée lors de la configuration de l’intégration et de faire correspondre ces ECID à l’identifiant de cookie Marketo correspondant. Cela permet à Marketo de  des profils utilisateur anonymes afin de les enrichir avec des ECID Adobes.

Une autre étape est nécessaire pour associer le profil utilisateur anonyme à un profil de piste, qui est identifié à l’aide d’un email en texte brut. La façon exacte dont cela fonctionne est [décrite ici](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Quelles informations sont partagées ?**

Cette intégration partage uniquement les informations d’appartenance à la liste de Marketo vers l’Adobe (par exemple, la connaissance que le prospect X est membre de la liste Y). Aucun autre attribut de piste n’est partagé vers Adobe via cette intégration.
