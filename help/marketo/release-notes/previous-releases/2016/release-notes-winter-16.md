---
unique-page-id: 10097199
description: Notes De Mise À Jour - Hiver 16 - Documents Marketo - Documentation Du Produit
title: Notes de mise à jour - Hiver 16
exl-id: 1e3b9207-27fe-47b1-b709-1306ac57b93b
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 5%

---

# Notes de mise à jour : hiver 2016 {#release-notes-winter}

Les fonctionnalités suivantes sont incluses dans la version d’hiver 16. Cliquez sur les liens de titre pour afficher les articles détaillés de chaque fonctionnalité.

## [Filtre anonyme &#x200B;](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) {#is-anonymous-filter}

Le filtre Est anonyme a été supprimé pour les listes dynamiques. Consultez le document [FAQ sur le suivi de Munchkin de nouvelle génération](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) pour plus d’informations. Cette modification n’a aucune incidence sur le Personalization Web (RTP), qui continue d’identifier les visiteurs web anonymes et connus et de personnaliser le contenu en temps réel pour ces visiteurs.

## [Tableau de bord de la base de données](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md)  {#database-dashboard}

La [!UICONTROL base de données des leads] a un tableau de bord récapitulatif mis à jour qui inclut la taille totale de la base de données des personnes, le nombre de leads commercialisables et une répartition des leads par cinq principales sources.

![](assets/image2016-1-12-16-3a18-3a7.png)

## [Navigateur Microsoft Edge](/help/marketo/product-docs/administration/setup-administration/supported-browsers.md) {#microsoft-edge-browser}

Nous avons ajouté [!DNL Microsoft Edge] à la [liste des navigateurs](https://docs.marketo.com/display/public/DOCS/Supported+Browsers) pris en charge par Marketo.

## [Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) {#microsoft-outlook}

[[!DNL Microsoft Outlook] 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) est désormais pris en charge.

## [Programme d’e-mail Head Start](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) {#email-program-head-start}

Utilisez [!UICONTROL Démarrage rapide] pour indiquer que le traitement de votre envoi doit avoir lieu à l’avance. Au lieu de qualifier les leads et de préparer les e-mails au moment prévu du programme, [!UICONTROL Démarrage rapide] s&#39;assure que ces tâches sont effectuées à l&#39;avance. Ainsi, votre audience commencera à recevoir des e-mails à l’heure planifiée.

![](assets/image2016-1-11-15-3a38-3a3.png)

Pour utiliser cette fonctionnalité, le programme de messagerie doit être planifié au moins 12 heures à l’avance et la liste dynamique sera verrouillée 12 heures avant l’envoi.

![](assets/image2016-1-11-15-3a35-3a55.png)

>[!NOTE]
>
>Cette fonctionnalité sera déployée progressivement pendant une semaine à compter de la version d’hiver 16. Elle ne peut pas être utilisée avec les campagnes intelligentes ou l’API.

## [Améliorations du marketing mobile](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md) {#mobile-marketing-enhancements}

Assistance **[!DNL PhoneGap]:** nous proposons désormais une assistance [!DNL PhoneGap] pour votre application mobile. [En savoir plus](https://developers.marketo.com/documentation/mobile/phonegap-plugin/).

**Prise en charge des applications Sandbox** :

![](assets/image2016-1-12-10-3a47-3a13.png)

## [Programmation et API](https://developers.marketo.com/documentation/programs/) {#program-api}

Créer, mettre à jour et cloner des programmes via l’API REST. Cela n’inclut pas la création ou la mise à jour de listes intelligentes et de campagnes intelligentes au sein d’un programme.

## [Améliorations de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#microsoft-dynamics-enhancements}

**[[!UICONTROL Statut de la synchronisation]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md)** : suivez le débit actuel et la liste d’attente du processus de synchronisation. Ventilez-la en fonction du nombre d&#39;insertions et de mises à jour par objet.

![](assets/pending-backog-cropped.png)

**[[!UICONTROL Notifications]](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)** : recevez des notifications pour les erreurs de synchronisation courantes, ainsi qu’une liste des prospects présentant cette erreur.

![](assets/image2016-1-12-8-3a13-3a9.png)

## [Améliorations des objets personnalisés](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md) {#custom-objects-enhancements}

Vous pouvez désormais créer des relations multiples-à-multiples entre les prospects/comptes et un objet personnalisé à l’aide d’un objet intermédiaire avec plusieurs champs de lien.

![](assets/image2016-1-11-12-3a59-3a59.png)

## [Publicités de lead Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) {#facebook-lead-ads}

[[!UICONTROL Les annonces de leads Facebook]](https://www.facebook.com/business/a/lead-ads) sont un moyen plus direct pour une entreprise d’exécuter des campagnes de génération de leads sur [!DNL Facebook]. Les gens remplissent un formulaire pour exprimer leur intérêt pour un produit ou un service, afin que l&#39;entreprise puisse faire un suivi auprès d&#39;eux. L’intégration de Marketo à [!UICONTROL Facebook Lead Ads] capture automatiquement les informations fournies par un prospect dans le formulaire de prospect publicitaire. Les actions de suivi et les notifications peuvent ensuite être automatisées à l’aide du nouveau déclencheur [!UICONTROL Remplit les publicités du lead Facebook].

![](assets/image2016-1-11-10-3a20-3a39.png)

## [Planificateur De Campagnes Web (Real-Time Personalization)](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/schedule-a-web-campaign.md) {#web-real-time-personalization-campaign-scheduler}

Planifiez votre campagne à l’avance. Configurez des dates de début et de fin pour le contenu web personnalisé et des campagnes répétées à des jours et heures spécifiques. Personnalisez le planning pour afficher la campagne en fonction de l’heure du visiteur web ou d’un fuseau horaire sélectionné.

![](assets/image2016-1-14-8-3a36-3a36.png)
