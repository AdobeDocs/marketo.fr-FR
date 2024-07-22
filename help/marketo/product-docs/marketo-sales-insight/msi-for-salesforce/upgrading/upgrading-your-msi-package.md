---
unique-page-id: 37357050
description: Mise à niveau de votre package MSI - Documents Marketo - Documentation du produit
title: Mise à niveau de votre package MSI
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
feature: Marketo Sales Insights
source-git-commit: ddc9242bdf1b3ec34bb2672821b6b054647d94b5
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Mise à niveau de votre package MSI {#upgrading-your-msi-package}

>[!IMPORTANT]
>
>En raison des améliorations de sécurité apportées par Salesforce, le package Sales Insight ne peut plus accorder d’autorisation sur les objets standard. Dorénavant, le profil Salesforce des utilisateurs de Sales Insight devra disposer d’un accès en lecture aux objets standard suivants : prospect, contact, compte et opportunité. [Découvrez comment configurer cela ici](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#grant-sales-insight-users-profile-access){target="_blank"}.

1. Accédez à [cette page dans l’échange d’applications](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target="_blank"}.

1. Connectez-vous à votre instance Salesforce (celle connectée à votre instance Marketo, peut être sandbox ou production) à partir du coin supérieur droit de la page à partir de l’étape 1. Vous devez disposer de droits d’administrateur pour installer/mettre à niveau un package géré dans Salesforce.

1. Cliquez sur le bouton **Obtenir maintenant** . Il vous sera demandé de choisir l’emplacement où vous souhaitez installer. Vous aurez la possibilité de mettre à niveau car vous disposez déjà d’une version précédente de MSI. Choisissez une option en fonction du compte auquel vous vous êtes connecté à l’étape 1.

   >[!TIP]
   >
   >Nous vous recommandons de le tester sur votre instance sandbox avant de mettre à niveau votre instance de production.

1. Vous pouvez mettre à niveau le module en choisissant &quot;Installer pour les administrateurs uniquement&quot; (et fournir un accès MSI à des profils spécifiques ultérieurement), &quot;Installer pour tous les utilisateurs&quot; ou &quot;Installer pour des profils spécifiques&quot;. Dans cet exemple, nous choisissons Uniquement les administrateurs. Une fois la sélection effectuée, cliquez sur **Upgrade**.

   ![](assets/four.png)

>[!NOTE]
>
>Il est recommandé de mettre à jour le package uniquement pour les administrateurs, puis de [donner accès à des utilisateurs spécifiques](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"} en fonction du nombre de sièges MSI achetés. Vous pouvez également créer un profil Salesforce spécifique pour les utilisateurs MSI et installer ou mettre à niveau le module pour ces utilisateurs uniquement.
