---
unique-page-id: 27656223
description: Installation [!DNL Salesforce] personnalisation pour les clients Professional Edition - Documents Marketo - Documentation du produit
title: Installation [!DNL Salesforce] personnalisation pour les clients Professional Edition
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Installer [!DNL Salesforce] Customization pour les clients Professional Edition {#install-salesforce-customization-for-professional-edition-customers}

Les clients disposant de l’édition professionnelle de [!DNL Salesforce] devront suivre ces étapes pour installer la personnalisation.

>[!PREREQUISITES]
>
>* [!DNL Sales Connect] administrateur doit connecter ses comptes [!DNL Salesforce] et [!DNL Sales Connect].
>* [!DNL Salesforce]’instance utilisée doit disposer d’un espace suffisant pour installer treize champs d’activité personnalisés.

## Installation {#installation}

1. Dans [!DNL Sales Connect], cliquez sur l’icône d’engrenage en haut à droite et sélectionnez **[!UICONTROL Paramètres]**.

   ![](assets/one-4.png)

1. Sous [!UICONTROL Paramètres d’administration], cliquez sur **[!UICONTROL Salesforce]**.

   ![](assets/two-4.png)

1. Vérifiez que vous êtes connecté à votre compte [!DNL Salesforce].

   >[!CAUTION]
   >
   >Si vous êtes connecté, un bouton vert « [!UICONTROL Installer] » s’affiche. **NE PAS** cliquez sur ce bouton, passez plutôt à l’étape 4.

1. Connectez-vous au compte [!DNL Salesforce] auquel vous êtes connecté, puis cliquez sur [ce lien](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ).
1. Vous accédez à la page Installation de [!DNL Sales Connect].

   ![](assets/install-package.png)

1. Choisissez les utilisateurs pour lesquels vous souhaitez installer des personnalisations : administrateur uniquement, tous les utilisateurs ou des profils spécifiques.
1. Cliquez sur le bouton **[!UICONTROL Installer]** pour installer la personnalisation.
1. Pour confirmer la réussite de l’installation, connectez-vous à votre compte [!DNL Salesforce].
1. Cliquez sur **[!UICONTROL Configuration]**, recherchez « Packages installés » dans la barre de recherche, puis cliquez sur **[!UICONTROL Packages installés]**.

   Vous verrez ici les personnalisations de Marketo Sales Connect .

   Pour configurer [!DNL Sales Connect] dans votre instance [!DNL Salesforce], suivez les étapes en commençant par la section « CONFIGURATION DU PACKAGE SALESFORCE SALES ENGAGE » à la page 7 du Guide d’installation.

   >[!NOTE]
   >
   >[!DNL Sales Engage] est le nom précédent de [!DNL Sales Connect].

## Guides {#guides}

[Guide d’installation de Salesforce Classic](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[&#x200B; Guide d’installation de Salesforce Lightning &#x200B;](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
