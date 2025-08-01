---
unique-page-id: 3571743
description: Découvrez comment configurer Marketo Sales Insight dans Salesforce Professional Edition.
title: Configuration de Marketo Sales Insight dans Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# Configuration de [!DNL Marketo Sales Insight] dans [!DNL Salesforce] Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Configurez Marketo Sales Insight dans Salesforce Professional Edition en procédant comme suit.

>[!PREREQUISITES]
>
>* Installez Marketo dans votre édition professionnelle d’[!DNL Salesforce].
>
>* [Installer [!DNL Marketo Sales Insight] Package dans [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}

>[!NOTE]
>
>**Des autorisations d’administrateur sont requises.**

## Configuration de Sales Insight dans Marketo Engage {#configure-sales-insight-in-marketo}

1. Pour obtenir les informations d’identification Marketo Sales Insight à partir de votre compte Marketo, ouvrez une nouvelle fenêtre de navigateur.

1. Dans la zone **[!UICONTROL Admin]**, sélectionnez **[!UICONTROL Insight commerciale]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Cliquez sur **[!UICONTROL Modifier la configuration de l’API]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Saisissez la clé secrète API de votre choix, puis cliquez sur **[!UICONTROL Enregistrer]**. N’utilisez PAS d’esperluette (`&`) dans votre clé secrète API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >Votre clé secrète API est semblable à un mot de passe pour votre organisation et doit être sécurisée.

1. Pour renseigner les informations d’identification, cliquez sur **[!UICONTROL Afficher]** dans le panneau _[!UICONTROL Configuration de l’API REST]_.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Lorsqu’une boîte de dialogue de confirmation s’affiche, cliquez sur **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Configuration de Sales Insight dans [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. Dans Salesforce, cliquez sur **[!UICONTROL Configuration]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Recherchez « site distant » et sélectionnez **[!UICONTROL Paramètres du site distant]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Cliquez sur **[!UICONTROL Nouveau site distant]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Saisissez le nom du site distant (il peut s’agir d’un nom similaire à `MarketoSoapAPI`). Saisissez l’URL du site distant, qui est votre URL d’hôte Marketo à partir du panneau Configuration de l’API Soap dans Marketo Engage. Cliquez sur **[!UICONTROL Enregistrer]**. Vous avez maintenant créé des paramètres de site distant pour l’API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Cliquez de nouveau sur **[!UICONTROL Nouveau site distant]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Saisissez le Nom du site distant (il peut s’agir d’un élément du type « MarketoRestAPI »). Saisissez l’URL du site distant, qui est votre URL d’API à partir du panneau Configuration de l’API REST dans Marketo. Cliquez sur **[!UICONTROL Enregistrer]**. Vous avez maintenant créé les paramètres du site distant pour l’API REST.

## Octroyer aux utilisateurs de Sales Insight l’accès aux objets Salesforce standard {#grant-sales-insight-users-profile-access}

En raison des améliorations apportées à la sécurité de Salesforce, les packages AppExchange ne peuvent plus accorder d’autorisation aux objets standard. En outre, l’accès doit être accordé aux objets Salesforce appropriés à partir du profil de l’utilisateur Salesforce. Accordez les autorisations requises en suivant ces étapes.

1. Cliquez sur **[!UICONTROL Configurer]**.

1. Recherchez « Profils » dans la recherche rapide.

1. Cliquez sur **[!UICONTROL Modifier]** en regard du profil utilisé par vos utilisateurs Salesforce.

1. Dans la section Autorisation d’objet standard , activez l’accès en lecture pour les objets suivants : Lead, Contact, Compte et Opportunité.

1. Cliquez sur **[!UICONTROL Enregistrer]**.

## Personnaliser les mises en page {#customize-page-layouts}

1. Cliquez sur **[!UICONTROL Configurer]**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Recherchez « mise en page » et sélectionnez le **[!UICONTROL Mise en page]** sous **[!UICONTROL Prospects]**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. Cliquez sur **[!UICONTROL Pages Visualforce]** sur la gauche. Faites glisser **[!UICONTROL Section]** vers la disposition sous la section Liens personnalisés.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Saisissez « Marketo Sales Insight » comme **[!UICONTROL Nom de la section]**. Sélectionnez **[!UICONTROL 1-Column]** et cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Glissez-déposez **[!UICONTROL Lead]** dans la nouvelle section.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >Le nom de cette zone change en fonction du type d’objet. Par exemple, si vous modifiez la mise en page des contacts, elle affiche Contact.

1. Double-cliquez sur le bloc **[!UICONTROL Lead]** que vous venez d’ajouter.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Modifiez la hauteur sur 450 pixels et cliquez sur **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Cochez la case **[!UICONTROL Afficher les barres de défilement]** si vous avez besoin d’accéder aux activités de défilement.

   >[!TIP]
   >
   >La hauteur recommandée pour les objets Comptes et Opportunités est de 410 pixels.

1. Cliquez sur **[!UICONTROL Champs]** à gauche. Recherchez ensuite le libellé **[!UICONTROL Engagement]** et faites-le glisser vers la disposition **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Répétez l&#39;étape précédente pour les champs suivants :

   * [!UICONTROL Engagement]
   * [!UICONTROL &#x200B; Valeur de score relative &#x200B;]
   * [!UICONTROL Valeur d’urgence]
   * [!UICONTROL Dernière date intéressante]
   * [!UICONTROL Desc Dernier moment intéressant]
   * [!UICONTROL Source du dernier moment intéressant]
   * [!UICONTROL Type de dernier moment intéressant]

1. Cliquez sur **[!UICONTROL Enregistrer]** lorsque vous avez terminé.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Pour ajouter des sections de page Visualforce pour **[!UICONTROL Contact]**, **[!UICONTROL Compte]** et **[!UICONTROL Opportunité]**, répétez les étapes 5 à 7.

1. Répétez les étapes 8 à 10 pour ajouter les champs Sales Insight pour **[!UICONTROL Contact]**. Veillez à enregistrer après toute modification.

## Mapper des champs de personne personnalisés {#map-custom-person-fields}

Les champs Personne de Marketo doivent être mappés aux champs Contact de Salesforce pour garantir le bon fonctionnement de la conversion. Pour les mapper, procédez comme suit.

1. Cliquez sur **[!UICONTROL Configurer]**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Recherchez « fields » dans la barre de recherche et cliquez sur **[!UICONTROL Fields]** sous **[!UICONTROL Leads]**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Cliquez sur **[!UICONTROL Mapper les champs de lead]**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Cliquez sur la liste déroulante à droite pour **[!UICONTROL Engagement]**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Sélectionnez **[!UICONTROL Contact.Engagement]** dans la liste.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. Répétez et mappez également ces champs.

   | Champ personnalisé de personne Marketo | Champ personnalisé du contact Salesforce |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

   {style="table-layout:auto"}

1. Lorsque vous avez terminé, cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Onglet Configuration de Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. Dans Salesforce, cliquez sur le signe **+** à l’extrémité de la barre d’onglets, puis cliquez sur **[!UICONTROL Configuration Insight des ventes Marketo]**.

1. Copiez les informations d’identification du panneau API Soap dans la page d’administration Marketo Sales Insight [&#128279;](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} et collez-les dans la section API Soap de la page Configuration Salesforce Sales Insight .

1. Copiez les informations d’identification du panneau **[!UICONTROL API REST]** dans la page d’administration Marketo Sales Insight [&#128279;](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} et collez-les dans la section API Rest de la page Configuration Salesforce Sales Insight.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

Vous devriez être en mesure de voir les champs Marketo Sales Insight pour les leads, les contacts, les comptes et les opportunités.

>[!NOTE]
>
>Si le test des diagnostics échoue, l’ajout [ champs supplémentaires à la mise en page ](https://nation.marketo.com/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} peut résoudre le problème.

>[!NOTE]
>
>Pour les comptes, Sales Insight inclut tous les e-mails, mais uniquement les moments intéressants les plus récents, l’activité web et les changements de score.

>[!MORELIKETHIS]
>
>* [Priorité, urgence, score relatif et meilleurs résultats](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [Ajouter l’onglet Marketo à  [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [Ajouter un accès Sales Insight aux profils](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
