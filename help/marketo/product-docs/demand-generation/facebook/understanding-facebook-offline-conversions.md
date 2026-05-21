---
unique-page-id: 11383945
description: Découvrez les conversions hors ligne Facebook et leur fonctionnement avec Marketo. Découvrez comment les données de conversion améliorent les performances publicitaires.
title: Présentation des conversions hors ligne Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
TQID: https://experienceleague.adobe.com/22t2foTWN-7xooxnnXuyk1l10kI-H4-gq0LbwbWSlns
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 241
ht-degree: 2%

---

# Présentation des conversions hors ligne [!DNL Facebook] {#understanding-facebook-offline-conversions}

Les campagnes de publicités de leads Facebook génèrent des leads et les envoient à Marketo pour une utilisation dans les campagnes marketing. Cependant, sans visibilité sur les conversions hors ligne, l’annonceur [!DNL Facebook] ne peut pas savoir quelles publicités sont les plus efficaces. Voici un exemple.

>[!NOTE]
>
>**Exemple**
>
>[!UICONTROL Facebook Lead Ads] diffuse trois publicités.
>
>* La publicité 1 génère 20 prospects
>* L’annonce 2 génère 30 prospects
>* L’annonce 3 génère 50 prospects
>
>Sur la seule base de ces chiffres, Ad 3 semble le plus efficace.
>
>Cependant, lorsque l’on examine les données du côté de Marketo, une autre histoire se développe.
>
>* La publicité 1 génère 10 ventes
>* La publicité 3 génère 2 ventes
>
>Cela signifie que l’annonce publicitaire 1, malgré le fait qu’elle génère moins de leads, a un taux de réussite de 50 %, tandis que l’annonce publicitaire 3 n’était quasiment pas efficace.
>
>Sans conversions hors ligne, l’annonceur investirait probablement plus d’argent dans la publicité 3. Avec les données de conversion hors ligne, l’annonceur investira probablement davantage dans la publicité 1.

Vous pouvez [configurer les conversions hors ligne Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) pour envoyer les performances publicitaires hors ligne à [!DNL Facebook].

1. Vérifiez que votre intégration [[!DNL Facebook] [!UICONTROL LaunchPoint]](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) est à jour.
1. Mappez les étapes de votre modèle de cycle du chiffre d’affaires sur les étapes de conversion hors ligne sur [!DNL Facebook].
1. Lorsqu’un prospect [!DNL Facebook] est généré à partir d’une publicité de prospect [!DNL Facebook] et atteint une étape mappée, Marketo renvoie des données de conversion hors ligne à [!DNL Facebook] plusieurs fois par jour via une API automatisée et sécurisée. Les données apparaissent dans le rapport [!DNL Facebook] Ads Manager.

>[!MORELIKETHIS]
>
>[Configurer [!DNL Facebook] Conversions hors ligne](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
