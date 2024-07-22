---
unique-page-id: 10097199
description: Notes de mise à jour - Hiver 16 - Documents Marketo - Documentation du produit
title: Notes de mise à jour - Hiver 2016
exl-id: 1e3b9207-27fe-47b1-b709-1306ac57b93b
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 4%

---

# Notes de mise à jour : hiver 16 {#release-notes-winter}

Les fonctionnalités suivantes sont incluses dans la version de l’hiver 16. Cliquez sur les liens de titre pour afficher des articles détaillés pour chaque fonctionnalité.

## [Is Anonymous Filter](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) {#is-anonymous-filter}

Le filtre Is Anonymous a été supprimé pour les listes dynamiques. Pour plus d’informations, consultez la [FAQ sur le suivi de Munchkin de nouvelle génération](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) . Cette modification n’a aucune incidence sur le Web Personalization (RTP), qui continue à identifier les visiteurs web anonymes et connus et à personnaliser le contenu en temps réel pour ces visiteurs.

## [Tableau de bord de la base de données](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md) {#database-dashboard}

La base de données de piste comporte un tableau de bord de résumé mis à jour qui comprend la taille totale de la base de données des personnes, le nombre de pistes commercialisables et une ventilation des pistes par les cinq premières sources.

![](assets/image2016-1-12-16-3a18-3a7.png)

## [Navigateur Microsoft Edge](/help/marketo/product-docs/administration/setup-administration/supported-browsers.md) {#microsoft-edge-browser}

Nous avons ajouté Microsoft Edge à la [liste des navigateurs](https://docs.marketo.com/display/public/DOCS/Supported+Browsers) pris en charge par Marketo.

## [Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) {#microsoft-outlook}

[Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) est désormais pris en charge.

## [Programme d’e-mail Head Start](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) {#email-program-head-start}

Utilisez l’option Démarrage anticipé pour indiquer que le traitement de votre envoi doit avoir lieu à l’avance. Au lieu de qualifier les pistes et de préparer les emails à l’heure planifiée du programme, Head Start s’assure que ces tâches sont effectuées au préalable. Ainsi, votre audience commencera à recevoir des emails à l’heure planifiée.

![](assets/image2016-1-11-15-3a38-3a3.png)

Pour utiliser cette fonctionnalité, le programme de messagerie électronique doit être planifié au moins 12 heures à l’avance et la liste dynamique sera verrouillée 12 heures avant l’envoi.

![](assets/image2016-1-11-15-3a35-3a55.png)

>[!NOTE]
>
>Cette fonctionnalité sera déployée progressivement pendant une semaine après la version de l’hiver 16. Il n’est pas disponible pour une utilisation avec les campagnes intelligentes ou l’API.

## [Améliorations du marketing mobile](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md) {#mobile-marketing-enhancements}

**Prise en charge de PhoneGap :** Nous offrons désormais la prise en charge de PhoneGap pour votre application mobile. [En savoir plus](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/phonegap).

**Prise en charge des applications Sandbox** :

![](assets/image2016-1-12-10-3a47-3a13.png)

## [Programmation et API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/assets/programs) {#program-api}

Créez, mettez à jour et clonez des programmes via l’API REST. Cela n’inclut pas la création ou la mise à jour de listes dynamiques et de campagnes dynamiques dans un programme.

## [Améliorations de Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#microsoft-dynamics-enhancements}

**[État de synchronisation](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md)** : conservez des onglets sur le débit actuel et le journal de la synchronisation. Ventilez-la selon le nombre d’insertions et de mises à jour par objet.

![](assets/pending-backog-cropped.png)

**[Notifications](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)** : soyez averti des erreurs de synchronisation courantes, ainsi que de la liste des pistes qui comportent cette erreur.

![](assets/image2016-1-12-8-3a13-3a9.png)

## [Améliorations des objets personnalisés](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md) {#custom-objects-enhancements}

Vous pouvez désormais créer des relations de type &quot;plusieurs à plusieurs&quot; entre les pistes/comptes et un objet personnalisé en utilisant un objet intermédiaire avec plusieurs champs de lien.

![](assets/image2016-1-11-12-3a59-3a59.png)

## [Publicités de lead Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) {#facebook-lead-ads}

[ Les publicités de piste Facebook](https://www.facebook.com/business/a/lead-ads) sont un moyen plus direct pour une entreprise d’exécuter des campagnes de génération de pistes sur Facebook. Les utilisateurs remplissent un formulaire pour exprimer leur intérêt pour un produit ou un service, de sorte que l’entreprise puisse les suivre. L’intégration de Marketo avec Facebook Lead Ads capture automatiquement les informations fournies par un prospect dans le formulaire de piste publicitaire. Les actions de suivi et les notifications peuvent ensuite être automatisées à l’aide du nouveau déclencheur Fills Out Facebook Lead Ads.

![](assets/image2016-1-11-10-3a20-3a39.png)

## [Planificateur de campagne web (Personalization en temps réel)](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/schedule-a-web-campaign.md) {#web-real-time-personalization-campaign-scheduler}

Planifiez votre campagne à l’avance. Configurez des dates de début et de fin pour le contenu web personnalisé et répétez les campagnes selon des jours et des heures spécifiques. Personnalisez le planning pour afficher la campagne en fonction de l&#39;heure du visiteur web ou d&#39;un fuseau horaire sélectionné.

![](assets/image2016-1-14-8-3a36-3a36.png)
