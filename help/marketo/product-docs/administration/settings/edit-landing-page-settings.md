---
unique-page-id: 2359918
description: Comment modifier le nom de domaine, la page de secours, le préremplissage de formulaire et d’autres options de page de destination.
title: Modifier les paramètres de la page de destination
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
TQID: https://experienceleague.adobe.com/dOvxpv09JPPBMNjqA0JTe-L4wIWUtkEELLl-PCs4CME
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 236
ht-degree: 7%

---

# Modifier les paramètres de la page de destination {#edit-landing-page-settings}

Vous pouvez modifier votre nom de domaine et votre page de secours, activer ou désactiver le préremplissage de formulaire, empêcher toute utilisation abusive de votre page de destination, etc. Suivez les étapes ci-après.

>[!NOTE]
>
>**Autorisations d’administration requises**

1. Accédez à la zone **[!UICONTROL Admin]**.

   ![](assets/edit-landing-page-settings-1.png)

1. Cliquez sur **[!UICONTROL Pages de destination]**.

   ![](assets/edit-landing-page-settings-2.png)

1. Dans la section **[!UICONTROL Pages de destination]**, cliquez sur **[!UICONTROL Modifier]**.

   ![](assets/edit-landing-page-settings-3.png)

1. Saisissez les informations relatives à votre domaine et à votre page.

   ![](assets/edit-landing-page-settings-4.png)

   | Terme | Définition |
   |---|---|
   | [!UICONTROL Nom de domaine pour les landing pages] | Il s’agit de votre CNAME. Un CNAME est la première partie de l’URL que vous fournissez aux personnes pour les pages de destination. Par exemple, dans `https://go.yourCompany.com`, le mot « go » correspond au CNAME. Vous pouvez en avoir plusieurs, mais la plupart des gens n’en utilisent qu’une seule. |
   | [!UICONTROL &#x200B; Page de secours &#x200B;] | C’est là que aller si la page de destination n’existe pas ou est en panne. En savoir plus sur les [pages de secours](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | [!UICONTROL Page d’accueil] | Saisissez l’URL de votre site d’entreprise. |

1. Cochez la case **[!UICONTROL Préremplissage de formulaire]** pour permettre aux formulaires de préremplir des informations pour des personnes connues (cookies). Décochez pour bloquer.

   ![](assets/edit-landing-page-settings-5.png)

   >[!NOTE]
   >
   >Si vous souhaitez que la balise de `<script>` de préremplissage s’affiche à la fin de la balise `<head>` dans le code, cochez la case **[!UICONTROL Insérer un script de préremplissage à la fin de la tête]**. Ne cochez pas cette case si vous souhaitez qu’elle apparaisse au début.
   >
   >Cochez la case **[!UICONTROL Supprimer les liens favicon par défaut]** pour empêcher Marketo d’insérer des liens favicon dans le code.

1. Après avoir effectué vos sélections, cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/edit-landing-page-settings-6.png)

   Vos landing pages disposent désormais des informations appropriées et devraient commencer à fonctionner immédiatement.
