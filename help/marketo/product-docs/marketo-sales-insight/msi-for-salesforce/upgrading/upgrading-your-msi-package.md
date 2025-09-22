---
unique-page-id: 37357050
description: Mise à niveau de votre package MSI - Documents Marketo - Documentation du produit
title: Mise à niveau de votre package MSI
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 3%

---

# Mise à niveau de votre package MSI {#upgrading-your-msi-package}

>[!IMPORTANT]
>
>En raison des améliorations de sécurité apportées par Salesforce, le package Sales Insight ne peut plus accorder d’autorisation aux objets standard. À l’avenir, le profil Salesforce des utilisateurs de Sales Insight devra disposer d’un accès en lecture aux objets standard suivants : lead, contact, compte et opportunité. [Découvrez comment configurer cela ici](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#grant-sales-insight-users-profile-access){target="_blank"}.

1. Accédez à [cette page dans appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}.

1. Connectez-vous à votre instance [!DNL Salesforce] (celle connectée à votre instance Marketo, peut être le sandbox ou la production) à partir du coin supérieur droit de la page à partir de l’étape 1. Vous devez disposer de droits d’administrateur pour installer/mettre à niveau un package géré dans [!DNL Salesforce].

1. Cliquez sur le bouton **Télécharger maintenant**. Il vous sera demandé de choisir l&#39;emplacement où vous souhaitez installer. Vous aurez la possibilité d&#39;effectuer la mise à niveau puisque vous disposez déjà d&#39;une version antérieure de MSI. Choisissez une option en fonction du compte auquel vous vous êtes connecté lors de la première étape.

   >[!TIP]
   >
   >Nous vous recommandons de tester cette opération sur votre instance Sandbox avant de mettre à niveau votre instance de production.

1. Vous pouvez mettre à niveau le package en choisissant « Installer pour les administrateurs uniquement » (et fournir un accès MSI à des profils spécifiques ultérieurement), « Installer pour tous les utilisateurs » ou « Installer pour des profils spécifiques ». Dans cet exemple, nous choisissons Administrateurs uniquement. Une fois votre sélection effectuée, cliquez sur **Mettre à niveau**.

   ![](assets/four.png)

>[!NOTE]
>
>Il est recommandé de mettre à jour le package uniquement pour les administrateurs, puis de [fournir l’accès à des utilisateurs spécifiques](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"} en fonction du nombre de places MSI achetées. Vous pouvez également créer un profil Salesforce spécifique pour les utilisateurs de MSI et installer ou mettre à niveau le package pour ces utilisateurs uniquement.
