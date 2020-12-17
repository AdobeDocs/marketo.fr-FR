---
title: priorité-remplacement-pour-déclencher-campagnes
description: Remplacement des priorités pour les campagnes de déclenchement
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Remplacement des priorités pour les campagnes de déclenchement

<br> 

Les administrateurs peuvent remplacer la priorité définie par Marketo pour déclencher des campagnes afin de définir des priorités qui s’alignent mieux sur les objectifs de l’entreprise.

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement pour les campagnes de déclenchement et pour les utilisateurs qui se sont vus accorder l’autorisation &quot;Modifier la priorité Campaign Trigger&quot;.

>[!CAUTION]
>
>Il est vivement conseillé d’utiliser cette fonction sur un ensemble limité de campagnes stratégiques (25 est la valeur maximale recommandée). L’utilisation de la fonction de manière approximative sur un ensemble volumineux peut avoir un impact négatif sur l’exécution générale de la campagne.

## Priorité de remplacement

1. Dans votre campagne de déclenchement, cliquez sur l&#39;onglet **[!UICONTROL Planification]**, puis sur **[!UICONTROL Remplacer la priorité]**.

   ![Image un](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. Choisissez un nouveau niveau de priorité dans la liste déroulante. Cliquez sur **[!UICONTROL Confirmer]**.

   ![Image 2](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![Image trois](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* Vous pouvez vue la priorité par défaut de votre campagne dans la [!UICONTROL file d’attente de Campaign] sous [!UICONTROL Activités marketing]. Pour augmenter le taux d’exécution, nous vous recommandons de définir la priorité de votre campagne à un niveau supérieur à celui par défaut.
>* La priorité définie par l’utilisateur s’applique uniquement aux nouvelles personnes remplissant les conditions requises pour la campagne ; les personnes qui font déjà la queue ne seront pas touchées.


## Réinitialiser la priorité

1. Pour rétablir la priorité de la campagne par défaut, accédez à l&#39;onglet **[!UICONTROL Planification]** de votre campagne de déclenchement et cliquez sur **[!UICONTROL Réinitialiser la priorité]**.

   ![Image 4](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. Cliquez sur **[!UICONTROL Réinitialiser]** pour confirmer.

   ![Image 5](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>Les remplacements et les réinitialisations de priorité sont capturés dans la piste d’audit. Vous pouvez vue la [piste d’audit](https://docs.marketo.com/x/GZ2t) via la zone [!UICONTROL Admin] de l’expérience Classic.

## Octroi d’un accès de remplacement de priorité

>[!CAUTION]
>
>Seuls les administrateurs ou les utilisateurs ayant des responsabilités d’administrateur doivent avoir la priorité de campagne sur l’accès.

1. Dans la zone [!UICONTROL Admin], cliquez sur **[!UICONTROL Utilisateurs et rôles]**.

   ![Image six](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. Cliquez sur l&#39;onglet **[!UICONTROL Rôles]**, sélectionnez l&#39;utilisateur auquel vous souhaitez accorder l&#39;accès, puis cliquez sur **[!UICONTROL Modifier le rôle]**.

   ![Image sept](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. Sous [!UICONTROL Accéder aux Activités marketing], cochez **[!UICONTROL Modifier la priorité du déclencheur]**. Cliquez sur **[!UICONTROL Enregistrer]**.

   ![Image huit](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Priorité de la vue Campaign dans Marketo Classic

Vous pouvez vue la priorité de la campagne dans l&#39;[!DNL Classic] expérience en cliquant sur l&#39;onglet **[!UICONTROL Planifier]** dans une campagne de déclenchement.

![Image neuf](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>La priorité de l&#39;expérience [!DNL Classic] est la vue uniquement. La modification ou la réinitialisation de la priorité de la campagne n’est disponible que par l’intermédiaire du Marketo Sky.
