---
unique-page-id: 2360368
description: Découvrez comment configurer Marketo Sales Insight dans les éditions Salesforce Enterprise/Unlimited.
title: Configuration de Marketo Sales Insight dans Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 3cbefabe80778b0502eaecd733b5732fd9003316
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 4%

---

# Configuration de Marketo Sales Insight dans Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Configurez Marketo Sales Insight dans les éditions Salesforce Enterprise/Unlimited en procédant comme suit.

>[!PREREQUISITES]
>
>[Installer le package Marketo Sales Insight dans l&#39;AppExchange Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Des autorisations d&#39;administrateur sont requises.**

## Configuration de Sales Insight dans Marketo Engage {#configure-sales-insight-in-marketo}

1. Pour obtenir vos informations d’identification Marketo Sales Insight en Marketo Engage, accédez à la zone **[!UICONTROL Admin]** et sélectionnez **[!UICONTROL Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Cliquez sur **[!UICONTROL Modifier la configuration de l’API]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Saisissez une clé secrète API de votre choix et cliquez sur **[!UICONTROL Enregistrer]**. N’utilisez PAS d’esperluette (`&`) dans votre clé secrète API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >Votre clé secrète d’API est semblable à un mot de passe pour votre organisation et doit être sécurisée.

1. Pour renseigner les informations d’identification, cliquez sur **[!UICONTROL Afficher]** dans le panneau _[!UICONTROL Configuration de l’API REST]_ .

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Lorsque la boîte de dialogue de confirmation s’affiche, cliquez sur **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Gardez cette fenêtre ouverte. Vous aurez besoin de ces informations ultérieurement pour la configuration Salesforce.

## Configuration de Sales Insight dans Salesforce {#configure-sales-insight-in-salesforce}

1. Dans Salesforce, cliquez sur **[!UICONTROL Setup]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Recherchez &quot;site distant&quot; et sélectionnez **[!UICONTROL Paramètres du site distant]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Cliquez sur **[!UICONTROL Nouveau site distant]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Saisissez le nom du site distant (il peut s’agir d’un élément similaire à `MarketoSoapAPI`). Saisissez l’URL du site distant, qui est l’URL de votre hôte Marketo à partir du panneau _[!UICONTROL Configuration de l’API Soap]_ dans Marketo Engage. Cliquez sur **[!UICONTROL Enregistrer]**. Vous avez maintenant créé des paramètres de site distant pour l’API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Cliquez à nouveau sur **[!UICONTROL Nouveau site distant]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Saisissez le nom du site distant (il peut s’agir d’un élément similaire à `MarketoAPI`). Saisissez l’URL du site distant, qui est l’URL de votre API issue du panneau _[!UICONTROL Configuration de l’API REST]_ en Marketo Engage. Cliquez sur **[!UICONTROL Enregistrer]**. Vous avez maintenant créé des paramètres de site distant pour l’API REST.

   >[!NOTE]
   >
   >_Vous_ choisissez votre **[!UICONTROL Nom du site distant]** (`MarketoAPI` ici). L’**[!UICONTROL URL de site distant]** se trouve dans le champ Hôte Marketo de votre boîte de dialogue Modifier la configuration de l’API à l’étape 3 de la section &quot;Configurer les statistiques de ventes dans Marketo&quot;.

## Octroi aux utilisateurs d’Insight sur les ventes d’un accès aux objets Salesforce standard {#grant-sales-insight-users-profile-access}

En raison des améliorations apportées à la sécurité de Salesforce, les modules d’AppExchange ne peuvent plus accorder d’autorisation aux objets standard, et l’accès doit être accordé aux objets Salesforce appropriés à partir du profil de l’utilisateur Salesforce. Pour accorder les autorisations requises, procédez comme suit.

1. Cliquez sur **[!UICONTROL Configuration]**.

1. Recherchez &quot;Profils&quot; dans Recherche rapide.

1. Cliquez sur **[!UICONTROL Modifier]** en regard du profil que vos utilisateurs Salesforce utilisent.

1. Dans la section _[!UICONTROL Autorisation d’objet standard]_, activez l’accès **[!UICONTROL en lecture]** pour les objets suivants : [!UICONTROL Lead], [!UICONTROL Contact], [!UICONTROL Account] et [!UICONTROL Opportunity].

1. Cliquez sur **[!UICONTROL Enregistrer]**.

## Personnalisation des dispositions de page {#customize-page-layouts}

1. Cliquez sur **[!UICONTROL Configuration]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Recherchez &quot;mise en page&quot; et sélectionnez la **[!UICONTROL mise en page]** sous **[!UICONTROL Pistes]**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Cliquez sur **[!UICONTROL Visualforce Pages]** à gauche. Faites glisser **[!UICONTROL Section]** vers la disposition sous la section _[!UICONTROL Liens personnalisés]_ .

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Saisissez &quot;Marketo Sales Insight&quot; comme **[!UICONTROL Nom de section]**, sélectionnez **[!UICONTROL 1-Column]**, puis cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Faites glisser **[!UICONTROL Lead]** et déposez-le dans la nouvelle section.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Le nom de cette zone change en fonction du type d’objet. Par exemple, si vous modifiez la mise en page des contacts, l’option Contact s’affiche.

1. Double-cliquez sur le bloc **[!UICONTROL Lead]** que vous venez d’ajouter.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Editez la hauteur à **450** pixels et cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Cochez la case **[!UICONTROL Afficher les barres de défilement]** si vous avez besoin d’accéder aux activités de défilement.

   >[!TIP]
   >
   >La hauteur recommandée pour les objets Comptes et opportunités est de 410 pixels.

1. Cliquez sur **[!UICONTROL Fields]** à gauche. Recherchez ensuite le libellé **[!UICONTROL Urgence]** et faites-le glisser dans la disposition **[!UICONTROL Marketo Sales Insight]** .

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Répétez également l’étape ci-dessus pour ces champs.

   * Dernier moment significatif
   * Date dernier moment significatif
   * Description dernier moment significatif
   * Source dernier moment significatif
   * Type dernier moment significatif
   * Dernière activité par vente
   * Dernier engagement par vente
   * Identifiant de contact MSI
   * Évaluation relative
   * Valeur d&#39;évaluation relative
   * Urgence
   * Valeur d&#39;urgence
   * Afficher dans Marketo

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Répétez les étapes 5 à 7 pour ajouter des sections de page Visualforce et des champs de statistiques sur les ventes pour **[!UICONTROL Contact]**, **[!UICONTROL Compte]** et **[!UICONTROL Opportunité]**.

1. Répétez les étapes 8 à 10 pour ajouter ces champs de statistiques sur les ventes pour **[!UICONTROL Contact]**. Veillez à enregistrer les modifications.

   * Dernier moment significatif
   * Date du dernier moment significatif
   * [!UICONTROL Dernier moment intéressant Desc]
   * [!UICONTROL Dernier moment intéressant Source]
   * [!UICONTROL Dernier type de moment intéressant]
   * [!UICONTROL Dernière activité Marketo par vente]
   * [!UICONTROL Dernier engagement Marketo par les ventes]
   * [!UICONTROL Score de piste MKTO]
   * [!UICONTROL Score relatif]
   * [!UICONTROL Valeur de score relatif]
   * [!UICONTROL Sales Insight] - Ouvre la page de liste complète des contacts
   * [!UICONTROL Urgence]
   * [!UICONTROL Valeur D’Urgence]

## Faire correspondre les champs de personne personnalisés {#map-custom-person-fields}

Les champs de personne Marketo doivent être mappés aux champs de contact Salesforce pour garantir le bon fonctionnement de la conversion. Suivez ces étapes pour les mapper.

1. Cliquez sur **[!UICONTROL Configuration]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Recherchez &quot;fields&quot; dans la barre de recherche et cliquez sur **[!UICONTROL Fields]** sous **[!UICONTROL Leads]**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Cliquez sur **[!UICONTROL Mapper les champs de piste]**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Cliquez sur la liste déroulante à droite de **[!UICONTROL Engagement]**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Sélectionnez **[!UICONTROL Contact.Engagement]** dans la liste.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Répétez et mappez également ces champs.

   | Champ personnalisé de personne Marketo | Champ personnalisé Contact Salesforce |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

## Onglet de configuration de Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. Dans Salesforce, cliquez sur le **+** à la fin de la barre d’onglets et cliquez sur **[!UICONTROL Marketo Sales Insight Config]**.

1. Copiez les informations d’identification du panneau API Soap dans la [page d’administration Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} et collez-les dans la section API Soap de la page de configuration Salesforce Sales Insight.

1. Copiez les informations d’identification du panneau API REST dans la [page d’administration de Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} et collez-les dans la section API REST de la page de configuration de Salesforce Sales Insight.

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

Vous devriez être en mesure d’afficher les champs Marketo Sales Insight pour les Leads, les contacts, les comptes et les opportunités.

>[!NOTE]
>
>Si le test de diagnostic échoue, l’ [ ajout de champs supplémentaires à la mise en page](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} peut résoudre le problème.

>[!NOTE]
>
>Pour les comptes, Sales Insight inclut tous les e-mails, mais uniquement les derniers moments intéressants, l’activité web et les changements de score.

>[!MORELIKETHIS]
>
>* [Priorité, urgence, note relative et meilleurs taux de misère](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Ajouter un onglet Marketo à Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Ajout de l’accès Sales Insight aux profils](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
