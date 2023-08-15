---
unique-page-id: 2359918
description: Modifier les paramètres de la page d’entrée - Documents Marketo - Documentation du produit
title: Modifier les paramètres de la page d’entrée
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
source-git-commit: 43565104a7f6512d2f99eae6bc47e1ae048b2231
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 6%

---

# Modifier les paramètres de la page d’entrée {#edit-landing-page-settings}

Vous pouvez modifier le nom de domaine et la page de secours, activer ou désactiver le préremplissage de formulaire, empêcher tout mauvais usage de votre landing page, etc. Voici comment.

>[!NOTE]
>
>**Autorisations d’administrateur requises**

1. Cliquez sur l&#39;icône **[!UICONTROL Admin]**.

   ![](assets/edit-landing-page-settings-1.png)

1. Cliquez sur **[!UICONTROL Pages de destination]**.

   ![](assets/edit-landing-page-settings-2.png)

1. Dans le **[!UICONTROL Pages d’entrée]** , cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/edit-landing-page-settings-3.png)

1. Renseignez les informations sur votre domaine et votre page.

   ![](assets/edit-landing-page-settings-4.png)

   | Terme | Définition |
   |---|---|
   | [!UICONTROL Nom de domaine des landing pages] | Il s’agit de votre CNAME. Un CNAME est la première partie de l’URL que vous donnez aux personnes pour les landing pages. Par exemple, dans `https://go.yourCompany.com`, le mot &quot;go&quot; est le CNAME. Vous pouvez avoir plusieurs, mais la plupart des gens utilisent seulement celui-ci. |
   | [!UICONTROL Page de secours] | C’est là que vous pouvez aller si la landing page n’existe pas ou est en panne. En savoir plus sur [pages de secours](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | [!UICONTROL Page d&#39;accueil] | Saisissez l’URL de votre site d’entreprise. |

1. Vérifiez les **[!UICONTROL Préremplissage de formulaire]** pour permettre aux formulaires de préremplir des informations pour les personnes connues (cookies). Décochez pour bloquer.

   ![](assets/edit-landing-page-settings-5.png)

   >[!NOTE]
   >
   >Si vous souhaitez préremplir la `<script>` s’affiche à la fin de la balise `<head>` dans le code, vérifiez les **[!UICONTROL Injection de script de préremplissage en fin d’en-tête]** de la boîte. Laissez cette option décochée si vous souhaitez qu’elle s’affiche au début.
   >
   >Vérifier **[!UICONTROL Suppression des liens de favicon par défaut]** pour empêcher Marketo d’insérer des liens favicon dans le code.

1. Après avoir effectué vos sélections, cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/edit-landing-page-settings-6.png)

   Très bon travail ! Vos landing pages contiennent maintenant les informations appropriées et doivent commencer à fonctionner immédiatement.
