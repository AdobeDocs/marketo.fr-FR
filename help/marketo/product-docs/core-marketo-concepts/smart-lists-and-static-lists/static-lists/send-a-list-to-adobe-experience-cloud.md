---
unique-page-id: 37356194
description: Envoyer une liste à Adobe Experience Cloud - Documents Marketo - Documentation du produit
title: Envoi d’une liste à Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
feature: Static Lists
source-git-commit: c10ecc0ccad28f2e480343acefe10f5eca2ae578
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 1%

---

# Envoi d’une liste à Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Un déploiement conforme à la loi HIPAA d’une instance de Marketo Engage ne peut pas utiliser cette fonctionnalité.

>[!PREREQUISITES]
>
>[Configurer le mappage d&#39;une organisation d&#39;Adobe ](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Applications de destination prises en charge {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (_uniquement_ si vous possédez une licence Adobe Audience Manager)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-Time Customer Data Platform
* Adobe Target

## Comment envoyer une liste statique {#how-to-send-a-static-list}

Une liste statique, c&#39;est tout. Aucune modification ne sera apportée à la liste dans Adobe Experience Cloud à moins que vous ne les apportiez manuellement.

1. Dans Marketo, recherchez la liste à exporter. Cliquez dessus avec le bouton droit et sélectionnez **[!UICONTROL Envoyer à l’Experience Cloud]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Dossier d’Audience Manager]** et sélectionnez le dossier de destination souhaité dans l’Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. Choisissez de créer une audience ou de remplacer une audience existante (dans cet exemple, nous en créons une nouvelle). Saisissez le nouveau nom d’audience et cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. Cliquez sur **[!UICONTROL OK]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >L’Adobe de l’abonnement de l’audience peut prendre jusqu’à 6 à 8 heures.

## Comment envoyer une liste synchronisée {#how-to-send-a-synced-list}

La synchronisation d’une liste signifie que chaque fois que vous mettez à jour une liste dans Marketo, cette modification se synchronise automatiquement avec son audience dans Adobe Experience Cloud.

1. Dans Marketo, recherchez la liste à exporter. Cliquez dessus avec le bouton droit et sélectionnez **[!UICONTROL Envoyer à l’Experience Cloud]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. Cliquez sur la liste déroulante **[!UICONTROL Dossier de la bibliothèque d’audiences]** et sélectionnez le dossier de destination de votre choix dans l’Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. Choisissez de créer une audience ou de remplacer une audience existante (dans cet exemple, nous en créons une nouvelle). Saisissez le nom de la nouvelle audience, cochez la case **[!UICONTROL Garder l’appartenance à l’audience synchronisée]**, puis cliquez sur **[!UICONTROL Envoyer]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. Cliquez sur **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## Comment arrêter une synchronisation de liste {#how-to-stop-a-list-sync}

Vous pouvez arrêter la synchronisation de votre liste à tout moment.

1. Dans Marketo, recherchez la liste dont vous souhaitez arrêter la synchronisation, puis cliquez dessus avec le bouton droit. Cliquez sur **[!UICONTROL Arrêter la synchronisation de la liste]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. Sélectionnez la ou les audiences que vous souhaitez arrêter de synchroniser, puis cliquez sur **[!UICONTROL Arrêter]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. Cliquez sur **[!UICONTROL Arrêter]** pour confirmer.

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## Éléments à noter {#things-to-note}

**Partage vers Adobe Analytics**

* Pour les clients qui possèdent à la fois Adobe Audience Manager et Adobe Analytics, cette intégration permet le partage des audiences de Marketo vers vos suites de rapports Adobe Analytics. Toutefois, des étapes de configuration supplémentaires doivent être effectuées dans Adobe Audience Manager pour activer ce partage. Veuillez consulter la [documentation de Adobe Audience Manager](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html){target="_blank"} pour plus d&#39;informations sur la configuration.

* Si une liste est vide ou ne comporte aucune personne avec des valeurs ECID, le nom de la liste n’est pas transmis pour être référencé en dehors de Marketo Engage.

**Utilisation des caractéristiques pour les clients Adobe Audience Manager**

Lorsque vous lancez une exportation de liste dans Marketo, vous remarquerez les modifications suivantes répercutées dans votre instance Adobe Audience Manager :

* Pour toutes les personnes de la liste exportée, Marketo écrira une caractéristique à l’aide de leurs e-mails hachés en tant qu’identifiant sur l’ensemble des appareils. Le nom de la caractéristique correspond au nom de l’audience de destination que vous avez spécifié lors de l’exportation.
* Pour tous les ECID que Marketo a réussi à faire correspondre aux personnes de la liste exportée, Marketo écrira une caractéristique à l’aide de l’identifiant d’appareil ECID. Le nom de la caractéristique correspond au nom de l’audience de destination que vous avez spécifié lors de l’exportation.
* Marketo crée également un segment dans votre instance d’Audience Manager en utilisant la caractéristique ECID comme seul critère de segmentation. Le nom du segment correspond au nom de l’audience de destination que vous avez spécifié lors de l’exportation.

## Questions fréquentes {#faq}

**Pourquoi la taille de la liste dans Marketo est-elle différente de celle dans l’Adobe ?**

L’intégration de l’audience fonctionne en synchronisant les cookies Marketo Munchkin avec le cookie ECID d’Adobe correspondant. Marketo ne peut partager des données d’abonnement que pour les personnes pour lesquelles Marketo a synchronisé un ECID. Pour des résultats optimaux, il est recommandé de charger le script de suivi munchkin.js de Marketo parallèlement au code de suivi visitor.js d’Adobe sur toutes les pages qui vous intéressent à des fins de marketing.

**Comment fonctionne la synchronisation des cookies ?**

Lorsque la synchronisation des cookies est activée pour votre abonnement Marketo, Marketo munchkin.js tente de capturer et de stocker les ECID Adobes pour l’organisation Adobe IMS que vous avez spécifiée lors de la configuration de l’intégration, puis de faire correspondre ces ECID à l’identifiant de cookie Marketo correspondant. Cela permet aux profils d’utilisateurs anonymes de Marketo d’être enrichis avec des ECID Adobes.

Une étape supplémentaire est nécessaire pour associer le profil utilisateur anonyme à un profil de personne, qui est identifié à l’aide d’un e-mail en texte brut. Le fonctionnement exact est [décrit ici](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Quelles informations sont partagées ?**

Cette intégration partage uniquement les informations d’appartenance à la liste de Marketo vers Adobe (par exemple, la connaissance du fait que la personne X est membre de la liste Y). Aucun attribut de personne supplémentaire n’est partagé avec l’Adobe via cette intégration.
